# Comparing `tmp/clarifai-grpc-9.3.0.tar.gz` & `tmp/clarifai-grpc-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-grpc-9.3.0.tar", last modified: Mon Apr  3 17:07:21 2023, max compression
+gzip compressed data, was "clarifai-grpc-9.4.0.tar", last modified: Tue May  2 21:06:33 2023, max compression
```

## Comparing `clarifai-grpc-9.3.0.tar` & `clarifai-grpc-9.4.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.618907 clarifai-grpc-9.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-03 17:07:21.618907 clarifai-grpc-9.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.606907 clarifai-grpc-9.3.0/clarifai_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.610907 clarifai-grpc-9.3.0/clarifai_grpc/channel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/clarifai_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.610907 clarifai-grpc-9.3.0/clarifai_grpc/channel/custom_converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/custom_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12533 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/grpc_json_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/channel/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.610907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.610907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94275 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/resources_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   362258 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/resources_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/resources_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   229343 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   373513 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   363181 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.610907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20208 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    51533 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_code_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.614907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/extensions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/test_proto_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.614907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.614907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/scope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/scope/scope_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.618907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/types/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/types/types_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.618907 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/util/extension_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/util/extension_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:07:21.606907 clarifai-grpc-9.3.0/clarifai_grpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-03 17:07:21.000000 clarifai-grpc-9.3.0/clarifai_grpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-03 17:07:21.000000 clarifai-grpc-9.3.0/clarifai_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 17:07:21.000000 clarifai-grpc-9.3.0/clarifai_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-03 17:07:21.000000 clarifai-grpc-9.3.0/clarifai_grpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 17:07:21.000000 clarifai-grpc-9.3.0/clarifai_grpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 17:07:21.618907 clarifai-grpc-9.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-03 17:07:06.000000 clarifai-grpc-9.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.920432 clarifai-grpc-9.4.0/clarifai_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.924433 clarifai-grpc-9.4.0/clarifai_grpc/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/clarifai_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.924433 clarifai-grpc-9.4.0/clarifai_grpc/channel/custom_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/custom_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12533 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/grpc_json_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/channel/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.924433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.928433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94966 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/resources_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   364692 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/resources_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/resources_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   232549 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   381597 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   369799 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.932433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51755 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_code_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/extensions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/test_proto_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/scope/scope_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/types/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/types/types_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/util/extension_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/util/extension_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:06:33.920432 clarifai-grpc-9.4.0/clarifai_grpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-02 21:06:33.000000 clarifai-grpc-9.4.0/clarifai_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-02 21:06:33.000000 clarifai-grpc-9.4.0/clarifai_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:06:33.000000 clarifai-grpc-9.4.0/clarifai_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 21:06:33.000000 clarifai-grpc-9.4.0/clarifai_grpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 21:06:33.000000 clarifai-grpc-9.4.0/clarifai_grpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:06:33.936433 clarifai-grpc-9.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 21:06:14.000000 clarifai-grpc-9.4.0/setup.py
```

### Comparing `clarifai-grpc-9.3.0/LICENSE` & `clarifai-grpc-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/PKG-INFO` & `clarifai-grpc-9.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai-grpc
-Version: 9.3.0
+Version: 9.4.0
 Summary: Clarifai gRPC API Client
 Home-page: https://github.com/Clarifai/clarifai-python-grpc
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-grpc-9.3.0/README.md` & `clarifai-grpc-9.4.0/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/channel/clarifai_channel.py` & `clarifai-grpc-9.4.0/clarifai_grpc/channel/clarifai_channel.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py` & `clarifai-grpc-9.4.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py` & `clarifai-grpc-9.4.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/channel/grpc_json_channel.py` & `clarifai-grpc-9.4.0/clarifai_grpc/channel/grpc_json_channel.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/channel/http_client.py` & `clarifai-grpc-9.4.0/clarifai_grpc/channel/http_client.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/resources_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/resources_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from clarifai_grpc.grpc.api.utils import matrix_pb2 as proto_dot_clarifai_dot_api_dot_utils_dot_matrix__pb2
 from clarifai_grpc.grpc.auth.util import extension_pb2 as proto_dot_clarifai_dot_auth_dot_util_dot_extension__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"proto/clarifai/api/resources.proto\x12\x0c\x63larifai.api\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/api/utils/matrix.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xe5\x03\n\nAnnotation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x30\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x18\n\x10model_version_id\x18\x10 \x01(\t\x12\"\n\x16\x65mbed_model_version_id\x18\x0e \x01(\tB\x02\x18\x01\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07trusted\x18\n \x01(\x08\x42\x02\x18\x01\x12\x13\n\x0binput_level\x18\x11 \x01(\x08\x12/\n\x0e\x63onsensus_info\x18\x12 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07task_id\x18\x13 \x01(\tJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\xea\x03\n\x03\x41pp\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65\x66\x61ult_language\x18\x03 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ult_workflow_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14legal_consent_status\x18\x07 \x01(\r\x12)\n\x08metadata\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x11\n\tsample_ms\x18\x0f \x01(\r\x12,\n\nvisibility\x18\x10 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x14\n\x0c\x64\x61ta_tier_id\x18\x12 \x01(\t\x12\x12\n\nis_starred\x18\x13 \x01(\x08\x12\x12\n\nstar_count\x18\x14 \x01(\x05\x12\r\n\x05notes\x18\x15 \x01(\t\x12\"\n\x05image\x18\x16 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x18\n\x08\x41ppQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x90\x02\n\x0c\x43ollaborator\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12 \n\x04user\x18\x03 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x11\n\tendpoints\x18\x05 \x03(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ndeleted_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x01\n\rCollaboration\x12\x1e\n\x03\x61pp\x18\x01 \x01(\x0b\x32\x11.clarifai.api.App\x12%\n\tapp_owner\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x97\x01\n\x05\x41udio\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\naudio_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.AudioInfo\"b\n\tAudioInfo\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x03 \x01(\x02\x12\x10\n\x08\x62it_rate\x18\x04 \x01(\x05\"w\n\x05Track\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x04 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\x12\x0f\n\x07quality\x18\x05 \x01(\x02J\x04\x08\x03\x10\x04\"h\n\x07\x43luster\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x1f\n\x04hits\x18\x04 \x03(\x0b\x32\x11.clarifai.api.Hit\x12\x12\n\nprojection\x18\x05 \x03(\x02\"M\n\x05\x43olor\x12\x0f\n\x07raw_hex\x18\x01 \x01(\t\x12\x1e\n\x03w3c\x18\x02 \x01(\x0b\x32\x11.clarifai.api.W3C\x12\x13\n\x05value\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\" \n\x03W3C\x12\x0b\n\x03hex\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"/\n\x0cUserAppIDSet\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\"J\n\x0bPatchAction\x12\n\n\x02op\x18\x01 \x01(\t\x12!\n\x19merge_conflict_resolution\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"\xa9\x02\n\x07\x43oncept\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1a\n\x05value\x18\x03 \x01(\x02\x42\x0b\xd5\xb5\x18\x00\x00\x80?\x80\xb5\x18\x01\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x06 \x01(\t\x12\x12\n\ndefinition\x18\x07 \x01(\t\x12\x10\n\x08vocab_id\x18\x08 \x01(\t\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\n \x01(\t\x12\x31\n\rkeypoint_info\x18\x0b \x01(\x0b\x32\x1a.clarifai.api.KeypointInfo\"T\n\x0cKeypointInfo\x12\x16\n\x0ekeypoint_names\x18\x01 \x03(\t\x12,\n\x08skeleton\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.KeypointEdge\"&\n\x0cKeypointEdge\x12\n\n\x02k1\x18\x01 \x01(\r\x12\n\n\x02k2\x18\x02 \x01(\r\"\xa4\x01\n\x0c\x43onceptCount\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12:\n\x12\x63oncept_type_count\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12>\n\x14\x64\x65tail_concept_count\x18\x04 \x01(\x0b\x32 .clarifai.api.DetailConceptCount\"B\n\x10\x43onceptTypeCount\x12\x16\n\x08positive\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08negative\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"\xdf\x01\n\x12\x44\x65tailConceptCount\x12\x31\n\tprocessed\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nto_process\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12.\n\x06\x65rrors\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nprocessing\x18\x04 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\"C\n\x0c\x43onceptQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08language\x18\x02 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x03 \x01(\t\"\xd9\x01\n\x0f\x43onceptRelation\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x0fsubject_concept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\x12-\n\x0eobject_concept\x18\x03 \x01(\x0b\x32\x15.clarifai.api.Concept\x12\x11\n\tpredicate\x18\x04 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x05 \x01(\t\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"y\n\x0eKnowledgeGraph\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x17\n\x0f\x65xamples_app_id\x18\x04 \x01(\t\x12\x1f\n\x17sampled_examples_app_id\x18\x05 \x01(\t\"D\n\x11\x43onceptMappingJob\x12\x1a\n\x12knowledge_graph_id\x18\x01 \x01(\t\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"?\n\x0f\x43onceptLanguage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndefinition\x18\x03 \x01(\t\"\xfa\x04\n\x04\x44\x61ta\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Image\x12\"\n\x05video\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Video\x12\'\n\x08\x63oncepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x03geo\x18\x06 \x01(\x0b\x32\x11.clarifai.api.Geo\x12#\n\x06\x63olors\x18\x07 \x03(\x0b\x32\x13.clarifai.api.Color\x12\'\n\x08\x63lusters\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Cluster\x12+\n\nembeddings\x18\t \x03(\x0b\x32\x17.clarifai.api.Embedding\x12%\n\x07regions\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Region\x12#\n\x06\x66rames\x18\x0c \x03(\x0b\x32\x13.clarifai.api.Frame\x12 \n\x04text\x18\r \x01(\x0b\x32\x12.clarifai.api.Text\x12\"\n\x05\x61udio\x18\x0e \x01(\x0b\x32\x13.clarifai.api.Audio\x12#\n\x06tracks\x18\x0f \x03(\x0b\x32\x13.clarifai.api.Track\x12\x30\n\rtime_segments\x18\x10 \x03(\x0b\x32\x19.clarifai.api.TimeSegment\x12\x1f\n\x04hits\x18\x11 \x03(\x0b\x32\x11.clarifai.api.Hit\x12%\n\x08heatmaps\x18\x12 \x03(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x04\x10\x05J\x04\x08\n\x10\x0b\"\x86\x01\n\x06Region\x12\n\n\x02id\x18\x01 \x01(\t\x12-\n\x0bregion_info\x18\x02 \x01(\x0b\x32\x18.clarifai.api.RegionInfo\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\r\n\x05value\x18\x04 \x01(\x02\x12\x10\n\x08track_id\x18\x05 \x01(\t\"\xae\x02\n\nRegionInfo\x12/\n\x0c\x62ounding_box\x18\x01 \x01(\x0b\x32\x19.clarifai.api.BoundingBox\x12 \n\x04mask\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Mask\x12&\n\x07polygon\x18\x05 \x01(\x0b\x32\x15.clarifai.api.Polygon\x12\"\n\x05point\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Point\x12 \n\x04span\x18\x07 \x01(\x0b\x32\x12.clarifai.api.Span\x12\"\n\x05token\x18\x08 \x01(\x0b\x32\x13.clarifai.api.Token\x12/\n\x12keypoint_locations\x18\t \x03(\x0b\x32\x13.clarifai.api.PointJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"o\n\x0b\x42oundingBox\x12\x15\n\x07top_row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08left_col\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nbottom_row\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tright_col\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"4\n\tFrameInfo\x12\x13\n\x05index\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x12\n\x04time\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"b\n\x05\x46rame\x12+\n\nframe_info\x18\x01 \x01(\x0b\x32\x17.clarifai.api.FrameInfo\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12\n\n\x02id\x18\x03 \x01(\t\"0\n\x04Mask\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x01\x10\x02\".\n\x07Polygon\x12#\n\x06points\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Point\"\xb6\x01\n\x05Point\x12\x11\n\x03row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03\x63ol\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\t\n\x01z\x18\x03 \x01(\x02\x12\x32\n\nvisibility\x18\x04 \x01(\x0e\x32\x1e.clarifai.api.Point.Visibility\"H\n\nVisibility\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0f\n\x0bNOT_VISIBLE\x10\x02\x12\x0f\n\x0bNOT_PRESENT\x10\x03\"J\n\x04Span\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"K\n\x05Token\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"7\n\tEmbedding\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x10\x01\x12\x16\n\x0enum_dimensions\x18\x02 \x01(\r\";\n\x08GeoPoint\x12\x17\n\tlongitude\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08latitude\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\"-\n\x08GeoLimit\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x05value\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\":\n\rGeoBoxedPoint\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\"\x89\x01\n\x03Geo\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\x12)\n\tgeo_limit\x18\x02 \x01(\x0b\x32\x16.clarifai.api.GeoLimit\x12,\n\x07geo_box\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.GeoBoxedPoint\"\x9d\x01\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nimage_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.ImageInfoJ\x04\x08\x03\x10\x04\"N\n\tImageInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x12\n\ncolor_mode\x18\x04 \x01(\t\"O\n\tHostedURL\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\r\n\x05sizes\x18\x03 \x03(\t\x12\x13\n\x0b\x63rossorigin\x18\x04 \x01(\t\"\xde\x01\n\x05Input\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x61taset_ids\x18\x07 \x03(\tJ\x04\x08\x03\x10\x04\"1\n\nInputBatch\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\"\xda\x01\n\nInputCount\x12\x17\n\tprocessed\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_process\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x14\n\x06\x65rrors\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nprocessing\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\treindexed\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_reindex\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1c\n\x0ereindex_errors\x18\x07 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nreindexing\x18\x08 \x01(\rB\x04\x80\xb5\x18\x01\"\x92\x03\n\x07\x44\x61taset\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x41\n\x19\x64\x65\x66\x61ult_annotation_filter\x18\x0c \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\r\n\x05notes\x18\x0b \x01(\t\x12-\n\x07version\x18\r \x01(\x0b\x32\x1c.clarifai.api.DatasetVersionJ\x04\x08\x06\x10\x07J\x04\x08\n\x10\x0b\"\xd8\x01\n\x10\x41nnotationFilter\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12*\n\x0csaved_search\x18\x08 \x01(\x0b\x32\x14.clarifai.api.SearchJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"b\n\x0c\x44\x61tasetInput\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xe9\x05\n\x0e\x44\x61tasetVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x12\n\ndataset_id\x18\x06 \x01(\t\x12H\n\x18\x61nnotation_filter_config\x18\x0f \x01(\x0b\x32$.clarifai.api.AnnotationFilterConfigH\x00\x12@\n\x14model_predict_config\x18\x12 \x01(\x0b\x32 .clarifai.api.ModelPredictConfigH\x00\x12+\n\x06status\x18\x08 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12:\n\x07metrics\x18\x10 \x03(\x0b\x32).clarifai.api.DatasetVersion.MetricsEntry\x12;\n\x0b\x65xport_info\x18\x11 \x01(\x0b\x32&.clarifai.api.DatasetVersionExportInfo\x12)\n\x08metadata\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x1f\n\x17\x65mbed_model_version_ids\x18\x0e \x03(\t\x1aS\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics:\x02\x38\x01\x42\r\n\x0b\x64\x61ta_configJ\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0c\"p\n\x16\x41nnotationFilterConfig\x12\x39\n\x11\x61nnotation_filter\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x1b\n\x13ignore_empty_inputs\x18\x02 \x01(\x08\"8\n\x12ModelPredictConfig\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Model\"\xc3\x08\n\x15\x44\x61tasetVersionMetrics\x12\x32\n\x0cinputs_count\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12<\n\x16unlabeled_inputs_count\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1ainputs_with_metadata_count\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12;\n\x15inputs_with_geo_count\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x33\n\rregions_count\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12-\n\x16region_location_matrix\x18\x15 \x01(\x0b\x32\r.MatrixUint64\x12:\n\x14\x62ounding_boxes_count\x18\x16 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x34\n\x0epolygons_count\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0cpoints_count\x18\x18 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmasks_count\x18\x19 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_inputs_count\x18< \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_frames_count\x18= \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0c\x66rames_count\x18\x1e \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x12\x66rame_inputs_count\x18\x46 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x36\n\x10\x65mbeddings_count\x18( \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_input_tags_count\x18\x32 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1apositive_region_tags_count\x18\x33 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_frame_tags_count\x18\x34 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"\xca\x01\n\x1a\x44\x61tasetVersionMetricsGroup\x12\x13\n\x0bparent_path\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12%\n\x05value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x34\n\x07metrics\x18\x04 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics\"\xd0\x01\n\x18\x44\x61tasetVersionExportInfo\x12\x42\n\x16\x63larifai_data_protobuf\x18\x01 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12>\n\x12\x63larifai_data_json\x18\x03 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12\x30\n\x04\x63oco\x18\x02 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\"\xb4\x01\n\x14\x44\x61tasetVersionExport\x12\x38\n\x06\x66ormat\x18\x01 \x01(\x0e\x32(.clarifai.api.DatasetVersionExportFormat\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x04\x12\x1a\n\x12include_embeddings\x18\x05 \x01(\x08\"n\n\x19WorkflowResultsSimilarity\x12(\n\x0bprobe_input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12\'\n\x0cpool_results\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Hit\"\xf4\x01\n\x03Key\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x07 \x03(\t\x12\x1f\n\x04\x61pps\x18\x04 \x03(\x0b\x32\x11.clarifai.api.App\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61uthorized_idp_ids\x18\t \x03(\t\"\xd8\x07\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x04name\x18\x02 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x06\x61pp_id\x18\x04 \x01(\tB\x04\x80\xb5\x18\x01\x12\x31\n\x0boutput_info\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfoB\x02\x18\x01\x12\x31\n\rmodel_version\x18\x06 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x18\n\x0c\x64isplay_name\x18\x07 \x01(\tB\x02\x18\x01\x12\x0f\n\x07user_id\x18\t \x01(\t\x12/\n\ninput_info\x18\x0c \x01(\x0b\x32\x17.clarifai.api.InputInfoB\x02\x18\x01\x12/\n\ntrain_info\x18\r \x01(\x0b\x32\x17.clarifai.api.TrainInfoB\x02\x18\x01\x12\x31\n\x11\x64\x65\x66\x61ult_eval_info\x18\x1e \x01(\x0b\x32\x16.clarifai.api.EvalInfo\x12\x15\n\rmodel_type_id\x18\x0e \x01(\t\x12\x0c\n\x04task\x18\x1a \x01(\t\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\x12)\n\x08metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07presets\x18\x1b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05notes\x18\x12 \x01(\t\x12\x16\n\x08toolkits\x18\x14 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tuse_cases\x18\x15 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tlanguages\x18\x19 \x03(\tB\x04\x80\xb5\x18\x01\x12\x33\n\x0elanguages_full\x18\x1f \x03(\x0b\x32\x15.clarifai.api.FullTagB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18  \x03(\tB\x04\x80\xb5\x18\x01\x12\x12\n\nis_starred\x18\x16 \x01(\x08\x12\x12\n\nstar_count\x18\x17 \x01(\x05\x12\x31\n\x0bimport_info\x18\x18 \x01(\x0b\x32\x18.clarifai.api.ImportInfoB\x02\x18\x01\x12\x38\n\x14workflow_recommended\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.BoolValueJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x1c\x10\x1d\"t\n\x0eModelReference\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x97\x01\n\x18ModelVersionInputExample\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"\xd4\x01\n\nOutputInfo\x12 \n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x31\n\routput_config\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12\x0f\n\x07message\x18\x03 \x01(\t\x12+\n\nfields_map\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"a\n\tInputInfo\x12+\n\nfields_map\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"4\n\tTrainInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"3\n\x08\x45valInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"5\n\nImportInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x81\x04\n\x0cOutputConfig\x12\'\n\x1b\x63oncepts_mutually_exclusive\x18\x01 \x01(\x08\x42\x02\x18\x01\x12 \n\x12\x63losed_environment\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x1d\n\x11\x65xisting_model_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x1c\n\x10hyper_parameters\x18\x05 \x01(\tB\x02\x18\x01\x12\x1a\n\x0cmax_concepts\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\tmin_value\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12.\n\x0fselect_concepts\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x18\n\x10training_timeout\x18\t \x01(\r\x12\x11\n\tsample_ms\x18\n \x01(\r\x12-\n\x0chyper_params\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x16\x65mbed_model_version_id\x18\x0e \x01(\t\x12)\n!fail_on_missing_positive_examples\x18\x0f \x01(\x08\x12\x33\n\x0emodel_metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x10\x10\x11J\x04\x08\x12\x10\x13\"\xd2\x03\n\tModelType\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cinput_fields\x18\x05 \x03(\t\x12\x15\n\routput_fields\x18\x06 \x03(\t\x12\x11\n\ttrainable\x18\x08 \x01(\x08\x12\x11\n\tcreatable\x18\t \x01(\x08\x12\x15\n\rinternal_only\x18\n \x01(\x08\x12\x37\n\x11model_type_fields\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\"\n\x1arequires_sequential_frames\x18\x0c \x01(\x08\x12;\n\x15\x65xpected_input_layers\x18\x10 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12<\n\x16\x65xpected_output_layers\x18\x11 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12\x35\n\x0f\x65valuation_type\x18\x12 \x01(\x0e\x32\x1c.clarifai.api.EvaluationTypeJ\x04\x08\x07\x10\x08J\x04\x08\x04\x10\x05J\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10\"\x89\x01\n\x0eModelLayerInfo\x12\x17\n\x0f\x64\x61ta_field_name\x18\x01 \x01(\t\x12(\n\x06shapes\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LayerShape\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1f\n\x17requires_label_filename\x18\x04 \x01(\x08\"D\n\x12TritonCondaEnvInfo\x12\x16\n\x0e\x63onda_pack_url\x18\x01 \x01(\t\x12\x16\n\x0e\x63onda_yaml_url\x18\x02 \x01(\t\"l\n\nLayerShape\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x10\n\x08max_dims\x18\x02 \x03(\x05\x12)\n\tdata_type\x18\x03 \x01(\x0e\x32\x16.clarifai.api.DataType\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xd2\x05\n\x0eModelTypeField\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x43\n\nfield_type\x18\x02 \x01(\x0e\x32/.clarifai.api.ModelTypeField.ModelTypeFieldType\x12-\n\rdefault_value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0bplaceholder\x18\x05 \x01(\t\x12\x42\n\x17model_type_enum_options\x18\x06 \x03(\x0b\x32!.clarifai.api.ModelTypeEnumOption\x12\x15\n\rinternal_only\x18\x07 \x01(\x08\x12\x10\n\x08required\x18\x08 \x01(\x08\x12?\n\x15model_type_range_info\x18\t \x01(\x0b\x32 .clarifai.api.ModelTypeRangeInfo\"\xe5\x02\n\x12ModelTypeFieldType\x12!\n\x1dINVALID_MODEL_TYPE_FIELD_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\n\n\x06NUMBER\x10\x03\x12\x15\n\x11\x41RRAY_OF_CONCEPTS\x10\x04\x12$\n ARRAY_OF_CONCEPTS_WITH_THRESHOLD\x10\x05\x12\t\n\x05RANGE\x10\x07\x12\x08\n\x04\x45NUM\x10\x08\x12\x11\n\rCOLLABORATORS\x10\t\x12\x08\n\x04JSON\x10\n\x12\x14\n\x10\x41RRAY_OF_NUMBERS\x10\x0b\x12\x19\n\x15WORKFLOW_EMBED_MODELS\x10\x0c\x12\x14\n\x10\x41RRAY_OF_STRINGS\x10\r\x12\x12\n\x0eRECURSIVE_ENUM\x10\x0e\x12\x0f\n\x0bPYTHON_CODE\x10\x0f\x12\x0e\n\nDATASET_ID\x10\x10\x12\x16\n\x12\x44\x41TASET_VERSION_ID\x10\x11\"\x04\x08\x06\x10\x06\"<\n\x12ModelTypeRangeInfo\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03max\x18\x02 \x01(\x02\x12\x0c\n\x04step\x18\x03 \x01(\x02\"\xd4\x01\n\x13ModelTypeEnumOption\x12\n\n\x02id\x18\x01 \x01(\t\x12\x37\n\x07\x61liases\x18\x05 \x03(\x0b\x32&.clarifai.api.ModelTypeEnumOptionAlias\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x37\n\x11model_type_fields\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\x15\n\rinternal_only\x18\x04 \x01(\x08\x12\x13\n\x0brecommended\x18\x06 \x01(\x08\"C\n\x18ModelTypeEnumOptionAlias\x12\x0e\n\x06id_int\x18\x01 \x01(\x03\x12\x17\n\x0fwildcard_string\x18\x02 \x01(\t\"7\n\nModelQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rmodel_type_id\x18\x03 \x01(\tJ\x04\x08\x02\x10\x03\"\xfc\x05\n\x0cModelVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x04 \x01(\r\x12*\n\x07metrics\x18\x05 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12\x19\n\x11total_input_count\x18\x06 \x01(\r\x12\x44\n\x17pretrained_model_config\x18\x07 \x01(\x0b\x32#.clarifai.api.PretrainedModelConfig\x12\x30\n\x0c\x63ompleted_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\r \x01(\t\x12\x0f\n\x07user_id\x18\x0e \x01(\t\x12/\n\x0bmodified_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07license\x18\x11 \x01(\t\x12-\n\x0boutput_info\x18\x13 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\x12+\n\ninput_info\x18\x14 \x01(\x0b\x32\x17.clarifai.api.InputInfo\x12+\n\ntrain_info\x18\x15 \x01(\x0b\x32\x17.clarifai.api.TrainInfo\x12-\n\x0bimport_info\x18\x16 \x01(\x0b\x32\x18.clarifai.api.ImportInfo\x12\x11\n\ttrain_log\x18\x17 \x01(\tJ\x04\x08\t\x10\nJ\x04\x08\x12\x10\x13\"\xa1\x01\n\x15PretrainedModelConfig\x12\x31\n\x10input_fields_map\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x11output_fields_map\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rmodel_zip_url\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06\">\n\nTrainStats\x12\x30\n\nloss_curve\x18\x01 \x03(\x0b\x32\x1c.clarifai.api.LossCurveEntry\"B\n\x0eLossCurveEntry\x12\r\n\x05\x65poch\x18\x01 \x01(\r\x12\x13\n\x0bglobal_step\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\x02\"1\n\nLabelCount\x12\x14\n\x0c\x63oncept_name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"L\n\x11LabelDistribution\x12\x37\n\x15positive_label_counts\x18\x01 \x03(\x0b\x32\x18.clarifai.api.LabelCount\"B\n\x17\x43ooccurrenceMatrixEntry\x12\x0b\n\x03row\x18\x01 \x01(\t\x12\x0b\n\x03\x63ol\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"`\n\x12\x43ooccurrenceMatrix\x12\x35\n\x06matrix\x18\x01 \x03(\x0b\x32%.clarifai.api.CooccurrenceMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"N\n\x14\x43onfusionMatrixEntry\x12\x11\n\tpredicted\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x02 \x01(\t\x12\x13\n\x05value\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"Z\n\x0f\x43onfusionMatrix\x12\x32\n\x06matrix\x18\x01 \x03(\x0b\x32\".clarifai.api.ConfusionMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"t\n\x03ROC\x12\x11\n\x03\x66pr\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03tpr\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x15\n\rfpr_per_image\x18\x04 \x03(\x02\x12\x16\n\x0e\x66pr_per_object\x18\x05 \x03(\x02\"_\n\x14PrecisionRecallCurve\x12\x14\n\x06recall\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tprecision\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\"\xea\x02\n\rBinaryMetrics\x12\x15\n\x07num_pos\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_neg\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_tot\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x10\n\x02\x66\x31\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12&\n\x07\x63oncept\x18\x06 \x01(\x0b\x32\x15.clarifai.api.Concept\x12$\n\troc_curve\x18\x07 \x01(\x0b\x32\x11.clarifai.api.ROC\x12\x42\n\x16precision_recall_curve\x18\x08 \x01(\x0b\x32\".clarifai.api.PrecisionRecallCurve\x12\x15\n\ravg_precision\x18\t \x01(\x02\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x10\n\x08\x61rea_min\x18\x0b \x01(\x01\x12\x10\n\x08\x61rea_max\x18\x0c \x01(\x01\x12\x0b\n\x03iou\x18\r \x01(\x02\"\x91\x01\n\x0eTrackerMetrics\x12\x10\n\x08mot_mota\x18\x01 \x01(\x02\x12\x18\n\x10mot_num_switches\x18\x02 \x01(\x05\x12\x12\n\nmorse_frag\x18\x03 \x01(\x02\x12\x15\n\ravg_precision\x18\x04 \x01(\x02\x12\x0c\n\x04\x61iid\x18\x05 \x01(\t\x12\x1a\n\x12unique_switch_rate\x18\x06 \x01(\x02\"\xee\x01\n\x10\x45valTestSetEntry\x12\x0e\n\x02id\x18\x01 \x01(\tB\x02\x18\x01\x12\x0f\n\x03url\x18\x02 \x01(\tB\x02\x18\x01\x12\"\n\x05input\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\x12predicted_concepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x34\n\x15ground_truth_concepts\x18\x04 \x03(\x0b\x32\x15.clarifai.api.Concept\x12,\n\nannotation\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\xcd\x01\n\x0eLOPQEvalResult\x12\t\n\x01k\x18\x01 \x01(\x05\x12#\n\x15recall_vs_brute_force\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1akendall_tau_vs_brute_force\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1amost_frequent_code_percent\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tlopq_ndcg\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10\x62rute_force_ndcg\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\"\x8c\x03\n\x0eMetricsSummary\x12\x19\n\rtop1_accuracy\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rtop5_accuracy\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x1f\n\x11macro_avg_roc_auc\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1f\n\x11macro_std_roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_avg_f1_score\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_std_f1_score\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x13macro_avg_precision\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10macro_avg_recall\x18\x08 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x19mean_avg_precision_iou_50\x18\n \x01(\x02\x12$\n\x1cmean_avg_precision_iou_range\x18\x0b \x01(\x02\x12\x32\n\x0clopq_metrics\x18\t \x03(\x0b\x32\x1c.clarifai.api.LOPQEvalResult\"\xda\x04\n\x0b\x45valMetrics\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\n \x01(\t\x12-\n\x07summary\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.MetricsSummary\x12\x37\n\x10\x63onfusion_matrix\x18\x03 \x01(\x0b\x32\x1d.clarifai.api.ConfusionMatrix\x12=\n\x13\x63ooccurrence_matrix\x18\x04 \x01(\x0b\x32 .clarifai.api.CooccurrenceMatrix\x12\x35\n\x0clabel_counts\x18\x05 \x01(\x0b\x32\x1f.clarifai.api.LabelDistribution\x12\x33\n\x0e\x62inary_metrics\x18\x06 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x30\n\x08test_set\x18\x07 \x03(\x0b\x32\x1e.clarifai.api.EvalTestSetEntry\x12\x34\n\x0fmetrics_by_area\x18\x08 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x10metrics_by_class\x18\t \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x0ftracker_metrics\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.TrackerMetrics\x12)\n\teval_info\x18\x0c \x01(\x0b\x32\x16.clarifai.api.EvalInfo\"\xb7\x01\n\x0b\x46ieldsValue\x12\x18\n\x10\x63onfusion_matrix\x18\x01 \x01(\x08\x12\x1b\n\x13\x63ooccurrence_matrix\x18\x02 \x01(\x08\x12\x14\n\x0clabel_counts\x18\x03 \x01(\x08\x12\x16\n\x0e\x62inary_metrics\x18\x04 \x01(\x08\x12\x10\n\x08test_set\x18\x05 \x01(\x08\x12\x17\n\x0fmetrics_by_area\x18\x06 \x01(\x08\x12\x18\n\x10metrics_by_class\x18\x07 \x01(\x08\"\xdb\x01\n\x06Output\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12 \n\x04\x64\x61ta\x18\x06 \x01(\x0b\x32\x12.clarifai.api.Data\"4\n\tScopeDeps\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\":\n\x0c\x45ndpointDeps\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\"\x8d\x01\n\x03Hit\x12\x13\n\x05score\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\x12,\n\nannotation\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\"\x8d\x01\n\x03\x41nd\x12\"\n\x05input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12$\n\x06output\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Output\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x88\x01\n\x05Query\x12#\n\x04\x61nds\x18\x01 \x03(\x0b\x32\x11.clarifai.api.AndB\x02\x18\x01\x12\x10\n\x08language\x18\x02 \x01(\t\x12%\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Filter\x12!\n\x05ranks\x18\x04 \x03(\x0b\x32\x12.clarifai.api.Rank\"\xd6\x03\n\x06Search\x12\"\n\x05query\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Query\x12\n\n\x02id\x18\x02 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x05\x61s_of\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08git_hash\x18\x06 \x01(\t\x12.\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\talgorithm\x18\t \x01(\t\x12\x0c\n\x04save\x18\n \x01(\x08\x12\x11\n\tmin_value\x18\x0b \x01(\x02\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12+\n\x06metric\x18\r \x01(\x0e\x32\x1b.clarifai.api.Search.Metric\"I\n\x06Metric\x12\x12\n\x0eMETRIC_NOT_SET\x10\x00\x12\x16\n\x12\x45UCLIDEAN_DISTANCE\x10\x01\x12\x13\n\x0f\x43OSINE_DISTANCE\x10\x02\"\xa4\x01\n\x06\x46ilter\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x38\n\x17last_updated_time_range\x18\x06 \x01(\x0b\x32\x17.clarifai.api.TimeRange\"i\n\tTimeRange\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x04Rank\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x8d\x02\n\x17\x41nnotationSearchMetrics\x12*\n\x0cground_truth\x18\x01 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Search\x12*\n\x07metrics\x18\x03 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x05 \x01(\r\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"\x91\x01\n\x04Text\x12\x0b\n\x03raw\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x1b\n\x13\x61llow_duplicate_url\x18\x03 \x01(\x08\x12\'\n\x06hosted\x18\x04 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12)\n\ttext_info\x18\x05 \x01(\x0b\x32\x16.clarifai.api.TextInfo\"0\n\x08TextInfo\x12\x12\n\nchar_count\x18\x01 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x02 \x01(\t\"\xfc\x05\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\rprimary_email\x18\x02 \x01(\tB\x02\x18\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x14\n\x0c\x63ompany_name\x18\x05 \x01(\t\x12\x11\n\tjob_title\x18\x13 \x01(\t\x12\x10\n\x08job_role\x18\x14 \x01(\t\x12\x15\n\tbill_type\x18\x07 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x11\x64\x61te_gdpr_consent\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_tos_consent\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12>\n\x16\x64\x61te_marketing_consent\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_pii_consent\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12-\n\x08metadata\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x37\n\x0f\x65mail_addresses\x18\x0c \x03(\x0b\x32\x1a.clarifai.api.EmailAddressB\x02\x18\x01\x12#\n\x17two_factor_auth_enabled\x18\x0f \x01(\x08\x42\x02\x18\x01\x12\x17\n\x0bteams_count\x18\x10 \x01(\rB\x02\x18\x01\x12\x12\n\nis_starred\x18\x15 \x01(\x08\x12\x12\n\nstar_count\x18\x16 \x01(\x05\x12,\n\nvisibility\x18\x11 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12-\n\x0buser_detail\x18\x12 \x01(\x0b\x32\x18.clarifai.api.UserDetailJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\xd1\x03\n\nUserDetail\x12\x15\n\rprimary_email\x18\x01 \x01(\t\x12\x11\n\tbill_type\x18\x02 \x01(\t\x12\x35\n\x11\x64\x61te_gdpr_consent\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_tos_consent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x64\x61te_marketing_consent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_pii_consent\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x33\n\x0f\x65mail_addresses\x18\x07 \x03(\x0b\x32\x1a.clarifai.api.EmailAddress\x12\x1f\n\x17two_factor_auth_enabled\x18\t \x01(\x08\x12\x13\n\x0bteams_count\x18\n \x01(\r\x12\x0f\n\x07\x63ountry\x18\x0b \x01(\t\x12\r\n\x05state\x18\x0c \x01(\tJ\x04\x08\x08\x10\t\"R\n\x0c\x45mailAddress\x12\x13\n\x05\x65mail\x18\x01 \x01(\tB\x04\x80\xb5\x18\x01\x12\x15\n\x07primary\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08verified\x18\x03 \x01(\x08\x42\x04\x80\xb5\x18\x01\"\x1d\n\x08Password\x12\x11\n\tplaintext\x18\x01 \x01(\t\"\x86\x03\n\x12PasswordViolations\x12\x16\n\x0eminimum_length\x18\x01 \x01(\x08\x12\x16\n\x0emaximum_length\x18\x02 \x01(\x08\x12\x19\n\x11upper_case_needed\x18\x03 \x01(\x08\x12\x19\n\x11lower_case_needed\x18\x04 \x01(\x08\x12\x16\n\x0enumeric_needed\x18\x05 \x01(\x08\x12\x1f\n\x17non_alphanumeric_needed\x18\x06 \x01(\x08\x12\x16\n\x0epassword_reuse\x18\x07 \x01(\x08\x12\x15\n\rexclude_names\x18\x08 \x01(\x08\x12\x15\n\rexclude_email\x18\t \x01(\x08\x12\x1c\n\x14no_confusing_letters\x18\n \x01(\x08\x12\x1b\n\x13no_simple_passwords\x18\x0b \x01(\x08\x12\x18\n\x10no_common_vocabs\x18\x0c \x01(\x08\x12\x1b\n\x13no_overlap_with_old\x18\r \x01(\x08\x12\x19\n\x11password_lifespan\x18\x0e \x01(\x08\"\xae\x01\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\x15\n\rthumbnail_url\x18\x05 \x01(\t\x12\'\n\x06hosted\x18\x06 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nvideo_info\x18\x07 \x01(\x0b\x32\x17.clarifai.api.VideoInfo\"\x8e\x01\n\tVideoInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0b\n\x03\x66ps\x18\x03 \x01(\x02\x12\x14\n\x0cvideo_format\x18\x04 \x01(\t\x12\x10\n\x08\x62it_rate\x18\x05 \x01(\x05\x12\x13\n\x0b\x66rame_count\x18\x06 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x07 \x01(\x02\"\xcf\x03\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x05nodes\x18\x04 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\x07 \x01(\t\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x07version\x18\t \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x12\n\nis_starred\x18\n \x01(\x08\x12\x12\n\nstar_count\x18\x0b \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\r\n\x05notes\x18\r \x01(\t\x12\x17\n\tuse_cases\x18\x0e \x03(\tB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18\x0f \x03(\tB\x04\x80\xb5\x18\x01\"\xde\x02\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x05nodes\x18\x06 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06\x61pp_id\x18\x08 \x01(\t\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07license\x18\x0b \x01(\t\"\xbd\x01\n\x0cWorkflowNode\x12\n\n\x02id\x18\x01 \x01(\t\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\x12,\n\x0bnode_inputs\x18\x03 \x03(\x0b\x32\x17.clarifai.api.NodeInput\x12\x17\n\x0fsuppress_output\x18\x04 \x01(\x08\x12\x36\n\x14output_info_override\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\"\x1c\n\tNodeInput\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x02\n\x0eWorkflowResult\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12%\n\x07outputs\x18\x06 \x03(\x0b\x32\x14.clarifai.api.Output\x12\x17\n\x0fsuppress_output\x18\x07 \x01(\x08\"\x1b\n\rWorkflowState\x12\n\n\x02id\x18\x01 \x01(\t\"\xd8\x02\n\x0e\x41ppDuplication\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nnew_app_id\x18\x02 \x01(\t\x12\x14\n\x0cnew_app_name\x18\x03 \x01(\t\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x66ilter\x18\x07 \x01(\x0b\x32#.clarifai.api.AppDuplicationFilters\x12\x17\n\x0f\x65xisting_app_id\x18\x08 \x01(\t\x12/\n\x08progress\x18\t \x03(\x0b\x32\x1d.clarifai.api.AppCopyProgress\"/\n\x0f\x41ppCopyProgress\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05\"\x8a\x01\n\x15\x41ppDuplicationFilters\x12\x13\n\x0b\x63opy_inputs\x18\x01 \x01(\x08\x12\x15\n\rcopy_concepts\x18\x02 \x01(\x08\x12\x18\n\x10\x63opy_annotations\x18\x03 \x01(\x08\x12\x13\n\x0b\x63opy_models\x18\x04 \x01(\x08\x12\x16\n\x0e\x63opy_workflows\x18\x05 \x01(\x08\"\xfa\x02\n\nLabelOrder\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x61uto_release\x18\x04 \x01(\x08\x12\x17\n\x0f\x61llow_empty_tag\x18\x05 \x01(\x08\x12\x38\n\x14\x64\x65sired_fulfill_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15\x65stimate_fulfill_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x04task\x18\x08 \x01(\x0b\x32\x12.clarifai.api.Task\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xe5\x05\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.clarifai.api.Task.TaskType\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12(\n\x06worker\x18\x06 \x01(\x0b\x32\x18.clarifai.api.TaskWorker\x12\x13\n\x0b\x63oncept_ids\x18\x07 \x03(\t\x12\x33\n\x0cinput_source\x18\x08 \x01(\x0b\x32\x1d.clarifai.api.TaskInputSource\x12\x11\n\tsample_ms\x18\t \x01(\r\x12\x33\n\x0c\x61i_assistant\x18\n \x01(\x0b\x32\x1d.clarifai.api.TaskAIAssistant\x12(\n\x06review\x18\x0b \x01(\x0b\x32\x18.clarifai.api.TaskReview\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0c\n\x04name\x18\r \x01(\t\x12:\n\x10\x61i_assist_params\x18\x0e \x01(\x0b\x32 .clarifai.api.AiAssistParameters\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\x0f\n\x07user_id\x18\x11 \x01(\t\x12\x16\n\x0elabel_order_id\x18\x12 \x01(\t\"l\n\x08TaskType\x12\x10\n\x0cTYPE_NOT_SET\x10\x00\x12\x1b\n\x17\x43ONCEPTS_CLASSIFICATION\x10\x01\x12\x1a\n\x16\x42OUNDING_BOX_DETECTION\x10\x02\x12\x15\n\x11POLYGON_DETECTION\x10\x03\"`\n\x12\x41iAssistParameters\x12\x15\n\rmin_threshold\x18\x01 \x01(\x02\x12\x15\n\rmax_threshold\x18\x02 \x01(\x02\x12\x1c\n\x14\x63oncept_relation_ids\x18\x03 \x03(\t\"\xbf\x02\n\nTaskWorker\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskWorker.TaskWorkerStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x04 \x03(\x0b\x32\x12.clarifai.api.User\x12T\n\x19partitioned_strategy_info\x18\x03 \x01(\x0b\x32/.clarifai.api.TaskWorkerPartitionedStrategyInfoH\x00\"R\n\x12TaskWorkerStrategy\x12\x1b\n\x17WORKER_STRATEGY_NOT_SET\x10\x00\x12\x0f\n\x0bPARTITIONED\x10\x02\x12\x08\n\x04\x46ULL\x10\x03\"\x04\x08\x01\x10\x01\x42\x0f\n\rstrategy_info\"\xa9\x02\n!TaskWorkerPartitionedStrategyInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.clarifai.api.TaskWorkerPartitionedStrategyInfo.TaskWorkerPartitionedStrategy\x12\x19\n\x11workers_per_input\x18\x02 \x01(\x05\x12(\n\x07weights\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"b\n\x1dTaskWorkerPartitionedStrategy\x12\'\n#PARTITIONED_WORKER_STRATEGY_NOT_SET\x10\x00\x12\n\n\x06\x45VENLY\x10\x01\x12\x0c\n\x08WEIGHTED\x10\x02\"\xc3\x01\n\x0fTaskInputSource\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.clarifai.api.TaskInputSource.TaskInputSourceType\x12\n\n\x02id\x18\x02 \x01(\t\"c\n\x13TaskInputSourceType\x12\x1d\n\x19INPUT_SOURCE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nALL_INPUTS\x10\x01\x12\x10\n\x0cSAVED_SEARCH\x10\x02\x12\x0b\n\x07\x44\x41TASET\x10\x03\"\x90\x03\n\nTaskReview\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskReview.TaskReviewStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x05 \x03(\x0b\x32\x12.clarifai.api.User\x12J\n\x14manual_strategy_info\x18\x03 \x01(\x0b\x32*.clarifai.api.TaskReviewManualStrategyInfoH\x00\x12P\n\x17\x63onsensus_strategy_info\x18\x04 \x01(\x0b\x32-.clarifai.api.TaskReviewConsensusStrategyInfoH\x00\"[\n\x12TaskReviewStrategy\x12 \n\x1cTASK_REVIEW_STRATEGY_NOT_SET\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06MANUAL\x10\x02\x12\r\n\tCONSENSUS\x10\x03\x42\x0f\n\rstrategy_info\"9\n\x1cTaskReviewManualStrategyInfo\x12\x19\n\x11sample_percentage\x18\x01 \x01(\x02\"C\n\x1fTaskReviewConsensusStrategyInfo\x12\x1a\n\x12\x61pproval_threshold\x18\x02 \x01(\rJ\x04\x08\x01\x10\x02\"&\n\x0fTaskAIAssistant\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"\xbc\x01\n\x16TaskStatusCountPerUser\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x15\n\x07pending\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1d\n\x0f\x61waiting_review\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07success\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1b\n\rreview_denied\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\'\n\x19\x61waiting_consensus_review\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\"\x81\x02\n\tCollector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1d\n\x15pre_queue_workflow_id\x18\x04 \x01(\t\x12\x1e\n\x16post_queue_workflow_id\x18\x05 \x01(\t\x12\x37\n\x10\x63ollector_source\x18\x06 \x01(\x0b\x32\x1d.clarifai.api.CollectorSource\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"t\n\x0f\x43ollectorSource\x12\x61\n\'api_post_model_outputs_collector_source\x18\x02 \x01(\x0b\x32\x30.clarifai.api.APIPostModelOutputsCollectorSource\"\x99\x01\n\"APIPostModelOutputsCollectorSource\x12\x15\n\rmodel_user_id\x18\x01 \x01(\t\x12\x14\n\x0cmodel_app_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x18\n\x10model_version_id\x18\x04 \x01(\t\x12\x1a\n\x12post_inputs_key_id\x18\x05 \x01(\t\"R\n\tStatValue\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04tags\x18\x03 \x03(\t\"\xa6\x01\n\x18StatValueAggregateResult\x12?\n\x15stat_value_aggregates\x18\x01 \x03(\x0b\x32 .clarifai.api.StatValueAggregate\x12I\n\x1astat_value_aggregate_query\x18\x02 \x01(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"t\n\x12StatValueAggregate\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x61ggregate_value\x18\x02 \x01(\x02\x12\r\n\x05\x63ount\x18\x03 \x01(\x04\x12\x0c\n\x04tags\x18\x04 \x03(\t\"\x91\x02\n\x17StatValueAggregateQuery\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x12\n\ntag_groups\x18\x02 \x03(\t\x12;\n\x13stat_value_agg_type\x18\x03 \x01(\x0e\x32\x1e.clarifai.api.StatValueAggType\x12\x39\n\x12stat_time_agg_type\x18\x04 \x01(\x0e\x32\x1d.clarifai.api.StatTimeAggType\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xef\x01\n\x19\x44\x61tasetInputsSearchAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x12\n\ndataset_id\x18\x05 \x01(\t\x12$\n\x06search\x18\x06 \x01(\x0b\x32\x14.clarifai.api.Search\"O\n\x17PCAProjectionComparator\x12\x1a\n\x12\x64istance_threshold\x18\x01 \x01(\x02\x12\x18\n\x10model_version_id\x18\x02 \x01(\t\"K\n\x1b\x44uplicateAnnotationsResults\x12\x16\n\x0e\x64uplicate_cfid\x18\x01 \x03(\t\x12\x14\n\x0cunique_count\x18\x02 \x01(\x05\"\x87\x01\n\nVisibility\x12\x33\n\x08gettable\x18\x01 \x01(\x0e\x32!.clarifai.api.Visibility.Gettable\"D\n\x08Gettable\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\x0b\n\x07PRIVATE\x10\n\x12\x07\n\x03ORG\x10\x1e\x12\n\n\x06PUBLIC\x10\x32\"X\n\x0eTrendingMetric\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\x12\x12\n\nview_count\x18\x04 \x01(\x04\"#\n\x07\x46ullTag\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x0bTimeSegment\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x03 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\"D\n\x08TimeInfo\x12\x12\n\nnum_frames\x18\x01 \x01(\r\x12\x12\n\nbegin_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\"\xbf\x02\n\x06Module\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x07 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x0e\n\x06\x61pp_id\x18\n \x01(\t\x12\x33\n\x0emodule_version\x18\x0b \x01(\x0b\x32\x1b.clarifai.api.ModuleVersionJ\x04\x08\x02\x10\x03\"\xbe\x04\n\rModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\r\n\x05notes\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0egit_commit_url\x18\n \x01(\t\x12\x39\n\nmodule_nav\x18\x0b \x01(\x0b\x32%.clarifai.api.ModuleVersion.ModuleNav\x12\x10\n\x08\x61pproved\x18\x0c \x01(\x08\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x1a\x45\n\x0cModuleSubNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x11\n\tquery_key\x18\x02 \x01(\t\x12\x13\n\x0bquery_value\x18\x03 \x01(\t\x1a]\n\tModuleNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x41\n\x0fmodule_sub_navs\x18\x02 \x03(\x0b\x32(.clarifai.api.ModuleVersion.ModuleSubNavJ\x04\x08\x05\x10\x06\"\xad\x02\n\x16InstalledModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeploy_url\x18\x07 \x01(\t\x12,\n\nvisibility\x18\x08 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06key_id\x18\t \x01(\t\"\x8d\x03\n\rBulkOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\tinput_ids\x18\x02 \x01(\x0b\x32\x16.clarifai.api.InputIDsH\x00\x12&\n\x06search\x18\n \x01(\x0b\x32\x14.clarifai.api.SearchH\x00\x12*\n\toperation\x18\x03 \x01(\x0b\x32\x17.clarifai.api.Operation\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08progress\x18\x06 \x01(\x0b\x32\x16.clarifai.api.Progress\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x0e\n\x0cinput_source\"\x1d\n\x08InputIDs\x12\x11\n\tinput_ids\x18\x01 \x03(\t\"8\n\x08Progress\x12\x11\n\tprocessed\x18\x01 \x01(\r\x12\x19\n\x11last_processed_id\x18\x02 \x01(\t\"\x94\x03\n\tOperation\x12\x31\n\x0c\x61\x64\x64_concepts\x18\x01 \x01(\x0b\x32\x19.clarifai.api.AddConceptsH\x00\x12\x37\n\x0f\x64\x65lete_concepts\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DeleteConceptsH\x00\x12\x31\n\x0c\x61\x64\x64_metadata\x18\x03 \x01(\x0b\x32\x19.clarifai.api.AddMetadataH\x00\x12\x37\n\x0f\x64\x65lete_metadata\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.DeleteMetadataH\x00\x12\x33\n\roverwrite_geo\x18\x05 \x01(\x0b\x32\x1a.clarifai.api.OverwriteGeoH\x00\x12-\n\ndelete_geo\x18\x06 \x01(\x0b\x32\x17.clarifai.api.DeleteGeoH\x00\x12>\n\x13\x64\x65lete_from_dataset\x18\x07 \x01(\x0b\x32\x1f.clarifai.api.DeleteFromDatasetH\x00\x42\x0b\n\toperation\"6\n\x0b\x41\x64\x64\x43oncepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\"K\n\x0e\x44\x65leteConcepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x10\n\x08user_ids\x18\x02 \x03(\t\"8\n\x0b\x41\x64\x64Metadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\";\n\x0e\x44\x65leteMetadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\".\n\x0cOverwriteGeo\x12\x1e\n\x03geo\x18\x01 \x01(\x0b\x32\x11.clarifai.api.Geo\"\x0b\n\tDeleteGeo\"\'\n\x11\x44\x65leteFromDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\xce\x02\n\x0cInputsAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\x12\x34\n\x08progress\x18\x07 \x01(\x0b\x32\".clarifai.api.InputsAddJobProgress\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x0f\x65xtraction_jobs\x18\n \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\x12%\n\x07uploads\x18\x0b \x03(\x0b\x32\x14.clarifai.api.UploadJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"u\n\x14InputsAddJobProgress\x12\x15\n\rpending_count\x18\x01 \x01(\x04\x12\x19\n\x11in_progress_count\x18\x02 \x01(\x04\x12\x15\n\rsuccess_count\x18\x03 \x01(\x04\x12\x14\n\x0c\x66\x61iled_count\x18\x04 \x01(\x04\"\x95\x02\n\x06Upload\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x63ontent_name\x18\x08 \x01(\t\x12\x16\n\x0e\x63ontent_length\x18\x06 \x01(\x04\x12\x13\n\x0b\x63ontent_url\x18\x07 \x01(\t\"K\n\x11UploadContentPart\x12\x13\n\x0brange_start\x18\x01 \x01(\x04\x12\x13\n\x0bpart_number\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"l\n\x19\x43ustomCodeOperatorRequest\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\x12*\n\x08metadata\x18\xea\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xf9\x01\n\x13InputsExtractionJob\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12;\n\x08progress\x18\x04 \x01(\x0b\x32).clarifai.api.InputsExtractionJobProgress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa8\x01\n\x1bInputsExtractionJobProgress\x12\x1a\n\x12read_objects_count\x18\x01 \x01(\x04\x12\x1a\n\x12\x61udio_inputs_count\x18\x02 \x01(\x04\x12\x1a\n\x12image_inputs_count\x18\x03 \x01(\x04\x12\x1a\n\x12video_inputs_count\x18\x04 \x01(\x04\x12\x19\n\x11text_inputs_count\x18\x05 \x01(\x04\"W\n\x10InputsDataSource\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12(\n\x03url\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.DataSourceURL\"V\n\rDataSourceURL\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x38\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32#.clarifai.api.DataSourceCredentials\"\xa7\x01\n\x15\x44\x61taSourceCredentials\x12*\n\x08s3_creds\x18\x01 \x01(\x0b\x32\x16.clarifai.api.AWSCredsH\x00\x12\x13\n\tgcp_creds\x18\x02 \x01(\x0cH\x00\x12\x38\n\x10\x61zure_blob_creds\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.AzureBlobCredsH\x00\x42\r\n\x0b\x63redentialsJ\x04\x08\x03\x10\x04\"K\n\x08\x41WSCreds\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0e\n\x06secret\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\tJ\x04\x08\x01\x10\x02\";\n\x0e\x41zureBlobCreds\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\"`\n\x0cInputsUpload\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x02 \x01(\t\x12$\n\x06upload\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Upload*\xf9\x01\n\x1e\x44\x61tasetVersionMetricsGroupType\x12.\n*DATASET_VERSION_METRICS_GROUP_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_TYPE\x10\x02\x12\x0e\n\nCONCEPT_ID\x10\n\x12\x12\n\x0e\x43ONCEPTS_COUNT\x10\x0b\x12\x18\n\x14\x42OUNDING_BOXES_COUNT\x10\x14\x12\x12\n\x0ePOLYGONS_COUNT\x10\x15\x12\x10\n\x0cPOINTS_COUNT\x10\x16\x12\x0f\n\x0bMASKS_COUNT\x10\x17\x12\x10\n\x0cPIXELS_COUNT\x10\x1e\x12\x10\n\x0c\x41SPECT_RATIO\x10\x1f*\x85\x01\n\x1a\x44\x61tasetVersionExportFormat\x12)\n%DATASET_VERSION_EXPORT_FORMAT_NOT_SET\x10\x00\x12\x1a\n\x16\x43LARIFAI_DATA_PROTOBUF\x10\x01\x12\x16\n\x12\x43LARIFAI_DATA_JSON\x10\x03\x12\x08\n\x04\x43OCO\x10\x02*H\n\x10\x45xpirationAction\x12\x1d\n\x19\x45XPIRATION_ACTION_NOT_SET\x10\x00\x12\t\n\x05\x44\x45LAY\x10\x01\x12\n\n\x06\x45XPIRY\x10\x02*M\n\x0cLicenseScope\x12\x19\n\x15LICENSE_SCOPE_NOT_SET\x10\x00\x12\x0b\n\x07PREDICT\x10\x01\x12\t\n\x05TRAIN\x10\x02\x12\n\n\x06SEARCH\x10\x03*P\n\x08\x44\x61taType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\t\n\x05UINT8\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04\x46P32\x10\x05*\x8f\x01\n\x0fValueComparator\x12\x1d\n\x19\x43ONCEPT_THRESHOLD_NOT_SET\x10\x00\x12\x10\n\x0cGREATER_THAN\x10\x01\x12\x19\n\x15GREATER_THAN_OR_EQUAL\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x16\n\x12LESS_THAN_OR_EQUAL\x10\x04\x12\t\n\x05\x45QUAL\x10\x05*q\n\x0e\x45valuationType\x12\r\n\tUndefined\x10\x00\x12\x12\n\x0e\x43lassification\x10\x01\x12\r\n\tDetection\x10\x02\x12\x10\n\x0cSegmentation\x10\x03\x12\x0e\n\nClustering\x10\x04\x12\x0b\n\x07Tracker\x10\x05*f\n\x0c\x41PIEventType\x12\x1a\n\x16\x41PI_EVENT_TYPE_NOT_SET\x10\x00\x12\x13\n\x0fON_PREM_PREDICT\x10\x01\x12\x11\n\rON_PREM_TRAIN\x10\x02\x12\x12\n\x0eON_PREM_SEARCH\x10\x03*<\n\x11UsageIntervalType\x12\t\n\x05undef\x10\x00\x12\x07\n\x03\x64\x61y\x10\x01\x12\t\n\x05month\x10\x02\x12\x08\n\x04year\x10\x03*\x1d\n\x08RoleType\x12\x08\n\x04TEAM\x10\x00\x12\x07\n\x03ORG\x10\x01*$\n\x10StatValueAggType\x12\x07\n\x03SUM\x10\x00\x12\x07\n\x03\x41VG\x10\x01*`\n\x0fStatTimeAggType\x12\x0f\n\x0bNO_TIME_AGG\x10\x00\x12\x08\n\x04YEAR\x10\x01\x12\t\n\x05MONTH\x10\x02\x12\x08\n\x04WEEK\x10\x03\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x05\x12\n\n\x06MINUTE\x10\x06*b\n\x13ValidationErrorType\x12!\n\x1dVALIDATION_ERROR_TYPE_NOT_SET\x10\x00\x12\x0e\n\nRESTRICTED\x10\x01\x12\x0c\n\x08\x44\x41TABASE\x10\x02\x12\n\n\x06\x46ORMAT\x10\x03\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"proto/clarifai/api/resources.proto\x12\x0c\x63larifai.api\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/api/utils/matrix.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xe5\x03\n\nAnnotation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x30\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x18\n\x10model_version_id\x18\x10 \x01(\t\x12\"\n\x16\x65mbed_model_version_id\x18\x0e \x01(\tB\x02\x18\x01\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07trusted\x18\n \x01(\x08\x42\x02\x18\x01\x12\x13\n\x0binput_level\x18\x11 \x01(\x08\x12/\n\x0e\x63onsensus_info\x18\x12 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07task_id\x18\x13 \x01(\tJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x9c\x04\n\x03\x41pp\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65\x66\x61ult_language\x18\x03 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ult_workflow_id\x18\x04 \x01(\t\x12\x30\n\x10\x64\x65\x66\x61ult_workflow\x18\x17 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14legal_consent_status\x18\x07 \x01(\r\x12)\n\x08metadata\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x11\n\tsample_ms\x18\x0f \x01(\r\x12,\n\nvisibility\x18\x10 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x14\n\x0c\x64\x61ta_tier_id\x18\x12 \x01(\t\x12\x12\n\nis_starred\x18\x13 \x01(\x08\x12\x12\n\nstar_count\x18\x14 \x01(\x05\x12\r\n\x05notes\x18\x15 \x01(\t\x12\"\n\x05image\x18\x16 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x18\n\x08\x41ppQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x90\x02\n\x0c\x43ollaborator\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12 \n\x04user\x18\x03 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x11\n\tendpoints\x18\x05 \x03(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ndeleted_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x01\n\rCollaboration\x12\x1e\n\x03\x61pp\x18\x01 \x01(\x0b\x32\x11.clarifai.api.App\x12%\n\tapp_owner\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x97\x01\n\x05\x41udio\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\naudio_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.AudioInfo\"b\n\tAudioInfo\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x03 \x01(\x02\x12\x10\n\x08\x62it_rate\x18\x04 \x01(\x05\"w\n\x05Track\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x04 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\x12\x0f\n\x07quality\x18\x05 \x01(\x02J\x04\x08\x03\x10\x04\"h\n\x07\x43luster\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x1f\n\x04hits\x18\x04 \x03(\x0b\x32\x11.clarifai.api.Hit\x12\x12\n\nprojection\x18\x05 \x03(\x02\"M\n\x05\x43olor\x12\x0f\n\x07raw_hex\x18\x01 \x01(\t\x12\x1e\n\x03w3c\x18\x02 \x01(\x0b\x32\x11.clarifai.api.W3C\x12\x13\n\x05value\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\" \n\x03W3C\x12\x0b\n\x03hex\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"/\n\x0cUserAppIDSet\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\"J\n\x0bPatchAction\x12\n\n\x02op\x18\x01 \x01(\t\x12!\n\x19merge_conflict_resolution\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"\xa9\x02\n\x07\x43oncept\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1a\n\x05value\x18\x03 \x01(\x02\x42\x0b\xd5\xb5\x18\x00\x00\x80?\x80\xb5\x18\x01\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x06 \x01(\t\x12\x12\n\ndefinition\x18\x07 \x01(\t\x12\x10\n\x08vocab_id\x18\x08 \x01(\t\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\n \x01(\t\x12\x31\n\rkeypoint_info\x18\x0b \x01(\x0b\x32\x1a.clarifai.api.KeypointInfo\"T\n\x0cKeypointInfo\x12\x16\n\x0ekeypoint_names\x18\x01 \x03(\t\x12,\n\x08skeleton\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.KeypointEdge\"&\n\x0cKeypointEdge\x12\n\n\x02k1\x18\x01 \x01(\r\x12\n\n\x02k2\x18\x02 \x01(\r\"\xa4\x01\n\x0c\x43onceptCount\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12:\n\x12\x63oncept_type_count\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12>\n\x14\x64\x65tail_concept_count\x18\x04 \x01(\x0b\x32 .clarifai.api.DetailConceptCount\"B\n\x10\x43onceptTypeCount\x12\x16\n\x08positive\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08negative\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"\xdf\x01\n\x12\x44\x65tailConceptCount\x12\x31\n\tprocessed\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nto_process\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12.\n\x06\x65rrors\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nprocessing\x18\x04 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\"C\n\x0c\x43onceptQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08language\x18\x02 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x03 \x01(\t\"\xd9\x01\n\x0f\x43onceptRelation\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x0fsubject_concept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\x12-\n\x0eobject_concept\x18\x03 \x01(\x0b\x32\x15.clarifai.api.Concept\x12\x11\n\tpredicate\x18\x04 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x05 \x01(\t\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"y\n\x0eKnowledgeGraph\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x17\n\x0f\x65xamples_app_id\x18\x04 \x01(\t\x12\x1f\n\x17sampled_examples_app_id\x18\x05 \x01(\t\"D\n\x11\x43onceptMappingJob\x12\x1a\n\x12knowledge_graph_id\x18\x01 \x01(\t\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"?\n\x0f\x43onceptLanguage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndefinition\x18\x03 \x01(\t\"\xfa\x04\n\x04\x44\x61ta\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Image\x12\"\n\x05video\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Video\x12\'\n\x08\x63oncepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x03geo\x18\x06 \x01(\x0b\x32\x11.clarifai.api.Geo\x12#\n\x06\x63olors\x18\x07 \x03(\x0b\x32\x13.clarifai.api.Color\x12\'\n\x08\x63lusters\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Cluster\x12+\n\nembeddings\x18\t \x03(\x0b\x32\x17.clarifai.api.Embedding\x12%\n\x07regions\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Region\x12#\n\x06\x66rames\x18\x0c \x03(\x0b\x32\x13.clarifai.api.Frame\x12 \n\x04text\x18\r \x01(\x0b\x32\x12.clarifai.api.Text\x12\"\n\x05\x61udio\x18\x0e \x01(\x0b\x32\x13.clarifai.api.Audio\x12#\n\x06tracks\x18\x0f \x03(\x0b\x32\x13.clarifai.api.Track\x12\x30\n\rtime_segments\x18\x10 \x03(\x0b\x32\x19.clarifai.api.TimeSegment\x12\x1f\n\x04hits\x18\x11 \x03(\x0b\x32\x11.clarifai.api.Hit\x12%\n\x08heatmaps\x18\x12 \x03(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x04\x10\x05J\x04\x08\n\x10\x0b\"\x86\x01\n\x06Region\x12\n\n\x02id\x18\x01 \x01(\t\x12-\n\x0bregion_info\x18\x02 \x01(\x0b\x32\x18.clarifai.api.RegionInfo\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\r\n\x05value\x18\x04 \x01(\x02\x12\x10\n\x08track_id\x18\x05 \x01(\t\"\xae\x02\n\nRegionInfo\x12/\n\x0c\x62ounding_box\x18\x01 \x01(\x0b\x32\x19.clarifai.api.BoundingBox\x12 \n\x04mask\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Mask\x12&\n\x07polygon\x18\x05 \x01(\x0b\x32\x15.clarifai.api.Polygon\x12\"\n\x05point\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Point\x12 \n\x04span\x18\x07 \x01(\x0b\x32\x12.clarifai.api.Span\x12\"\n\x05token\x18\x08 \x01(\x0b\x32\x13.clarifai.api.Token\x12/\n\x12keypoint_locations\x18\t \x03(\x0b\x32\x13.clarifai.api.PointJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"o\n\x0b\x42oundingBox\x12\x15\n\x07top_row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08left_col\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nbottom_row\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tright_col\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"4\n\tFrameInfo\x12\x13\n\x05index\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x12\n\x04time\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"b\n\x05\x46rame\x12+\n\nframe_info\x18\x01 \x01(\x0b\x32\x17.clarifai.api.FrameInfo\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12\n\n\x02id\x18\x03 \x01(\t\"0\n\x04Mask\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x01\x10\x02\".\n\x07Polygon\x12#\n\x06points\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Point\"\xb6\x01\n\x05Point\x12\x11\n\x03row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03\x63ol\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\t\n\x01z\x18\x03 \x01(\x02\x12\x32\n\nvisibility\x18\x04 \x01(\x0e\x32\x1e.clarifai.api.Point.Visibility\"H\n\nVisibility\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0f\n\x0bNOT_VISIBLE\x10\x02\x12\x0f\n\x0bNOT_PRESENT\x10\x03\"J\n\x04Span\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"K\n\x05Token\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"7\n\tEmbedding\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x10\x01\x12\x16\n\x0enum_dimensions\x18\x02 \x01(\r\";\n\x08GeoPoint\x12\x17\n\tlongitude\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08latitude\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\"-\n\x08GeoLimit\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x05value\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\":\n\rGeoBoxedPoint\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\"\x89\x01\n\x03Geo\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\x12)\n\tgeo_limit\x18\x02 \x01(\x0b\x32\x16.clarifai.api.GeoLimit\x12,\n\x07geo_box\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.GeoBoxedPoint\"\x9d\x01\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nimage_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.ImageInfoJ\x04\x08\x03\x10\x04\"N\n\tImageInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x12\n\ncolor_mode\x18\x04 \x01(\t\"O\n\tHostedURL\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\r\n\x05sizes\x18\x03 \x03(\t\x12\x13\n\x0b\x63rossorigin\x18\x04 \x01(\t\"\xde\x01\n\x05Input\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x61taset_ids\x18\x07 \x03(\tJ\x04\x08\x03\x10\x04\"1\n\nInputBatch\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\"\xda\x01\n\nInputCount\x12\x17\n\tprocessed\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_process\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x14\n\x06\x65rrors\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nprocessing\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\treindexed\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_reindex\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1c\n\x0ereindex_errors\x18\x07 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nreindexing\x18\x08 \x01(\rB\x04\x80\xb5\x18\x01\"\x92\x03\n\x07\x44\x61taset\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x41\n\x19\x64\x65\x66\x61ult_annotation_filter\x18\x0c \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\r\n\x05notes\x18\x0b \x01(\t\x12-\n\x07version\x18\r \x01(\x0b\x32\x1c.clarifai.api.DatasetVersionJ\x04\x08\x06\x10\x07J\x04\x08\n\x10\x0b\"\xd8\x01\n\x10\x41nnotationFilter\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12*\n\x0csaved_search\x18\x08 \x01(\x0b\x32\x14.clarifai.api.SearchJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"b\n\x0c\x44\x61tasetInput\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xe9\x05\n\x0e\x44\x61tasetVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x12\n\ndataset_id\x18\x06 \x01(\t\x12H\n\x18\x61nnotation_filter_config\x18\x0f \x01(\x0b\x32$.clarifai.api.AnnotationFilterConfigH\x00\x12@\n\x14model_predict_config\x18\x12 \x01(\x0b\x32 .clarifai.api.ModelPredictConfigH\x00\x12+\n\x06status\x18\x08 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12:\n\x07metrics\x18\x10 \x03(\x0b\x32).clarifai.api.DatasetVersion.MetricsEntry\x12;\n\x0b\x65xport_info\x18\x11 \x01(\x0b\x32&.clarifai.api.DatasetVersionExportInfo\x12)\n\x08metadata\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x1f\n\x17\x65mbed_model_version_ids\x18\x0e \x03(\t\x1aS\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics:\x02\x38\x01\x42\r\n\x0b\x64\x61ta_configJ\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0c\"p\n\x16\x41nnotationFilterConfig\x12\x39\n\x11\x61nnotation_filter\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x1b\n\x13ignore_empty_inputs\x18\x02 \x01(\x08\"8\n\x12ModelPredictConfig\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Model\"\xc3\x08\n\x15\x44\x61tasetVersionMetrics\x12\x32\n\x0cinputs_count\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12<\n\x16unlabeled_inputs_count\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1ainputs_with_metadata_count\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12;\n\x15inputs_with_geo_count\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x33\n\rregions_count\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12-\n\x16region_location_matrix\x18\x15 \x01(\x0b\x32\r.MatrixUint64\x12:\n\x14\x62ounding_boxes_count\x18\x16 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x34\n\x0epolygons_count\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0cpoints_count\x18\x18 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmasks_count\x18\x19 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_inputs_count\x18< \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_frames_count\x18= \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0c\x66rames_count\x18\x1e \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x12\x66rame_inputs_count\x18\x46 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x36\n\x10\x65mbeddings_count\x18( \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_input_tags_count\x18\x32 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1apositive_region_tags_count\x18\x33 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_frame_tags_count\x18\x34 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"\xca\x01\n\x1a\x44\x61tasetVersionMetricsGroup\x12\x13\n\x0bparent_path\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12%\n\x05value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x34\n\x07metrics\x18\x04 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics\"\xd0\x01\n\x18\x44\x61tasetVersionExportInfo\x12\x42\n\x16\x63larifai_data_protobuf\x18\x01 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12>\n\x12\x63larifai_data_json\x18\x03 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12\x30\n\x04\x63oco\x18\x02 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\"\xb4\x01\n\x14\x44\x61tasetVersionExport\x12\x38\n\x06\x66ormat\x18\x01 \x01(\x0e\x32(.clarifai.api.DatasetVersionExportFormat\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x04\x12\x1a\n\x12include_embeddings\x18\x05 \x01(\x08\"n\n\x19WorkflowResultsSimilarity\x12(\n\x0bprobe_input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12\'\n\x0cpool_results\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Hit\"\xf4\x01\n\x03Key\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x07 \x03(\t\x12\x1f\n\x04\x61pps\x18\x04 \x03(\x0b\x32\x11.clarifai.api.App\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61uthorized_idp_ids\x18\t \x03(\t\"\xd8\x07\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x04name\x18\x02 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x06\x61pp_id\x18\x04 \x01(\tB\x04\x80\xb5\x18\x01\x12\x31\n\x0boutput_info\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfoB\x02\x18\x01\x12\x31\n\rmodel_version\x18\x06 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x18\n\x0c\x64isplay_name\x18\x07 \x01(\tB\x02\x18\x01\x12\x0f\n\x07user_id\x18\t \x01(\t\x12/\n\ninput_info\x18\x0c \x01(\x0b\x32\x17.clarifai.api.InputInfoB\x02\x18\x01\x12/\n\ntrain_info\x18\r \x01(\x0b\x32\x17.clarifai.api.TrainInfoB\x02\x18\x01\x12\x31\n\x11\x64\x65\x66\x61ult_eval_info\x18\x1e \x01(\x0b\x32\x16.clarifai.api.EvalInfo\x12\x15\n\rmodel_type_id\x18\x0e \x01(\t\x12\x0c\n\x04task\x18\x1a \x01(\t\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\x12)\n\x08metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07presets\x18\x1b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05notes\x18\x12 \x01(\t\x12\x16\n\x08toolkits\x18\x14 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tuse_cases\x18\x15 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tlanguages\x18\x19 \x03(\tB\x04\x80\xb5\x18\x01\x12\x33\n\x0elanguages_full\x18\x1f \x03(\x0b\x32\x15.clarifai.api.FullTagB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18  \x03(\tB\x04\x80\xb5\x18\x01\x12\x12\n\nis_starred\x18\x16 \x01(\x08\x12\x12\n\nstar_count\x18\x17 \x01(\x05\x12\x31\n\x0bimport_info\x18\x18 \x01(\x0b\x32\x18.clarifai.api.ImportInfoB\x02\x18\x01\x12\x38\n\x14workflow_recommended\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.BoolValueJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x1c\x10\x1d\"t\n\x0eModelReference\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x97\x01\n\x18ModelVersionInputExample\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"\xd4\x01\n\nOutputInfo\x12 \n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x31\n\routput_config\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12\x0f\n\x07message\x18\x03 \x01(\t\x12+\n\nfields_map\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"a\n\tInputInfo\x12+\n\nfields_map\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"4\n\tTrainInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"3\n\x08\x45valInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"5\n\nImportInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x81\x04\n\x0cOutputConfig\x12\'\n\x1b\x63oncepts_mutually_exclusive\x18\x01 \x01(\x08\x42\x02\x18\x01\x12 \n\x12\x63losed_environment\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x1d\n\x11\x65xisting_model_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x1c\n\x10hyper_parameters\x18\x05 \x01(\tB\x02\x18\x01\x12\x1a\n\x0cmax_concepts\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\tmin_value\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12.\n\x0fselect_concepts\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x18\n\x10training_timeout\x18\t \x01(\r\x12\x11\n\tsample_ms\x18\n \x01(\r\x12-\n\x0chyper_params\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x16\x65mbed_model_version_id\x18\x0e \x01(\t\x12)\n!fail_on_missing_positive_examples\x18\x0f \x01(\x08\x12\x33\n\x0emodel_metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x10\x10\x11J\x04\x08\x12\x10\x13\"\xd2\x03\n\tModelType\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cinput_fields\x18\x05 \x03(\t\x12\x15\n\routput_fields\x18\x06 \x03(\t\x12\x11\n\ttrainable\x18\x08 \x01(\x08\x12\x11\n\tcreatable\x18\t \x01(\x08\x12\x15\n\rinternal_only\x18\n \x01(\x08\x12\x37\n\x11model_type_fields\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\"\n\x1arequires_sequential_frames\x18\x0c \x01(\x08\x12;\n\x15\x65xpected_input_layers\x18\x10 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12<\n\x16\x65xpected_output_layers\x18\x11 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12\x35\n\x0f\x65valuation_type\x18\x12 \x01(\x0e\x32\x1c.clarifai.api.EvaluationTypeJ\x04\x08\x07\x10\x08J\x04\x08\x04\x10\x05J\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10\"\x89\x01\n\x0eModelLayerInfo\x12\x17\n\x0f\x64\x61ta_field_name\x18\x01 \x01(\t\x12(\n\x06shapes\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LayerShape\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1f\n\x17requires_label_filename\x18\x04 \x01(\x08\"D\n\x12TritonCondaEnvInfo\x12\x16\n\x0e\x63onda_pack_url\x18\x01 \x01(\t\x12\x16\n\x0e\x63onda_yaml_url\x18\x02 \x01(\t\"l\n\nLayerShape\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x10\n\x08max_dims\x18\x02 \x03(\x05\x12)\n\tdata_type\x18\x03 \x01(\x0e\x32\x16.clarifai.api.DataType\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xd2\x05\n\x0eModelTypeField\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x43\n\nfield_type\x18\x02 \x01(\x0e\x32/.clarifai.api.ModelTypeField.ModelTypeFieldType\x12-\n\rdefault_value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0bplaceholder\x18\x05 \x01(\t\x12\x42\n\x17model_type_enum_options\x18\x06 \x03(\x0b\x32!.clarifai.api.ModelTypeEnumOption\x12\x15\n\rinternal_only\x18\x07 \x01(\x08\x12\x10\n\x08required\x18\x08 \x01(\x08\x12?\n\x15model_type_range_info\x18\t \x01(\x0b\x32 .clarifai.api.ModelTypeRangeInfo\"\xe5\x02\n\x12ModelTypeFieldType\x12!\n\x1dINVALID_MODEL_TYPE_FIELD_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\n\n\x06NUMBER\x10\x03\x12\x15\n\x11\x41RRAY_OF_CONCEPTS\x10\x04\x12$\n ARRAY_OF_CONCEPTS_WITH_THRESHOLD\x10\x05\x12\t\n\x05RANGE\x10\x07\x12\x08\n\x04\x45NUM\x10\x08\x12\x11\n\rCOLLABORATORS\x10\t\x12\x08\n\x04JSON\x10\n\x12\x14\n\x10\x41RRAY_OF_NUMBERS\x10\x0b\x12\x19\n\x15WORKFLOW_EMBED_MODELS\x10\x0c\x12\x14\n\x10\x41RRAY_OF_STRINGS\x10\r\x12\x12\n\x0eRECURSIVE_ENUM\x10\x0e\x12\x0f\n\x0bPYTHON_CODE\x10\x0f\x12\x0e\n\nDATASET_ID\x10\x10\x12\x16\n\x12\x44\x41TASET_VERSION_ID\x10\x11\"\x04\x08\x06\x10\x06\"<\n\x12ModelTypeRangeInfo\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03max\x18\x02 \x01(\x02\x12\x0c\n\x04step\x18\x03 \x01(\x02\"\xd4\x01\n\x13ModelTypeEnumOption\x12\n\n\x02id\x18\x01 \x01(\t\x12\x37\n\x07\x61liases\x18\x05 \x03(\x0b\x32&.clarifai.api.ModelTypeEnumOptionAlias\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x37\n\x11model_type_fields\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\x15\n\rinternal_only\x18\x04 \x01(\x08\x12\x13\n\x0brecommended\x18\x06 \x01(\x08\"C\n\x18ModelTypeEnumOptionAlias\x12\x0e\n\x06id_int\x18\x01 \x01(\x03\x12\x17\n\x0fwildcard_string\x18\x02 \x01(\t\"7\n\nModelQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rmodel_type_id\x18\x03 \x01(\tJ\x04\x08\x02\x10\x03\"\xfc\x05\n\x0cModelVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x04 \x01(\r\x12*\n\x07metrics\x18\x05 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12\x19\n\x11total_input_count\x18\x06 \x01(\r\x12\x44\n\x17pretrained_model_config\x18\x07 \x01(\x0b\x32#.clarifai.api.PretrainedModelConfig\x12\x30\n\x0c\x63ompleted_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\r \x01(\t\x12\x0f\n\x07user_id\x18\x0e \x01(\t\x12/\n\x0bmodified_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07license\x18\x11 \x01(\t\x12-\n\x0boutput_info\x18\x13 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\x12+\n\ninput_info\x18\x14 \x01(\x0b\x32\x17.clarifai.api.InputInfo\x12+\n\ntrain_info\x18\x15 \x01(\x0b\x32\x17.clarifai.api.TrainInfo\x12-\n\x0bimport_info\x18\x16 \x01(\x0b\x32\x18.clarifai.api.ImportInfo\x12\x11\n\ttrain_log\x18\x17 \x01(\tJ\x04\x08\t\x10\nJ\x04\x08\x12\x10\x13\"\xa1\x01\n\x15PretrainedModelConfig\x12\x31\n\x10input_fields_map\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x11output_fields_map\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rmodel_zip_url\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06\">\n\nTrainStats\x12\x30\n\nloss_curve\x18\x01 \x03(\x0b\x32\x1c.clarifai.api.LossCurveEntry\"B\n\x0eLossCurveEntry\x12\r\n\x05\x65poch\x18\x01 \x01(\r\x12\x13\n\x0bglobal_step\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\x02\"1\n\nLabelCount\x12\x14\n\x0c\x63oncept_name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"L\n\x11LabelDistribution\x12\x37\n\x15positive_label_counts\x18\x01 \x03(\x0b\x32\x18.clarifai.api.LabelCount\"B\n\x17\x43ooccurrenceMatrixEntry\x12\x0b\n\x03row\x18\x01 \x01(\t\x12\x0b\n\x03\x63ol\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"`\n\x12\x43ooccurrenceMatrix\x12\x35\n\x06matrix\x18\x01 \x03(\x0b\x32%.clarifai.api.CooccurrenceMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"N\n\x14\x43onfusionMatrixEntry\x12\x11\n\tpredicted\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x02 \x01(\t\x12\x13\n\x05value\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"Z\n\x0f\x43onfusionMatrix\x12\x32\n\x06matrix\x18\x01 \x03(\x0b\x32\".clarifai.api.ConfusionMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"t\n\x03ROC\x12\x11\n\x03\x66pr\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03tpr\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x15\n\rfpr_per_image\x18\x04 \x03(\x02\x12\x16\n\x0e\x66pr_per_object\x18\x05 \x03(\x02\"_\n\x14PrecisionRecallCurve\x12\x14\n\x06recall\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tprecision\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\"\xea\x02\n\rBinaryMetrics\x12\x15\n\x07num_pos\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_neg\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_tot\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x10\n\x02\x66\x31\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12&\n\x07\x63oncept\x18\x06 \x01(\x0b\x32\x15.clarifai.api.Concept\x12$\n\troc_curve\x18\x07 \x01(\x0b\x32\x11.clarifai.api.ROC\x12\x42\n\x16precision_recall_curve\x18\x08 \x01(\x0b\x32\".clarifai.api.PrecisionRecallCurve\x12\x15\n\ravg_precision\x18\t \x01(\x02\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x10\n\x08\x61rea_min\x18\x0b \x01(\x01\x12\x10\n\x08\x61rea_max\x18\x0c \x01(\x01\x12\x0b\n\x03iou\x18\r \x01(\x02\"\x91\x01\n\x0eTrackerMetrics\x12\x10\n\x08mot_mota\x18\x01 \x01(\x02\x12\x18\n\x10mot_num_switches\x18\x02 \x01(\x05\x12\x12\n\nmorse_frag\x18\x03 \x01(\x02\x12\x15\n\ravg_precision\x18\x04 \x01(\x02\x12\x0c\n\x04\x61iid\x18\x05 \x01(\t\x12\x1a\n\x12unique_switch_rate\x18\x06 \x01(\x02\"\xee\x01\n\x10\x45valTestSetEntry\x12\x0e\n\x02id\x18\x01 \x01(\tB\x02\x18\x01\x12\x0f\n\x03url\x18\x02 \x01(\tB\x02\x18\x01\x12\"\n\x05input\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\x12predicted_concepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x34\n\x15ground_truth_concepts\x18\x04 \x03(\x0b\x32\x15.clarifai.api.Concept\x12,\n\nannotation\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\xcd\x01\n\x0eLOPQEvalResult\x12\t\n\x01k\x18\x01 \x01(\x05\x12#\n\x15recall_vs_brute_force\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1akendall_tau_vs_brute_force\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1amost_frequent_code_percent\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tlopq_ndcg\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10\x62rute_force_ndcg\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\"\x8c\x03\n\x0eMetricsSummary\x12\x19\n\rtop1_accuracy\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rtop5_accuracy\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x1f\n\x11macro_avg_roc_auc\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1f\n\x11macro_std_roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_avg_f1_score\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_std_f1_score\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x13macro_avg_precision\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10macro_avg_recall\x18\x08 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x19mean_avg_precision_iou_50\x18\n \x01(\x02\x12$\n\x1cmean_avg_precision_iou_range\x18\x0b \x01(\x02\x12\x32\n\x0clopq_metrics\x18\t \x03(\x0b\x32\x1c.clarifai.api.LOPQEvalResult\"\xda\x04\n\x0b\x45valMetrics\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\n \x01(\t\x12-\n\x07summary\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.MetricsSummary\x12\x37\n\x10\x63onfusion_matrix\x18\x03 \x01(\x0b\x32\x1d.clarifai.api.ConfusionMatrix\x12=\n\x13\x63ooccurrence_matrix\x18\x04 \x01(\x0b\x32 .clarifai.api.CooccurrenceMatrix\x12\x35\n\x0clabel_counts\x18\x05 \x01(\x0b\x32\x1f.clarifai.api.LabelDistribution\x12\x33\n\x0e\x62inary_metrics\x18\x06 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x30\n\x08test_set\x18\x07 \x03(\x0b\x32\x1e.clarifai.api.EvalTestSetEntry\x12\x34\n\x0fmetrics_by_area\x18\x08 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x10metrics_by_class\x18\t \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x0ftracker_metrics\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.TrackerMetrics\x12)\n\teval_info\x18\x0c \x01(\x0b\x32\x16.clarifai.api.EvalInfo\"\xb7\x01\n\x0b\x46ieldsValue\x12\x18\n\x10\x63onfusion_matrix\x18\x01 \x01(\x08\x12\x1b\n\x13\x63ooccurrence_matrix\x18\x02 \x01(\x08\x12\x14\n\x0clabel_counts\x18\x03 \x01(\x08\x12\x16\n\x0e\x62inary_metrics\x18\x04 \x01(\x08\x12\x10\n\x08test_set\x18\x05 \x01(\x08\x12\x17\n\x0fmetrics_by_area\x18\x06 \x01(\x08\x12\x18\n\x10metrics_by_class\x18\x07 \x01(\x08\"\xdb\x01\n\x06Output\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12 \n\x04\x64\x61ta\x18\x06 \x01(\x0b\x32\x12.clarifai.api.Data\"4\n\tScopeDeps\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\":\n\x0c\x45ndpointDeps\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\"\x8d\x01\n\x03Hit\x12\x13\n\x05score\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\x12,\n\nannotation\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\"#\n\x08HitCount\x12\x17\n\x0f\x65stimated_total\x18\x01 \x01(\x04\"\x8d\x01\n\x03\x41nd\x12\"\n\x05input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12$\n\x06output\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Output\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x88\x01\n\x05Query\x12#\n\x04\x61nds\x18\x01 \x03(\x0b\x32\x11.clarifai.api.AndB\x02\x18\x01\x12\x10\n\x08language\x18\x02 \x01(\t\x12%\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Filter\x12!\n\x05ranks\x18\x04 \x03(\x0b\x32\x12.clarifai.api.Rank\"\xd6\x03\n\x06Search\x12\"\n\x05query\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Query\x12\n\n\x02id\x18\x02 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x05\x61s_of\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08git_hash\x18\x06 \x01(\t\x12.\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\talgorithm\x18\t \x01(\t\x12\x0c\n\x04save\x18\n \x01(\x08\x12\x11\n\tmin_value\x18\x0b \x01(\x02\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12+\n\x06metric\x18\r \x01(\x0e\x32\x1b.clarifai.api.Search.Metric\"I\n\x06Metric\x12\x12\n\x0eMETRIC_NOT_SET\x10\x00\x12\x16\n\x12\x45UCLIDEAN_DISTANCE\x10\x01\x12\x13\n\x0f\x43OSINE_DISTANCE\x10\x02\"\xa4\x01\n\x06\x46ilter\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x38\n\x17last_updated_time_range\x18\x06 \x01(\x0b\x32\x17.clarifai.api.TimeRange\"i\n\tTimeRange\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x04Rank\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x8d\x02\n\x17\x41nnotationSearchMetrics\x12*\n\x0cground_truth\x18\x01 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Search\x12*\n\x07metrics\x18\x03 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x05 \x01(\r\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"\x91\x01\n\x04Text\x12\x0b\n\x03raw\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x1b\n\x13\x61llow_duplicate_url\x18\x03 \x01(\x08\x12\'\n\x06hosted\x18\x04 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12)\n\ttext_info\x18\x05 \x01(\x0b\x32\x16.clarifai.api.TextInfo\"0\n\x08TextInfo\x12\x12\n\nchar_count\x18\x01 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x02 \x01(\t\"\xfc\x05\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\rprimary_email\x18\x02 \x01(\tB\x02\x18\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x14\n\x0c\x63ompany_name\x18\x05 \x01(\t\x12\x11\n\tjob_title\x18\x13 \x01(\t\x12\x10\n\x08job_role\x18\x14 \x01(\t\x12\x15\n\tbill_type\x18\x07 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x11\x64\x61te_gdpr_consent\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_tos_consent\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12>\n\x16\x64\x61te_marketing_consent\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_pii_consent\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12-\n\x08metadata\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x37\n\x0f\x65mail_addresses\x18\x0c \x03(\x0b\x32\x1a.clarifai.api.EmailAddressB\x02\x18\x01\x12#\n\x17two_factor_auth_enabled\x18\x0f \x01(\x08\x42\x02\x18\x01\x12\x17\n\x0bteams_count\x18\x10 \x01(\rB\x02\x18\x01\x12\x12\n\nis_starred\x18\x15 \x01(\x08\x12\x12\n\nstar_count\x18\x16 \x01(\x05\x12,\n\nvisibility\x18\x11 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12-\n\x0buser_detail\x18\x12 \x01(\x0b\x32\x18.clarifai.api.UserDetailJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\xd1\x03\n\nUserDetail\x12\x15\n\rprimary_email\x18\x01 \x01(\t\x12\x11\n\tbill_type\x18\x02 \x01(\t\x12\x35\n\x11\x64\x61te_gdpr_consent\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_tos_consent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x64\x61te_marketing_consent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_pii_consent\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x33\n\x0f\x65mail_addresses\x18\x07 \x03(\x0b\x32\x1a.clarifai.api.EmailAddress\x12\x1f\n\x17two_factor_auth_enabled\x18\t \x01(\x08\x12\x13\n\x0bteams_count\x18\n \x01(\r\x12\x0f\n\x07\x63ountry\x18\x0b \x01(\t\x12\r\n\x05state\x18\x0c \x01(\tJ\x04\x08\x08\x10\t\"R\n\x0c\x45mailAddress\x12\x13\n\x05\x65mail\x18\x01 \x01(\tB\x04\x80\xb5\x18\x01\x12\x15\n\x07primary\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08verified\x18\x03 \x01(\x08\x42\x04\x80\xb5\x18\x01\"\x1d\n\x08Password\x12\x11\n\tplaintext\x18\x01 \x01(\t\"\x86\x03\n\x12PasswordViolations\x12\x16\n\x0eminimum_length\x18\x01 \x01(\x08\x12\x16\n\x0emaximum_length\x18\x02 \x01(\x08\x12\x19\n\x11upper_case_needed\x18\x03 \x01(\x08\x12\x19\n\x11lower_case_needed\x18\x04 \x01(\x08\x12\x16\n\x0enumeric_needed\x18\x05 \x01(\x08\x12\x1f\n\x17non_alphanumeric_needed\x18\x06 \x01(\x08\x12\x16\n\x0epassword_reuse\x18\x07 \x01(\x08\x12\x15\n\rexclude_names\x18\x08 \x01(\x08\x12\x15\n\rexclude_email\x18\t \x01(\x08\x12\x1c\n\x14no_confusing_letters\x18\n \x01(\x08\x12\x1b\n\x13no_simple_passwords\x18\x0b \x01(\x08\x12\x18\n\x10no_common_vocabs\x18\x0c \x01(\x08\x12\x1b\n\x13no_overlap_with_old\x18\r \x01(\x08\x12\x19\n\x11password_lifespan\x18\x0e \x01(\x08\"\xae\x01\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\x15\n\rthumbnail_url\x18\x05 \x01(\t\x12\'\n\x06hosted\x18\x06 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nvideo_info\x18\x07 \x01(\x0b\x32\x17.clarifai.api.VideoInfo\"\x8e\x01\n\tVideoInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0b\n\x03\x66ps\x18\x03 \x01(\x02\x12\x14\n\x0cvideo_format\x18\x04 \x01(\t\x12\x10\n\x08\x62it_rate\x18\x05 \x01(\x05\x12\x13\n\x0b\x66rame_count\x18\x06 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x07 \x01(\x02\"\xcf\x03\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x05nodes\x18\x04 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\x07 \x01(\t\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x07version\x18\t \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x12\n\nis_starred\x18\n \x01(\x08\x12\x12\n\nstar_count\x18\x0b \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\r\n\x05notes\x18\r \x01(\t\x12\x17\n\tuse_cases\x18\x0e \x03(\tB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18\x0f \x03(\tB\x04\x80\xb5\x18\x01\"\xde\x02\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x05nodes\x18\x06 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06\x61pp_id\x18\x08 \x01(\t\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07license\x18\x0b \x01(\t\"\xbd\x01\n\x0cWorkflowNode\x12\n\n\x02id\x18\x01 \x01(\t\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\x12,\n\x0bnode_inputs\x18\x03 \x03(\x0b\x32\x17.clarifai.api.NodeInput\x12\x17\n\x0fsuppress_output\x18\x04 \x01(\x08\x12\x36\n\x14output_info_override\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\"\x1c\n\tNodeInput\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x02\n\x0eWorkflowResult\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12%\n\x07outputs\x18\x06 \x03(\x0b\x32\x14.clarifai.api.Output\x12\x17\n\x0fsuppress_output\x18\x07 \x01(\x08\"\x1b\n\rWorkflowState\x12\n\n\x02id\x18\x01 \x01(\t\"\xd8\x02\n\x0e\x41ppDuplication\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nnew_app_id\x18\x02 \x01(\t\x12\x14\n\x0cnew_app_name\x18\x03 \x01(\t\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x66ilter\x18\x07 \x01(\x0b\x32#.clarifai.api.AppDuplicationFilters\x12\x17\n\x0f\x65xisting_app_id\x18\x08 \x01(\t\x12/\n\x08progress\x18\t \x03(\x0b\x32\x1d.clarifai.api.AppCopyProgress\"/\n\x0f\x41ppCopyProgress\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05\"\x8a\x01\n\x15\x41ppDuplicationFilters\x12\x13\n\x0b\x63opy_inputs\x18\x01 \x01(\x08\x12\x15\n\rcopy_concepts\x18\x02 \x01(\x08\x12\x18\n\x10\x63opy_annotations\x18\x03 \x01(\x08\x12\x13\n\x0b\x63opy_models\x18\x04 \x01(\x08\x12\x16\n\x0e\x63opy_workflows\x18\x05 \x01(\x08\"\xfa\x02\n\nLabelOrder\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x61uto_release\x18\x04 \x01(\x08\x12\x17\n\x0f\x61llow_empty_tag\x18\x05 \x01(\x08\x12\x38\n\x14\x64\x65sired_fulfill_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15\x65stimate_fulfill_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x04task\x18\x08 \x01(\x0b\x32\x12.clarifai.api.Task\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xe5\x05\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.clarifai.api.Task.TaskType\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12(\n\x06worker\x18\x06 \x01(\x0b\x32\x18.clarifai.api.TaskWorker\x12\x13\n\x0b\x63oncept_ids\x18\x07 \x03(\t\x12\x33\n\x0cinput_source\x18\x08 \x01(\x0b\x32\x1d.clarifai.api.TaskInputSource\x12\x11\n\tsample_ms\x18\t \x01(\r\x12\x33\n\x0c\x61i_assistant\x18\n \x01(\x0b\x32\x1d.clarifai.api.TaskAIAssistant\x12(\n\x06review\x18\x0b \x01(\x0b\x32\x18.clarifai.api.TaskReview\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0c\n\x04name\x18\r \x01(\t\x12:\n\x10\x61i_assist_params\x18\x0e \x01(\x0b\x32 .clarifai.api.AiAssistParameters\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\x0f\n\x07user_id\x18\x11 \x01(\t\x12\x16\n\x0elabel_order_id\x18\x12 \x01(\t\"l\n\x08TaskType\x12\x10\n\x0cTYPE_NOT_SET\x10\x00\x12\x1b\n\x17\x43ONCEPTS_CLASSIFICATION\x10\x01\x12\x1a\n\x16\x42OUNDING_BOX_DETECTION\x10\x02\x12\x15\n\x11POLYGON_DETECTION\x10\x03\"`\n\x12\x41iAssistParameters\x12\x15\n\rmin_threshold\x18\x01 \x01(\x02\x12\x15\n\rmax_threshold\x18\x02 \x01(\x02\x12\x1c\n\x14\x63oncept_relation_ids\x18\x03 \x03(\t\"\xbf\x02\n\nTaskWorker\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskWorker.TaskWorkerStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x04 \x03(\x0b\x32\x12.clarifai.api.User\x12T\n\x19partitioned_strategy_info\x18\x03 \x01(\x0b\x32/.clarifai.api.TaskWorkerPartitionedStrategyInfoH\x00\"R\n\x12TaskWorkerStrategy\x12\x1b\n\x17WORKER_STRATEGY_NOT_SET\x10\x00\x12\x0f\n\x0bPARTITIONED\x10\x02\x12\x08\n\x04\x46ULL\x10\x03\"\x04\x08\x01\x10\x01\x42\x0f\n\rstrategy_info\"\xa9\x02\n!TaskWorkerPartitionedStrategyInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.clarifai.api.TaskWorkerPartitionedStrategyInfo.TaskWorkerPartitionedStrategy\x12\x19\n\x11workers_per_input\x18\x02 \x01(\x05\x12(\n\x07weights\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"b\n\x1dTaskWorkerPartitionedStrategy\x12\'\n#PARTITIONED_WORKER_STRATEGY_NOT_SET\x10\x00\x12\n\n\x06\x45VENLY\x10\x01\x12\x0c\n\x08WEIGHTED\x10\x02\"\xc3\x01\n\x0fTaskInputSource\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.clarifai.api.TaskInputSource.TaskInputSourceType\x12\n\n\x02id\x18\x02 \x01(\t\"c\n\x13TaskInputSourceType\x12\x1d\n\x19INPUT_SOURCE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nALL_INPUTS\x10\x01\x12\x10\n\x0cSAVED_SEARCH\x10\x02\x12\x0b\n\x07\x44\x41TASET\x10\x03\"\x90\x03\n\nTaskReview\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskReview.TaskReviewStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x05 \x03(\x0b\x32\x12.clarifai.api.User\x12J\n\x14manual_strategy_info\x18\x03 \x01(\x0b\x32*.clarifai.api.TaskReviewManualStrategyInfoH\x00\x12P\n\x17\x63onsensus_strategy_info\x18\x04 \x01(\x0b\x32-.clarifai.api.TaskReviewConsensusStrategyInfoH\x00\"[\n\x12TaskReviewStrategy\x12 \n\x1cTASK_REVIEW_STRATEGY_NOT_SET\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06MANUAL\x10\x02\x12\r\n\tCONSENSUS\x10\x03\x42\x0f\n\rstrategy_info\"9\n\x1cTaskReviewManualStrategyInfo\x12\x19\n\x11sample_percentage\x18\x01 \x01(\x02\"C\n\x1fTaskReviewConsensusStrategyInfo\x12\x1a\n\x12\x61pproval_threshold\x18\x02 \x01(\rJ\x04\x08\x01\x10\x02\"&\n\x0fTaskAIAssistant\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"\xbc\x01\n\x16TaskStatusCountPerUser\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x15\n\x07pending\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1d\n\x0f\x61waiting_review\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07success\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1b\n\rreview_denied\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\'\n\x19\x61waiting_consensus_review\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\"\x81\x02\n\tCollector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1d\n\x15pre_queue_workflow_id\x18\x04 \x01(\t\x12\x1e\n\x16post_queue_workflow_id\x18\x05 \x01(\t\x12\x37\n\x10\x63ollector_source\x18\x06 \x01(\x0b\x32\x1d.clarifai.api.CollectorSource\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"t\n\x0f\x43ollectorSource\x12\x61\n\'api_post_model_outputs_collector_source\x18\x02 \x01(\x0b\x32\x30.clarifai.api.APIPostModelOutputsCollectorSource\"\x99\x01\n\"APIPostModelOutputsCollectorSource\x12\x15\n\rmodel_user_id\x18\x01 \x01(\t\x12\x14\n\x0cmodel_app_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x18\n\x10model_version_id\x18\x04 \x01(\t\x12\x1a\n\x12post_inputs_key_id\x18\x05 \x01(\t\"R\n\tStatValue\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04tags\x18\x03 \x03(\t\"\xa6\x01\n\x18StatValueAggregateResult\x12?\n\x15stat_value_aggregates\x18\x01 \x03(\x0b\x32 .clarifai.api.StatValueAggregate\x12I\n\x1astat_value_aggregate_query\x18\x02 \x01(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"t\n\x12StatValueAggregate\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x61ggregate_value\x18\x02 \x01(\x02\x12\r\n\x05\x63ount\x18\x03 \x01(\x04\x12\x0c\n\x04tags\x18\x04 \x03(\t\"\x91\x02\n\x17StatValueAggregateQuery\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x12\n\ntag_groups\x18\x02 \x03(\t\x12;\n\x13stat_value_agg_type\x18\x03 \x01(\x0e\x32\x1e.clarifai.api.StatValueAggType\x12\x39\n\x12stat_time_agg_type\x18\x04 \x01(\x0e\x32\x1d.clarifai.api.StatTimeAggType\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xef\x01\n\x19\x44\x61tasetInputsSearchAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x12\n\ndataset_id\x18\x05 \x01(\t\x12$\n\x06search\x18\x06 \x01(\x0b\x32\x14.clarifai.api.Search\"O\n\x17PCAProjectionComparator\x12\x1a\n\x12\x64istance_threshold\x18\x01 \x01(\x02\x12\x18\n\x10model_version_id\x18\x02 \x01(\t\"K\n\x1b\x44uplicateAnnotationsResults\x12\x16\n\x0e\x64uplicate_cfid\x18\x01 \x03(\t\x12\x14\n\x0cunique_count\x18\x02 \x01(\x05\"\x87\x01\n\nVisibility\x12\x33\n\x08gettable\x18\x01 \x01(\x0e\x32!.clarifai.api.Visibility.Gettable\"D\n\x08Gettable\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\x0b\n\x07PRIVATE\x10\n\x12\x07\n\x03ORG\x10\x1e\x12\n\n\x06PUBLIC\x10\x32\"X\n\x0eTrendingMetric\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\x12\x12\n\nview_count\x18\x04 \x01(\x04\"#\n\x07\x46ullTag\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x0bTimeSegment\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x03 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\"D\n\x08TimeInfo\x12\x12\n\nnum_frames\x18\x01 \x01(\r\x12\x12\n\nbegin_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\"\xbf\x02\n\x06Module\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x07 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x0e\n\x06\x61pp_id\x18\n \x01(\t\x12\x33\n\x0emodule_version\x18\x0b \x01(\x0b\x32\x1b.clarifai.api.ModuleVersionJ\x04\x08\x02\x10\x03\"\xbe\x04\n\rModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\r\n\x05notes\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0egit_commit_url\x18\n \x01(\t\x12\x39\n\nmodule_nav\x18\x0b \x01(\x0b\x32%.clarifai.api.ModuleVersion.ModuleNav\x12\x10\n\x08\x61pproved\x18\x0c \x01(\x08\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x1a\x45\n\x0cModuleSubNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x11\n\tquery_key\x18\x02 \x01(\t\x12\x13\n\x0bquery_value\x18\x03 \x01(\t\x1a]\n\tModuleNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x41\n\x0fmodule_sub_navs\x18\x02 \x03(\x0b\x32(.clarifai.api.ModuleVersion.ModuleSubNavJ\x04\x08\x05\x10\x06\"\xad\x02\n\x16InstalledModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeploy_url\x18\x07 \x01(\t\x12,\n\nvisibility\x18\x08 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06key_id\x18\t \x01(\t\"\x8d\x03\n\rBulkOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\tinput_ids\x18\x02 \x01(\x0b\x32\x16.clarifai.api.InputIDsH\x00\x12&\n\x06search\x18\n \x01(\x0b\x32\x14.clarifai.api.SearchH\x00\x12*\n\toperation\x18\x03 \x01(\x0b\x32\x17.clarifai.api.Operation\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08progress\x18\x06 \x01(\x0b\x32\x16.clarifai.api.Progress\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x0e\n\x0cinput_source\"\x1d\n\x08InputIDs\x12\x11\n\tinput_ids\x18\x01 \x03(\t\"8\n\x08Progress\x12\x11\n\tprocessed\x18\x01 \x01(\r\x12\x19\n\x11last_processed_id\x18\x02 \x01(\t\"\xca\x03\n\tOperation\x12\x31\n\x0c\x61\x64\x64_concepts\x18\x01 \x01(\x0b\x32\x19.clarifai.api.AddConceptsH\x00\x12\x37\n\x0f\x64\x65lete_concepts\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DeleteConceptsH\x00\x12\x31\n\x0c\x61\x64\x64_metadata\x18\x03 \x01(\x0b\x32\x19.clarifai.api.AddMetadataH\x00\x12\x37\n\x0f\x64\x65lete_metadata\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.DeleteMetadataH\x00\x12\x33\n\roverwrite_geo\x18\x05 \x01(\x0b\x32\x1a.clarifai.api.OverwriteGeoH\x00\x12-\n\ndelete_geo\x18\x06 \x01(\x0b\x32\x17.clarifai.api.DeleteGeoH\x00\x12>\n\x13\x64\x65lete_from_dataset\x18\x07 \x01(\x0b\x32\x1f.clarifai.api.DeleteFromDatasetH\x00\x12\x34\n\x0e\x61\x64\x64_to_dataset\x18\x08 \x01(\x0b\x32\x1a.clarifai.api.AddToDatasetH\x00\x42\x0b\n\toperation\"6\n\x0b\x41\x64\x64\x43oncepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\"K\n\x0e\x44\x65leteConcepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x10\n\x08user_ids\x18\x02 \x03(\t\"8\n\x0b\x41\x64\x64Metadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\";\n\x0e\x44\x65leteMetadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\".\n\x0cOverwriteGeo\x12\x1e\n\x03geo\x18\x01 \x01(\x0b\x32\x11.clarifai.api.Geo\"\x0b\n\tDeleteGeo\"\"\n\x0c\x41\x64\x64ToDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\'\n\x11\x44\x65leteFromDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\xce\x02\n\x0cInputsAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\x12\x34\n\x08progress\x18\x07 \x01(\x0b\x32\".clarifai.api.InputsAddJobProgress\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x0f\x65xtraction_jobs\x18\n \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\x12%\n\x07uploads\x18\x0b \x03(\x0b\x32\x14.clarifai.api.UploadJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"u\n\x14InputsAddJobProgress\x12\x15\n\rpending_count\x18\x01 \x01(\x04\x12\x19\n\x11in_progress_count\x18\x02 \x01(\x04\x12\x15\n\rsuccess_count\x18\x03 \x01(\x04\x12\x14\n\x0c\x66\x61iled_count\x18\x04 \x01(\x04\"\x95\x02\n\x06Upload\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x63ontent_name\x18\x08 \x01(\t\x12\x16\n\x0e\x63ontent_length\x18\x06 \x01(\x04\x12\x13\n\x0b\x63ontent_url\x18\x07 \x01(\t\"K\n\x11UploadContentPart\x12\x13\n\x0brange_start\x18\x01 \x01(\x04\x12\x13\n\x0bpart_number\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"l\n\x19\x43ustomCodeOperatorRequest\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\x12*\n\x08metadata\x18\xea\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xf9\x01\n\x13InputsExtractionJob\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12;\n\x08progress\x18\x04 \x01(\x0b\x32).clarifai.api.InputsExtractionJobProgress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xad\x02\n\x1bInputsExtractionJobProgress\x12\x1a\n\x12read_objects_count\x18\x01 \x01(\x04\x12\x1a\n\x12\x61udio_inputs_count\x18\x02 \x01(\x04\x12\x1a\n\x12image_inputs_count\x18\x03 \x01(\x04\x12\x1a\n\x12video_inputs_count\x18\x04 \x01(\x04\x12\x19\n\x11text_inputs_count\x18\x05 \x01(\x04\x12\x1e\n\x16pending_archives_count\x18\x06 \x01(\x04\x12\"\n\x1ain_progress_archives_count\x18\x07 \x01(\x04\x12 \n\x18\x63ompleted_archives_count\x18\x08 \x01(\x04\x12\x1d\n\x15\x66\x61iled_archives_count\x18\t \x01(\x04\"W\n\x10InputsDataSource\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12(\n\x03url\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.DataSourceURL\"V\n\rDataSourceURL\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x38\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32#.clarifai.api.DataSourceCredentials\"\xa7\x01\n\x15\x44\x61taSourceCredentials\x12*\n\x08s3_creds\x18\x01 \x01(\x0b\x32\x16.clarifai.api.AWSCredsH\x00\x12\x13\n\tgcp_creds\x18\x02 \x01(\x0cH\x00\x12\x38\n\x10\x61zure_blob_creds\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.AzureBlobCredsH\x00\x42\r\n\x0b\x63redentialsJ\x04\x08\x03\x10\x04\"K\n\x08\x41WSCreds\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0e\n\x06secret\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\tJ\x04\x08\x01\x10\x02\";\n\x0e\x41zureBlobCreds\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\"`\n\x0cInputsUpload\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x02 \x01(\t\x12$\n\x06upload\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Upload*\xf9\x01\n\x1e\x44\x61tasetVersionMetricsGroupType\x12.\n*DATASET_VERSION_METRICS_GROUP_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_TYPE\x10\x02\x12\x0e\n\nCONCEPT_ID\x10\n\x12\x12\n\x0e\x43ONCEPTS_COUNT\x10\x0b\x12\x18\n\x14\x42OUNDING_BOXES_COUNT\x10\x14\x12\x12\n\x0ePOLYGONS_COUNT\x10\x15\x12\x10\n\x0cPOINTS_COUNT\x10\x16\x12\x0f\n\x0bMASKS_COUNT\x10\x17\x12\x10\n\x0cPIXELS_COUNT\x10\x1e\x12\x10\n\x0c\x41SPECT_RATIO\x10\x1f*\x85\x01\n\x1a\x44\x61tasetVersionExportFormat\x12)\n%DATASET_VERSION_EXPORT_FORMAT_NOT_SET\x10\x00\x12\x1a\n\x16\x43LARIFAI_DATA_PROTOBUF\x10\x01\x12\x16\n\x12\x43LARIFAI_DATA_JSON\x10\x03\x12\x08\n\x04\x43OCO\x10\x02*H\n\x10\x45xpirationAction\x12\x1d\n\x19\x45XPIRATION_ACTION_NOT_SET\x10\x00\x12\t\n\x05\x44\x45LAY\x10\x01\x12\n\n\x06\x45XPIRY\x10\x02*M\n\x0cLicenseScope\x12\x19\n\x15LICENSE_SCOPE_NOT_SET\x10\x00\x12\x0b\n\x07PREDICT\x10\x01\x12\t\n\x05TRAIN\x10\x02\x12\n\n\x06SEARCH\x10\x03*P\n\x08\x44\x61taType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\t\n\x05UINT8\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04\x46P32\x10\x05*\x8f\x01\n\x0fValueComparator\x12\x1d\n\x19\x43ONCEPT_THRESHOLD_NOT_SET\x10\x00\x12\x10\n\x0cGREATER_THAN\x10\x01\x12\x19\n\x15GREATER_THAN_OR_EQUAL\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x16\n\x12LESS_THAN_OR_EQUAL\x10\x04\x12\t\n\x05\x45QUAL\x10\x05*q\n\x0e\x45valuationType\x12\r\n\tUndefined\x10\x00\x12\x12\n\x0e\x43lassification\x10\x01\x12\r\n\tDetection\x10\x02\x12\x10\n\x0cSegmentation\x10\x03\x12\x0e\n\nClustering\x10\x04\x12\x0b\n\x07Tracker\x10\x05*f\n\x0c\x41PIEventType\x12\x1a\n\x16\x41PI_EVENT_TYPE_NOT_SET\x10\x00\x12\x13\n\x0fON_PREM_PREDICT\x10\x01\x12\x11\n\rON_PREM_TRAIN\x10\x02\x12\x12\n\x0eON_PREM_SEARCH\x10\x03*<\n\x11UsageIntervalType\x12\t\n\x05undef\x10\x00\x12\x07\n\x03\x64\x61y\x10\x01\x12\t\n\x05month\x10\x02\x12\x08\n\x04year\x10\x03*\x1d\n\x08RoleType\x12\x08\n\x04TEAM\x10\x00\x12\x07\n\x03ORG\x10\x01*$\n\x10StatValueAggType\x12\x07\n\x03SUM\x10\x00\x12\x07\n\x03\x41VG\x10\x01*`\n\x0fStatTimeAggType\x12\x0f\n\x0bNO_TIME_AGG\x10\x00\x12\x08\n\x04YEAR\x10\x01\x12\t\n\x05MONTH\x10\x02\x12\x08\n\x04WEEK\x10\x03\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x05\x12\n\n\x06MINUTE\x10\x06*b\n\x13ValidationErrorType\x12!\n\x1dVALIDATION_ERROR_TYPE_NOT_SET\x10\x00\x12\x0e\n\nRESTRICTED\x10\x01\x12\x0c\n\x08\x44\x41TABASE\x10\x02\x12\n\n\x06\x46ORMAT\x10\x03\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.resources_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025com.clarifai.grpc.apiP\001Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\242\002\004CAIP'
@@ -226,412 +226,416 @@
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_review']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['success']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['success']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['review_denied']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['review_denied']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_consensus_review']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_consensus_review']._serialized_options = b'\200\265\030\001'
-  _DATASETVERSIONMETRICSGROUPTYPE._serialized_start=33834
-  _DATASETVERSIONMETRICSGROUPTYPE._serialized_end=34083
-  _DATASETVERSIONEXPORTFORMAT._serialized_start=34086
-  _DATASETVERSIONEXPORTFORMAT._serialized_end=34219
-  _EXPIRATIONACTION._serialized_start=34221
-  _EXPIRATIONACTION._serialized_end=34293
-  _LICENSESCOPE._serialized_start=34295
-  _LICENSESCOPE._serialized_end=34372
-  _DATATYPE._serialized_start=34374
-  _DATATYPE._serialized_end=34454
-  _VALUECOMPARATOR._serialized_start=34457
-  _VALUECOMPARATOR._serialized_end=34600
-  _EVALUATIONTYPE._serialized_start=34602
-  _EVALUATIONTYPE._serialized_end=34715
-  _APIEVENTTYPE._serialized_start=34717
-  _APIEVENTTYPE._serialized_end=34819
-  _USAGEINTERVALTYPE._serialized_start=34821
-  _USAGEINTERVALTYPE._serialized_end=34881
-  _ROLETYPE._serialized_start=34883
-  _ROLETYPE._serialized_end=34912
-  _STATVALUEAGGTYPE._serialized_start=34914
-  _STATVALUEAGGTYPE._serialized_end=34950
-  _STATTIMEAGGTYPE._serialized_start=34952
-  _STATTIMEAGGTYPE._serialized_end=35048
-  _VALIDATIONERRORTYPE._serialized_start=35050
-  _VALIDATIONERRORTYPE._serialized_end=35148
+  _DATASETVERSIONMETRICSGROUPTYPE._serialized_start=34144
+  _DATASETVERSIONMETRICSGROUPTYPE._serialized_end=34393
+  _DATASETVERSIONEXPORTFORMAT._serialized_start=34396
+  _DATASETVERSIONEXPORTFORMAT._serialized_end=34529
+  _EXPIRATIONACTION._serialized_start=34531
+  _EXPIRATIONACTION._serialized_end=34603
+  _LICENSESCOPE._serialized_start=34605
+  _LICENSESCOPE._serialized_end=34682
+  _DATATYPE._serialized_start=34684
+  _DATATYPE._serialized_end=34764
+  _VALUECOMPARATOR._serialized_start=34767
+  _VALUECOMPARATOR._serialized_end=34910
+  _EVALUATIONTYPE._serialized_start=34912
+  _EVALUATIONTYPE._serialized_end=35025
+  _APIEVENTTYPE._serialized_start=35027
+  _APIEVENTTYPE._serialized_end=35129
+  _USAGEINTERVALTYPE._serialized_start=35131
+  _USAGEINTERVALTYPE._serialized_end=35191
+  _ROLETYPE._serialized_start=35193
+  _ROLETYPE._serialized_end=35222
+  _STATVALUEAGGTYPE._serialized_start=35224
+  _STATVALUEAGGTYPE._serialized_end=35260
+  _STATTIMEAGGTYPE._serialized_start=35262
+  _STATTIMEAGGTYPE._serialized_end=35358
+  _VALIDATIONERRORTYPE._serialized_start=35360
+  _VALIDATIONERRORTYPE._serialized_end=35458
   _ANNOTATION._serialized_start=312
   _ANNOTATION._serialized_end=797
   _APP._serialized_start=800
-  _APP._serialized_end=1290
-  _APPQUERY._serialized_start=1292
-  _APPQUERY._serialized_end=1316
-  _COLLABORATOR._serialized_start=1319
-  _COLLABORATOR._serialized_end=1591
-  _COLLABORATION._serialized_start=1594
-  _COLLABORATION._serialized_end=1763
-  _AUDIO._serialized_start=1766
-  _AUDIO._serialized_end=1917
-  _AUDIOINFO._serialized_start=1919
-  _AUDIOINFO._serialized_end=2017
-  _TRACK._serialized_start=2019
-  _TRACK._serialized_end=2138
-  _CLUSTER._serialized_start=2140
-  _CLUSTER._serialized_end=2244
-  _COLOR._serialized_start=2246
-  _COLOR._serialized_end=2323
-  _W3C._serialized_start=2325
-  _W3C._serialized_end=2357
-  _USERAPPIDSET._serialized_start=2359
-  _USERAPPIDSET._serialized_end=2406
-  _PATCHACTION._serialized_start=2408
-  _PATCHACTION._serialized_end=2482
-  _CONCEPT._serialized_start=2485
-  _CONCEPT._serialized_end=2782
-  _KEYPOINTINFO._serialized_start=2784
-  _KEYPOINTINFO._serialized_end=2868
-  _KEYPOINTEDGE._serialized_start=2870
-  _KEYPOINTEDGE._serialized_end=2908
-  _CONCEPTCOUNT._serialized_start=2911
-  _CONCEPTCOUNT._serialized_end=3075
-  _CONCEPTTYPECOUNT._serialized_start=3077
-  _CONCEPTTYPECOUNT._serialized_end=3143
-  _DETAILCONCEPTCOUNT._serialized_start=3146
-  _DETAILCONCEPTCOUNT._serialized_end=3369
-  _CONCEPTQUERY._serialized_start=3371
-  _CONCEPTQUERY._serialized_end=3438
-  _CONCEPTRELATION._serialized_start=3441
-  _CONCEPTRELATION._serialized_end=3658
-  _KNOWLEDGEGRAPH._serialized_start=3660
-  _KNOWLEDGEGRAPH._serialized_end=3781
-  _CONCEPTMAPPINGJOB._serialized_start=3783
-  _CONCEPTMAPPINGJOB._serialized_end=3851
-  _CONCEPTLANGUAGE._serialized_start=3853
-  _CONCEPTLANGUAGE._serialized_end=3916
-  _DATA._serialized_start=3919
-  _DATA._serialized_end=4553
-  _REGION._serialized_start=4556
-  _REGION._serialized_end=4690
-  _REGIONINFO._serialized_start=4693
-  _REGIONINFO._serialized_end=4995
-  _BOUNDINGBOX._serialized_start=4997
-  _BOUNDINGBOX._serialized_end=5108
-  _FRAMEINFO._serialized_start=5110
-  _FRAMEINFO._serialized_end=5162
-  _FRAME._serialized_start=5164
-  _FRAME._serialized_end=5262
-  _MASK._serialized_start=5264
-  _MASK._serialized_end=5312
-  _POLYGON._serialized_start=5314
-  _POLYGON._serialized_end=5360
-  _POINT._serialized_start=5363
-  _POINT._serialized_end=5545
-  _POINT_VISIBILITY._serialized_start=5473
-  _POINT_VISIBILITY._serialized_end=5545
-  _SPAN._serialized_start=5547
-  _SPAN._serialized_end=5621
-  _TOKEN._serialized_start=5623
-  _TOKEN._serialized_end=5698
-  _EMBEDDING._serialized_start=5700
-  _EMBEDDING._serialized_end=5755
-  _GEOPOINT._serialized_start=5757
-  _GEOPOINT._serialized_end=5816
-  _GEOLIMIT._serialized_start=5818
-  _GEOLIMIT._serialized_end=5863
-  _GEOBOXEDPOINT._serialized_start=5865
-  _GEOBOXEDPOINT._serialized_end=5923
-  _GEO._serialized_start=5926
-  _GEO._serialized_end=6063
-  _IMAGE._serialized_start=6066
-  _IMAGE._serialized_end=6223
-  _IMAGEINFO._serialized_start=6225
-  _IMAGEINFO._serialized_end=6303
-  _HOSTEDURL._serialized_start=6305
-  _HOSTEDURL._serialized_end=6384
-  _INPUT._serialized_start=6387
-  _INPUT._serialized_end=6609
-  _INPUTBATCH._serialized_start=6611
-  _INPUTBATCH._serialized_end=6660
-  _INPUTCOUNT._serialized_start=6663
-  _INPUTCOUNT._serialized_end=6881
-  _DATASET._serialized_start=6884
-  _DATASET._serialized_end=7286
-  _ANNOTATIONFILTER._serialized_start=7289
-  _ANNOTATIONFILTER._serialized_end=7505
-  _DATASETINPUT._serialized_start=7507
-  _DATASETINPUT._serialized_end=7605
-  _DATASETVERSION._serialized_start=7608
-  _DATASETVERSION._serialized_end=8353
-  _DATASETVERSION_METRICSENTRY._serialized_start=8237
-  _DATASETVERSION_METRICSENTRY._serialized_end=8320
-  _ANNOTATIONFILTERCONFIG._serialized_start=8355
-  _ANNOTATIONFILTERCONFIG._serialized_end=8467
-  _MODELPREDICTCONFIG._serialized_start=8469
-  _MODELPREDICTCONFIG._serialized_end=8525
-  _DATASETVERSIONMETRICS._serialized_start=8528
-  _DATASETVERSIONMETRICS._serialized_end=9619
-  _DATASETVERSIONMETRICSGROUP._serialized_start=9622
-  _DATASETVERSIONMETRICSGROUP._serialized_end=9824
-  _DATASETVERSIONEXPORTINFO._serialized_start=9827
-  _DATASETVERSIONEXPORTINFO._serialized_end=10035
-  _DATASETVERSIONEXPORT._serialized_start=10038
-  _DATASETVERSIONEXPORT._serialized_end=10218
-  _WORKFLOWRESULTSSIMILARITY._serialized_start=10220
-  _WORKFLOWRESULTSSIMILARITY._serialized_end=10330
-  _KEY._serialized_start=10333
-  _KEY._serialized_end=10577
-  _MODEL._serialized_start=10580
-  _MODEL._serialized_end=11564
-  _MODELREFERENCE._serialized_start=11566
-  _MODELREFERENCE._serialized_end=11682
-  _MODELVERSIONINPUTEXAMPLE._serialized_start=11685
-  _MODELVERSIONINPUTEXAMPLE._serialized_end=11836
-  _OUTPUTINFO._serialized_start=11839
-  _OUTPUTINFO._serialized_end=12051
-  _INPUTINFO._serialized_start=12053
-  _INPUTINFO._serialized_end=12150
-  _TRAININFO._serialized_start=12152
-  _TRAININFO._serialized_end=12204
-  _EVALINFO._serialized_start=12206
-  _EVALINFO._serialized_end=12257
-  _IMPORTINFO._serialized_start=12259
-  _IMPORTINFO._serialized_end=12312
-  _OUTPUTCONFIG._serialized_start=12315
-  _OUTPUTCONFIG._serialized_end=12828
-  _MODELTYPE._serialized_start=12831
-  _MODELTYPE._serialized_end=13297
-  _MODELLAYERINFO._serialized_start=13300
-  _MODELLAYERINFO._serialized_end=13437
-  _TRITONCONDAENVINFO._serialized_start=13439
-  _TRITONCONDAENVINFO._serialized_end=13507
-  _LAYERSHAPE._serialized_start=13509
-  _LAYERSHAPE._serialized_end=13617
-  _MODELTYPEFIELD._serialized_start=13620
-  _MODELTYPEFIELD._serialized_end=14342
-  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_start=13985
-  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_end=14342
-  _MODELTYPERANGEINFO._serialized_start=14344
-  _MODELTYPERANGEINFO._serialized_end=14404
-  _MODELTYPEENUMOPTION._serialized_start=14407
-  _MODELTYPEENUMOPTION._serialized_end=14619
-  _MODELTYPEENUMOPTIONALIAS._serialized_start=14621
-  _MODELTYPEENUMOPTIONALIAS._serialized_end=14688
-  _MODELQUERY._serialized_start=14690
-  _MODELQUERY._serialized_end=14745
-  _MODELVERSION._serialized_start=14748
-  _MODELVERSION._serialized_end=15512
-  _PRETRAINEDMODELCONFIG._serialized_start=15515
-  _PRETRAINEDMODELCONFIG._serialized_end=15676
-  _TRAINSTATS._serialized_start=15678
-  _TRAINSTATS._serialized_end=15740
-  _LOSSCURVEENTRY._serialized_start=15742
-  _LOSSCURVEENTRY._serialized_end=15808
-  _LABELCOUNT._serialized_start=15810
-  _LABELCOUNT._serialized_end=15859
-  _LABELDISTRIBUTION._serialized_start=15861
-  _LABELDISTRIBUTION._serialized_end=15937
-  _COOCCURRENCEMATRIXENTRY._serialized_start=15939
-  _COOCCURRENCEMATRIXENTRY._serialized_end=16005
-  _COOCCURRENCEMATRIX._serialized_start=16007
-  _COOCCURRENCEMATRIX._serialized_end=16103
-  _CONFUSIONMATRIXENTRY._serialized_start=16105
-  _CONFUSIONMATRIXENTRY._serialized_end=16183
-  _CONFUSIONMATRIX._serialized_start=16185
-  _CONFUSIONMATRIX._serialized_end=16275
-  _ROC._serialized_start=16277
-  _ROC._serialized_end=16393
-  _PRECISIONRECALLCURVE._serialized_start=16395
-  _PRECISIONRECALLCURVE._serialized_end=16490
-  _BINARYMETRICS._serialized_start=16493
-  _BINARYMETRICS._serialized_end=16855
-  _TRACKERMETRICS._serialized_start=16858
-  _TRACKERMETRICS._serialized_end=17003
-  _EVALTESTSETENTRY._serialized_start=17006
-  _EVALTESTSETENTRY._serialized_end=17244
-  _LOPQEVALRESULT._serialized_start=17247
-  _LOPQEVALRESULT._serialized_end=17452
-  _METRICSSUMMARY._serialized_start=17455
-  _METRICSSUMMARY._serialized_end=17851
-  _EVALMETRICS._serialized_start=17854
-  _EVALMETRICS._serialized_end=18456
-  _FIELDSVALUE._serialized_start=18459
-  _FIELDSVALUE._serialized_end=18642
-  _OUTPUT._serialized_start=18645
-  _OUTPUT._serialized_end=18864
-  _SCOPEDEPS._serialized_start=18866
-  _SCOPEDEPS._serialized_end=18918
-  _ENDPOINTDEPS._serialized_start=18920
-  _ENDPOINTDEPS._serialized_end=18978
-  _HIT._serialized_start=18981
-  _HIT._serialized_end=19122
-  _AND._serialized_start=19125
-  _AND._serialized_end=19266
-  _QUERY._serialized_start=19269
-  _QUERY._serialized_end=19405
-  _SEARCH._serialized_start=19408
-  _SEARCH._serialized_end=19878
-  _SEARCH_METRIC._serialized_start=19805
-  _SEARCH_METRIC._serialized_end=19878
-  _FILTER._serialized_start=19881
-  _FILTER._serialized_end=20045
-  _TIMERANGE._serialized_start=20047
-  _TIMERANGE._serialized_end=20152
-  _RANK._serialized_start=20154
-  _RANK._serialized_end=20222
-  _ANNOTATIONSEARCHMETRICS._serialized_start=20225
-  _ANNOTATIONSEARCHMETRICS._serialized_end=20494
-  _TEXT._serialized_start=20497
-  _TEXT._serialized_end=20642
-  _TEXTINFO._serialized_start=20644
-  _TEXTINFO._serialized_end=20692
-  _USER._serialized_start=20695
-  _USER._serialized_end=21459
-  _USERDETAIL._serialized_start=21462
-  _USERDETAIL._serialized_end=21927
-  _EMAILADDRESS._serialized_start=21929
-  _EMAILADDRESS._serialized_end=22011
-  _PASSWORD._serialized_start=22013
-  _PASSWORD._serialized_end=22042
-  _PASSWORDVIOLATIONS._serialized_start=22045
-  _PASSWORDVIOLATIONS._serialized_end=22435
-  _VIDEO._serialized_start=22438
-  _VIDEO._serialized_end=22612
-  _VIDEOINFO._serialized_start=22615
-  _VIDEOINFO._serialized_end=22757
-  _WORKFLOW._serialized_start=22760
-  _WORKFLOW._serialized_end=23223
-  _WORKFLOWVERSION._serialized_start=23226
-  _WORKFLOWVERSION._serialized_end=23576
-  _WORKFLOWNODE._serialized_start=23579
-  _WORKFLOWNODE._serialized_end=23768
-  _NODEINPUT._serialized_start=23770
-  _NODEINPUT._serialized_end=23798
-  _WORKFLOWRESULT._serialized_start=23801
-  _WORKFLOWRESULT._serialized_end=24058
-  _WORKFLOWSTATE._serialized_start=24060
-  _WORKFLOWSTATE._serialized_end=24087
-  _APPDUPLICATION._serialized_start=24090
-  _APPDUPLICATION._serialized_end=24434
-  _APPCOPYPROGRESS._serialized_start=24436
-  _APPCOPYPROGRESS._serialized_end=24483
-  _APPDUPLICATIONFILTERS._serialized_start=24486
-  _APPDUPLICATIONFILTERS._serialized_end=24624
-  _LABELORDER._serialized_start=24627
-  _LABELORDER._serialized_end=25005
-  _TASK._serialized_start=25008
-  _TASK._serialized_end=25749
-  _TASK_TASKTYPE._serialized_start=25641
-  _TASK_TASKTYPE._serialized_end=25749
-  _AIASSISTPARAMETERS._serialized_start=25751
-  _AIASSISTPARAMETERS._serialized_end=25847
-  _TASKWORKER._serialized_start=25850
-  _TASKWORKER._serialized_end=26169
-  _TASKWORKER_TASKWORKERSTRATEGY._serialized_start=26070
-  _TASKWORKER_TASKWORKERSTRATEGY._serialized_end=26152
-  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_start=26172
-  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_end=26469
-  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_start=26371
-  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_end=26469
-  _TASKINPUTSOURCE._serialized_start=26472
-  _TASKINPUTSOURCE._serialized_end=26667
-  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_start=26568
-  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_end=26667
-  _TASKREVIEW._serialized_start=26670
-  _TASKREVIEW._serialized_end=27070
-  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_start=26962
-  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_end=27053
-  _TASKREVIEWMANUALSTRATEGYINFO._serialized_start=27072
-  _TASKREVIEWMANUALSTRATEGYINFO._serialized_end=27129
-  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_start=27131
-  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_end=27198
-  _TASKAIASSISTANT._serialized_start=27200
-  _TASKAIASSISTANT._serialized_end=27238
-  _TASKSTATUSCOUNTPERUSER._serialized_start=27241
-  _TASKSTATUSCOUNTPERUSER._serialized_end=27429
-  _COLLECTOR._serialized_start=27432
-  _COLLECTOR._serialized_end=27689
-  _COLLECTORSOURCE._serialized_start=27691
-  _COLLECTORSOURCE._serialized_end=27807
-  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_start=27810
-  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_end=27963
-  _STATVALUE._serialized_start=27965
-  _STATVALUE._serialized_end=28047
-  _STATVALUEAGGREGATERESULT._serialized_start=28050
-  _STATVALUEAGGREGATERESULT._serialized_end=28216
-  _STATVALUEAGGREGATE._serialized_start=28218
-  _STATVALUEAGGREGATE._serialized_end=28334
-  _STATVALUEAGGREGATEQUERY._serialized_start=28337
-  _STATVALUEAGGREGATEQUERY._serialized_end=28610
-  _DATASETINPUTSSEARCHADDJOB._serialized_start=28613
-  _DATASETINPUTSSEARCHADDJOB._serialized_end=28852
-  _PCAPROJECTIONCOMPARATOR._serialized_start=28854
-  _PCAPROJECTIONCOMPARATOR._serialized_end=28933
-  _DUPLICATEANNOTATIONSRESULTS._serialized_start=28935
-  _DUPLICATEANNOTATIONSRESULTS._serialized_end=29010
-  _VISIBILITY._serialized_start=29013
-  _VISIBILITY._serialized_end=29148
-  _VISIBILITY_GETTABLE._serialized_start=29080
-  _VISIBILITY_GETTABLE._serialized_end=29148
-  _TRENDINGMETRIC._serialized_start=29150
-  _TRENDINGMETRIC._serialized_end=29238
-  _FULLTAG._serialized_start=29240
-  _FULLTAG._serialized_end=29275
-  _TIMESEGMENT._serialized_start=29277
-  _TIMESEGMENT._serialized_end=29379
-  _TIMEINFO._serialized_start=29381
-  _TIMEINFO._serialized_end=29449
-  _MODULE._serialized_start=29452
-  _MODULE._serialized_end=29771
-  _MODULEVERSION._serialized_start=29774
-  _MODULEVERSION._serialized_end=30348
-  _MODULEVERSION_MODULESUBNAV._serialized_start=30178
-  _MODULEVERSION_MODULESUBNAV._serialized_end=30247
-  _MODULEVERSION_MODULENAV._serialized_start=30249
-  _MODULEVERSION_MODULENAV._serialized_end=30342
-  _INSTALLEDMODULEVERSION._serialized_start=30351
-  _INSTALLEDMODULEVERSION._serialized_end=30652
-  _BULKOPERATION._serialized_start=30655
-  _BULKOPERATION._serialized_end=31052
-  _INPUTIDS._serialized_start=31054
-  _INPUTIDS._serialized_end=31083
-  _PROGRESS._serialized_start=31085
-  _PROGRESS._serialized_end=31141
-  _OPERATION._serialized_start=31144
-  _OPERATION._serialized_end=31548
-  _ADDCONCEPTS._serialized_start=31550
-  _ADDCONCEPTS._serialized_end=31604
-  _DELETECONCEPTS._serialized_start=31606
-  _DELETECONCEPTS._serialized_end=31681
-  _ADDMETADATA._serialized_start=31683
-  _ADDMETADATA._serialized_end=31739
-  _DELETEMETADATA._serialized_start=31741
-  _DELETEMETADATA._serialized_end=31800
-  _OVERWRITEGEO._serialized_start=31802
-  _OVERWRITEGEO._serialized_end=31848
-  _DELETEGEO._serialized_start=31850
-  _DELETEGEO._serialized_end=31861
-  _DELETEFROMDATASET._serialized_start=31863
-  _DELETEFROMDATASET._serialized_end=31902
-  _INPUTSADDJOB._serialized_start=31905
-  _INPUTSADDJOB._serialized_end=32239
-  _INPUTSADDJOBPROGRESS._serialized_start=32241
-  _INPUTSADDJOBPROGRESS._serialized_end=32358
-  _UPLOAD._serialized_start=32361
-  _UPLOAD._serialized_end=32638
-  _UPLOADCONTENTPART._serialized_start=32640
-  _UPLOADCONTENTPART._serialized_end=32715
-  _CUSTOMCODEOPERATORREQUEST._serialized_start=32717
-  _CUSTOMCODEOPERATORREQUEST._serialized_end=32825
-  _INPUTSEXTRACTIONJOB._serialized_start=32828
-  _INPUTSEXTRACTIONJOB._serialized_end=33077
-  _INPUTSEXTRACTIONJOBPROGRESS._serialized_start=33080
-  _INPUTSEXTRACTIONJOBPROGRESS._serialized_end=33248
-  _INPUTSDATASOURCE._serialized_start=33250
-  _INPUTSDATASOURCE._serialized_end=33337
-  _DATASOURCEURL._serialized_start=33339
-  _DATASOURCEURL._serialized_end=33425
-  _DATASOURCECREDENTIALS._serialized_start=33428
-  _DATASOURCECREDENTIALS._serialized_end=33595
-  _AWSCREDS._serialized_start=33597
-  _AWSCREDS._serialized_end=33672
-  _AZUREBLOBCREDS._serialized_start=33674
-  _AZUREBLOBCREDS._serialized_end=33733
-  _INPUTSUPLOAD._serialized_start=33735
-  _INPUTSUPLOAD._serialized_end=33831
+  _APP._serialized_end=1340
+  _APPQUERY._serialized_start=1342
+  _APPQUERY._serialized_end=1366
+  _COLLABORATOR._serialized_start=1369
+  _COLLABORATOR._serialized_end=1641
+  _COLLABORATION._serialized_start=1644
+  _COLLABORATION._serialized_end=1813
+  _AUDIO._serialized_start=1816
+  _AUDIO._serialized_end=1967
+  _AUDIOINFO._serialized_start=1969
+  _AUDIOINFO._serialized_end=2067
+  _TRACK._serialized_start=2069
+  _TRACK._serialized_end=2188
+  _CLUSTER._serialized_start=2190
+  _CLUSTER._serialized_end=2294
+  _COLOR._serialized_start=2296
+  _COLOR._serialized_end=2373
+  _W3C._serialized_start=2375
+  _W3C._serialized_end=2407
+  _USERAPPIDSET._serialized_start=2409
+  _USERAPPIDSET._serialized_end=2456
+  _PATCHACTION._serialized_start=2458
+  _PATCHACTION._serialized_end=2532
+  _CONCEPT._serialized_start=2535
+  _CONCEPT._serialized_end=2832
+  _KEYPOINTINFO._serialized_start=2834
+  _KEYPOINTINFO._serialized_end=2918
+  _KEYPOINTEDGE._serialized_start=2920
+  _KEYPOINTEDGE._serialized_end=2958
+  _CONCEPTCOUNT._serialized_start=2961
+  _CONCEPTCOUNT._serialized_end=3125
+  _CONCEPTTYPECOUNT._serialized_start=3127
+  _CONCEPTTYPECOUNT._serialized_end=3193
+  _DETAILCONCEPTCOUNT._serialized_start=3196
+  _DETAILCONCEPTCOUNT._serialized_end=3419
+  _CONCEPTQUERY._serialized_start=3421
+  _CONCEPTQUERY._serialized_end=3488
+  _CONCEPTRELATION._serialized_start=3491
+  _CONCEPTRELATION._serialized_end=3708
+  _KNOWLEDGEGRAPH._serialized_start=3710
+  _KNOWLEDGEGRAPH._serialized_end=3831
+  _CONCEPTMAPPINGJOB._serialized_start=3833
+  _CONCEPTMAPPINGJOB._serialized_end=3901
+  _CONCEPTLANGUAGE._serialized_start=3903
+  _CONCEPTLANGUAGE._serialized_end=3966
+  _DATA._serialized_start=3969
+  _DATA._serialized_end=4603
+  _REGION._serialized_start=4606
+  _REGION._serialized_end=4740
+  _REGIONINFO._serialized_start=4743
+  _REGIONINFO._serialized_end=5045
+  _BOUNDINGBOX._serialized_start=5047
+  _BOUNDINGBOX._serialized_end=5158
+  _FRAMEINFO._serialized_start=5160
+  _FRAMEINFO._serialized_end=5212
+  _FRAME._serialized_start=5214
+  _FRAME._serialized_end=5312
+  _MASK._serialized_start=5314
+  _MASK._serialized_end=5362
+  _POLYGON._serialized_start=5364
+  _POLYGON._serialized_end=5410
+  _POINT._serialized_start=5413
+  _POINT._serialized_end=5595
+  _POINT_VISIBILITY._serialized_start=5523
+  _POINT_VISIBILITY._serialized_end=5595
+  _SPAN._serialized_start=5597
+  _SPAN._serialized_end=5671
+  _TOKEN._serialized_start=5673
+  _TOKEN._serialized_end=5748
+  _EMBEDDING._serialized_start=5750
+  _EMBEDDING._serialized_end=5805
+  _GEOPOINT._serialized_start=5807
+  _GEOPOINT._serialized_end=5866
+  _GEOLIMIT._serialized_start=5868
+  _GEOLIMIT._serialized_end=5913
+  _GEOBOXEDPOINT._serialized_start=5915
+  _GEOBOXEDPOINT._serialized_end=5973
+  _GEO._serialized_start=5976
+  _GEO._serialized_end=6113
+  _IMAGE._serialized_start=6116
+  _IMAGE._serialized_end=6273
+  _IMAGEINFO._serialized_start=6275
+  _IMAGEINFO._serialized_end=6353
+  _HOSTEDURL._serialized_start=6355
+  _HOSTEDURL._serialized_end=6434
+  _INPUT._serialized_start=6437
+  _INPUT._serialized_end=6659
+  _INPUTBATCH._serialized_start=6661
+  _INPUTBATCH._serialized_end=6710
+  _INPUTCOUNT._serialized_start=6713
+  _INPUTCOUNT._serialized_end=6931
+  _DATASET._serialized_start=6934
+  _DATASET._serialized_end=7336
+  _ANNOTATIONFILTER._serialized_start=7339
+  _ANNOTATIONFILTER._serialized_end=7555
+  _DATASETINPUT._serialized_start=7557
+  _DATASETINPUT._serialized_end=7655
+  _DATASETVERSION._serialized_start=7658
+  _DATASETVERSION._serialized_end=8403
+  _DATASETVERSION_METRICSENTRY._serialized_start=8287
+  _DATASETVERSION_METRICSENTRY._serialized_end=8370
+  _ANNOTATIONFILTERCONFIG._serialized_start=8405
+  _ANNOTATIONFILTERCONFIG._serialized_end=8517
+  _MODELPREDICTCONFIG._serialized_start=8519
+  _MODELPREDICTCONFIG._serialized_end=8575
+  _DATASETVERSIONMETRICS._serialized_start=8578
+  _DATASETVERSIONMETRICS._serialized_end=9669
+  _DATASETVERSIONMETRICSGROUP._serialized_start=9672
+  _DATASETVERSIONMETRICSGROUP._serialized_end=9874
+  _DATASETVERSIONEXPORTINFO._serialized_start=9877
+  _DATASETVERSIONEXPORTINFO._serialized_end=10085
+  _DATASETVERSIONEXPORT._serialized_start=10088
+  _DATASETVERSIONEXPORT._serialized_end=10268
+  _WORKFLOWRESULTSSIMILARITY._serialized_start=10270
+  _WORKFLOWRESULTSSIMILARITY._serialized_end=10380
+  _KEY._serialized_start=10383
+  _KEY._serialized_end=10627
+  _MODEL._serialized_start=10630
+  _MODEL._serialized_end=11614
+  _MODELREFERENCE._serialized_start=11616
+  _MODELREFERENCE._serialized_end=11732
+  _MODELVERSIONINPUTEXAMPLE._serialized_start=11735
+  _MODELVERSIONINPUTEXAMPLE._serialized_end=11886
+  _OUTPUTINFO._serialized_start=11889
+  _OUTPUTINFO._serialized_end=12101
+  _INPUTINFO._serialized_start=12103
+  _INPUTINFO._serialized_end=12200
+  _TRAININFO._serialized_start=12202
+  _TRAININFO._serialized_end=12254
+  _EVALINFO._serialized_start=12256
+  _EVALINFO._serialized_end=12307
+  _IMPORTINFO._serialized_start=12309
+  _IMPORTINFO._serialized_end=12362
+  _OUTPUTCONFIG._serialized_start=12365
+  _OUTPUTCONFIG._serialized_end=12878
+  _MODELTYPE._serialized_start=12881
+  _MODELTYPE._serialized_end=13347
+  _MODELLAYERINFO._serialized_start=13350
+  _MODELLAYERINFO._serialized_end=13487
+  _TRITONCONDAENVINFO._serialized_start=13489
+  _TRITONCONDAENVINFO._serialized_end=13557
+  _LAYERSHAPE._serialized_start=13559
+  _LAYERSHAPE._serialized_end=13667
+  _MODELTYPEFIELD._serialized_start=13670
+  _MODELTYPEFIELD._serialized_end=14392
+  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_start=14035
+  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_end=14392
+  _MODELTYPERANGEINFO._serialized_start=14394
+  _MODELTYPERANGEINFO._serialized_end=14454
+  _MODELTYPEENUMOPTION._serialized_start=14457
+  _MODELTYPEENUMOPTION._serialized_end=14669
+  _MODELTYPEENUMOPTIONALIAS._serialized_start=14671
+  _MODELTYPEENUMOPTIONALIAS._serialized_end=14738
+  _MODELQUERY._serialized_start=14740
+  _MODELQUERY._serialized_end=14795
+  _MODELVERSION._serialized_start=14798
+  _MODELVERSION._serialized_end=15562
+  _PRETRAINEDMODELCONFIG._serialized_start=15565
+  _PRETRAINEDMODELCONFIG._serialized_end=15726
+  _TRAINSTATS._serialized_start=15728
+  _TRAINSTATS._serialized_end=15790
+  _LOSSCURVEENTRY._serialized_start=15792
+  _LOSSCURVEENTRY._serialized_end=15858
+  _LABELCOUNT._serialized_start=15860
+  _LABELCOUNT._serialized_end=15909
+  _LABELDISTRIBUTION._serialized_start=15911
+  _LABELDISTRIBUTION._serialized_end=15987
+  _COOCCURRENCEMATRIXENTRY._serialized_start=15989
+  _COOCCURRENCEMATRIXENTRY._serialized_end=16055
+  _COOCCURRENCEMATRIX._serialized_start=16057
+  _COOCCURRENCEMATRIX._serialized_end=16153
+  _CONFUSIONMATRIXENTRY._serialized_start=16155
+  _CONFUSIONMATRIXENTRY._serialized_end=16233
+  _CONFUSIONMATRIX._serialized_start=16235
+  _CONFUSIONMATRIX._serialized_end=16325
+  _ROC._serialized_start=16327
+  _ROC._serialized_end=16443
+  _PRECISIONRECALLCURVE._serialized_start=16445
+  _PRECISIONRECALLCURVE._serialized_end=16540
+  _BINARYMETRICS._serialized_start=16543
+  _BINARYMETRICS._serialized_end=16905
+  _TRACKERMETRICS._serialized_start=16908
+  _TRACKERMETRICS._serialized_end=17053
+  _EVALTESTSETENTRY._serialized_start=17056
+  _EVALTESTSETENTRY._serialized_end=17294
+  _LOPQEVALRESULT._serialized_start=17297
+  _LOPQEVALRESULT._serialized_end=17502
+  _METRICSSUMMARY._serialized_start=17505
+  _METRICSSUMMARY._serialized_end=17901
+  _EVALMETRICS._serialized_start=17904
+  _EVALMETRICS._serialized_end=18506
+  _FIELDSVALUE._serialized_start=18509
+  _FIELDSVALUE._serialized_end=18692
+  _OUTPUT._serialized_start=18695
+  _OUTPUT._serialized_end=18914
+  _SCOPEDEPS._serialized_start=18916
+  _SCOPEDEPS._serialized_end=18968
+  _ENDPOINTDEPS._serialized_start=18970
+  _ENDPOINTDEPS._serialized_end=19028
+  _HIT._serialized_start=19031
+  _HIT._serialized_end=19172
+  _HITCOUNT._serialized_start=19174
+  _HITCOUNT._serialized_end=19209
+  _AND._serialized_start=19212
+  _AND._serialized_end=19353
+  _QUERY._serialized_start=19356
+  _QUERY._serialized_end=19492
+  _SEARCH._serialized_start=19495
+  _SEARCH._serialized_end=19965
+  _SEARCH_METRIC._serialized_start=19892
+  _SEARCH_METRIC._serialized_end=19965
+  _FILTER._serialized_start=19968
+  _FILTER._serialized_end=20132
+  _TIMERANGE._serialized_start=20134
+  _TIMERANGE._serialized_end=20239
+  _RANK._serialized_start=20241
+  _RANK._serialized_end=20309
+  _ANNOTATIONSEARCHMETRICS._serialized_start=20312
+  _ANNOTATIONSEARCHMETRICS._serialized_end=20581
+  _TEXT._serialized_start=20584
+  _TEXT._serialized_end=20729
+  _TEXTINFO._serialized_start=20731
+  _TEXTINFO._serialized_end=20779
+  _USER._serialized_start=20782
+  _USER._serialized_end=21546
+  _USERDETAIL._serialized_start=21549
+  _USERDETAIL._serialized_end=22014
+  _EMAILADDRESS._serialized_start=22016
+  _EMAILADDRESS._serialized_end=22098
+  _PASSWORD._serialized_start=22100
+  _PASSWORD._serialized_end=22129
+  _PASSWORDVIOLATIONS._serialized_start=22132
+  _PASSWORDVIOLATIONS._serialized_end=22522
+  _VIDEO._serialized_start=22525
+  _VIDEO._serialized_end=22699
+  _VIDEOINFO._serialized_start=22702
+  _VIDEOINFO._serialized_end=22844
+  _WORKFLOW._serialized_start=22847
+  _WORKFLOW._serialized_end=23310
+  _WORKFLOWVERSION._serialized_start=23313
+  _WORKFLOWVERSION._serialized_end=23663
+  _WORKFLOWNODE._serialized_start=23666
+  _WORKFLOWNODE._serialized_end=23855
+  _NODEINPUT._serialized_start=23857
+  _NODEINPUT._serialized_end=23885
+  _WORKFLOWRESULT._serialized_start=23888
+  _WORKFLOWRESULT._serialized_end=24145
+  _WORKFLOWSTATE._serialized_start=24147
+  _WORKFLOWSTATE._serialized_end=24174
+  _APPDUPLICATION._serialized_start=24177
+  _APPDUPLICATION._serialized_end=24521
+  _APPCOPYPROGRESS._serialized_start=24523
+  _APPCOPYPROGRESS._serialized_end=24570
+  _APPDUPLICATIONFILTERS._serialized_start=24573
+  _APPDUPLICATIONFILTERS._serialized_end=24711
+  _LABELORDER._serialized_start=24714
+  _LABELORDER._serialized_end=25092
+  _TASK._serialized_start=25095
+  _TASK._serialized_end=25836
+  _TASK_TASKTYPE._serialized_start=25728
+  _TASK_TASKTYPE._serialized_end=25836
+  _AIASSISTPARAMETERS._serialized_start=25838
+  _AIASSISTPARAMETERS._serialized_end=25934
+  _TASKWORKER._serialized_start=25937
+  _TASKWORKER._serialized_end=26256
+  _TASKWORKER_TASKWORKERSTRATEGY._serialized_start=26157
+  _TASKWORKER_TASKWORKERSTRATEGY._serialized_end=26239
+  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_start=26259
+  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_end=26556
+  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_start=26458
+  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_end=26556
+  _TASKINPUTSOURCE._serialized_start=26559
+  _TASKINPUTSOURCE._serialized_end=26754
+  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_start=26655
+  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_end=26754
+  _TASKREVIEW._serialized_start=26757
+  _TASKREVIEW._serialized_end=27157
+  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_start=27049
+  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_end=27140
+  _TASKREVIEWMANUALSTRATEGYINFO._serialized_start=27159
+  _TASKREVIEWMANUALSTRATEGYINFO._serialized_end=27216
+  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_start=27218
+  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_end=27285
+  _TASKAIASSISTANT._serialized_start=27287
+  _TASKAIASSISTANT._serialized_end=27325
+  _TASKSTATUSCOUNTPERUSER._serialized_start=27328
+  _TASKSTATUSCOUNTPERUSER._serialized_end=27516
+  _COLLECTOR._serialized_start=27519
+  _COLLECTOR._serialized_end=27776
+  _COLLECTORSOURCE._serialized_start=27778
+  _COLLECTORSOURCE._serialized_end=27894
+  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_start=27897
+  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_end=28050
+  _STATVALUE._serialized_start=28052
+  _STATVALUE._serialized_end=28134
+  _STATVALUEAGGREGATERESULT._serialized_start=28137
+  _STATVALUEAGGREGATERESULT._serialized_end=28303
+  _STATVALUEAGGREGATE._serialized_start=28305
+  _STATVALUEAGGREGATE._serialized_end=28421
+  _STATVALUEAGGREGATEQUERY._serialized_start=28424
+  _STATVALUEAGGREGATEQUERY._serialized_end=28697
+  _DATASETINPUTSSEARCHADDJOB._serialized_start=28700
+  _DATASETINPUTSSEARCHADDJOB._serialized_end=28939
+  _PCAPROJECTIONCOMPARATOR._serialized_start=28941
+  _PCAPROJECTIONCOMPARATOR._serialized_end=29020
+  _DUPLICATEANNOTATIONSRESULTS._serialized_start=29022
+  _DUPLICATEANNOTATIONSRESULTS._serialized_end=29097
+  _VISIBILITY._serialized_start=29100
+  _VISIBILITY._serialized_end=29235
+  _VISIBILITY_GETTABLE._serialized_start=29167
+  _VISIBILITY_GETTABLE._serialized_end=29235
+  _TRENDINGMETRIC._serialized_start=29237
+  _TRENDINGMETRIC._serialized_end=29325
+  _FULLTAG._serialized_start=29327
+  _FULLTAG._serialized_end=29362
+  _TIMESEGMENT._serialized_start=29364
+  _TIMESEGMENT._serialized_end=29466
+  _TIMEINFO._serialized_start=29468
+  _TIMEINFO._serialized_end=29536
+  _MODULE._serialized_start=29539
+  _MODULE._serialized_end=29858
+  _MODULEVERSION._serialized_start=29861
+  _MODULEVERSION._serialized_end=30435
+  _MODULEVERSION_MODULESUBNAV._serialized_start=30265
+  _MODULEVERSION_MODULESUBNAV._serialized_end=30334
+  _MODULEVERSION_MODULENAV._serialized_start=30336
+  _MODULEVERSION_MODULENAV._serialized_end=30429
+  _INSTALLEDMODULEVERSION._serialized_start=30438
+  _INSTALLEDMODULEVERSION._serialized_end=30739
+  _BULKOPERATION._serialized_start=30742
+  _BULKOPERATION._serialized_end=31139
+  _INPUTIDS._serialized_start=31141
+  _INPUTIDS._serialized_end=31170
+  _PROGRESS._serialized_start=31172
+  _PROGRESS._serialized_end=31228
+  _OPERATION._serialized_start=31231
+  _OPERATION._serialized_end=31689
+  _ADDCONCEPTS._serialized_start=31691
+  _ADDCONCEPTS._serialized_end=31745
+  _DELETECONCEPTS._serialized_start=31747
+  _DELETECONCEPTS._serialized_end=31822
+  _ADDMETADATA._serialized_start=31824
+  _ADDMETADATA._serialized_end=31880
+  _DELETEMETADATA._serialized_start=31882
+  _DELETEMETADATA._serialized_end=31941
+  _OVERWRITEGEO._serialized_start=31943
+  _OVERWRITEGEO._serialized_end=31989
+  _DELETEGEO._serialized_start=31991
+  _DELETEGEO._serialized_end=32002
+  _ADDTODATASET._serialized_start=32004
+  _ADDTODATASET._serialized_end=32038
+  _DELETEFROMDATASET._serialized_start=32040
+  _DELETEFROMDATASET._serialized_end=32079
+  _INPUTSADDJOB._serialized_start=32082
+  _INPUTSADDJOB._serialized_end=32416
+  _INPUTSADDJOBPROGRESS._serialized_start=32418
+  _INPUTSADDJOBPROGRESS._serialized_end=32535
+  _UPLOAD._serialized_start=32538
+  _UPLOAD._serialized_end=32815
+  _UPLOADCONTENTPART._serialized_start=32817
+  _UPLOADCONTENTPART._serialized_end=32892
+  _CUSTOMCODEOPERATORREQUEST._serialized_start=32894
+  _CUSTOMCODEOPERATORREQUEST._serialized_end=33002
+  _INPUTSEXTRACTIONJOB._serialized_start=33005
+  _INPUTSEXTRACTIONJOB._serialized_end=33254
+  _INPUTSEXTRACTIONJOBPROGRESS._serialized_start=33257
+  _INPUTSEXTRACTIONJOBPROGRESS._serialized_end=33558
+  _INPUTSDATASOURCE._serialized_start=33560
+  _INPUTSDATASOURCE._serialized_end=33647
+  _DATASOURCEURL._serialized_start=33649
+  _DATASOURCEURL._serialized_end=33735
+  _DATASOURCECREDENTIALS._serialized_start=33738
+  _DATASOURCECREDENTIALS._serialized_end=33905
+  _AWSCREDS._serialized_start=33907
+  _AWSCREDS._serialized_end=33982
+  _AZUREBLOBCREDS._serialized_start=33984
+  _AZUREBLOBCREDS._serialized_end=34043
+  _INPUTSUPLOAD._serialized_start=34045
+  _INPUTSUPLOAD._serialized_end=34141
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/resources_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/resources_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -491,14 +491,15 @@
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     DEFAULT_LANGUAGE_FIELD_NUMBER: builtins.int
     DEFAULT_WORKFLOW_ID_FIELD_NUMBER: builtins.int
+    DEFAULT_WORKFLOW_FIELD_NUMBER: builtins.int
     USER_ID_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     MODIFIED_AT_FIELD_NUMBER: builtins.int
     LEGAL_CONSENT_STATUS_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     SAMPLE_MS_FIELD_NUMBER: builtins.int
@@ -508,14 +509,17 @@
     STAR_COUNT_FIELD_NUMBER: builtins.int
     NOTES_FIELD_NUMBER: builtins.int
     IMAGE_FIELD_NUMBER: builtins.int
     id: builtins.str
     name: builtins.str
     default_language: builtins.str
     default_workflow_id: builtins.str
+    """Default workflow id deprecated in favor of default_workflow"""
+    @property
+    def default_workflow(self) -> global___Workflow: ...
     user_id: builtins.str
     """why is user_id present here when this message type is used in PostApps but completely ignored there? PostApp already
     specifies the userid in path but doesn't even actually use neither of userids, it instead used the id from auth context.
     This creates a lot of ambiguity, should always have different message types for Post/Get endpoints so that the minimum interface for each op can be described
     """
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
@@ -565,30 +569,31 @@
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         name: builtins.str = ...,
         default_language: builtins.str = ...,
         default_workflow_id: builtins.str = ...,
+        default_workflow: global___Workflow | None = ...,
         user_id: builtins.str = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         legal_consent_status: builtins.int = ...,
         metadata: google.protobuf.struct_pb2.Struct | None = ...,
         description: builtins.str = ...,
         sample_ms: builtins.int = ...,
         visibility: global___Visibility | None = ...,
         data_tier_id: builtins.str = ...,
         is_starred: builtins.bool = ...,
         star_count: builtins.int = ...,
         notes: builtins.str = ...,
         image: global___Image | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "image", b"image", "metadata", b"metadata", "modified_at", b"modified_at", "visibility", b"visibility"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "data_tier_id", b"data_tier_id", "default_language", b"default_language", "default_workflow_id", b"default_workflow_id", "description", b"description", "id", b"id", "image", b"image", "is_starred", b"is_starred", "legal_consent_status", b"legal_consent_status", "metadata", b"metadata", "modified_at", b"modified_at", "name", b"name", "notes", b"notes", "sample_ms", b"sample_ms", "star_count", b"star_count", "user_id", b"user_id", "visibility", b"visibility"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "default_workflow", b"default_workflow", "image", b"image", "metadata", b"metadata", "modified_at", b"modified_at", "visibility", b"visibility"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "data_tier_id", b"data_tier_id", "default_language", b"default_language", "default_workflow", b"default_workflow", "default_workflow_id", b"default_workflow_id", "description", b"description", "id", b"id", "image", b"image", "is_starred", b"is_starred", "legal_consent_status", b"legal_consent_status", "metadata", b"metadata", "modified_at", b"modified_at", "name", b"name", "notes", b"notes", "sample_ms", b"sample_ms", "star_count", b"star_count", "user_id", b"user_id", "visibility", b"visibility"]) -> None: ...
 
 global___App = App
 
 @typing_extensions.final
 class AppQuery(google.protobuf.message.Message):
     """App query"""
 
@@ -4591,14 +4596,30 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["annotation", b"annotation", "input", b"input"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["annotation", b"annotation", "app_id", b"app_id", "input", b"input", "score", b"score", "user_id", b"user_id"]) -> None: ...
 
 global___Hit = Hit
 
 @typing_extensions.final
+class HitCount(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ESTIMATED_TOTAL_FIELD_NUMBER: builtins.int
+    estimated_total: builtins.int
+    """The estimated total number of hits for the search query, not just the current page."""
+    def __init__(
+        self,
+        *,
+        estimated_total: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["estimated_total", b"estimated_total"]) -> None: ...
+
+global___HitCount = HitCount
+
+@typing_extensions.final
 class And(google.protobuf.message.Message):
     """This is the common building block of a query which is a sequence of And messages ANDed together.
     Note that some fields are used too RANK results (affect the scores) and some are used to FILTER
     results (unordered subset of your app's contents). In general, FILTER operations are more
     efficient queries at scale and when combined with RANK operations can speed up search performance
     as you effectively operate on a smaller sub-set of your entire app.
     """
@@ -7317,42 +7338,46 @@
     ADD_CONCEPTS_FIELD_NUMBER: builtins.int
     DELETE_CONCEPTS_FIELD_NUMBER: builtins.int
     ADD_METADATA_FIELD_NUMBER: builtins.int
     DELETE_METADATA_FIELD_NUMBER: builtins.int
     OVERWRITE_GEO_FIELD_NUMBER: builtins.int
     DELETE_GEO_FIELD_NUMBER: builtins.int
     DELETE_FROM_DATASET_FIELD_NUMBER: builtins.int
+    ADD_TO_DATASET_FIELD_NUMBER: builtins.int
     @property
     def add_concepts(self) -> global___AddConcepts: ...
     @property
     def delete_concepts(self) -> global___DeleteConcepts: ...
     @property
     def add_metadata(self) -> global___AddMetadata: ...
     @property
     def delete_metadata(self) -> global___DeleteMetadata: ...
     @property
     def overwrite_geo(self) -> global___OverwriteGeo: ...
     @property
     def delete_geo(self) -> global___DeleteGeo: ...
     @property
     def delete_from_dataset(self) -> global___DeleteFromDataset: ...
+    @property
+    def add_to_dataset(self) -> global___AddToDataset: ...
     def __init__(
         self,
         *,
         add_concepts: global___AddConcepts | None = ...,
         delete_concepts: global___DeleteConcepts | None = ...,
         add_metadata: global___AddMetadata | None = ...,
         delete_metadata: global___DeleteMetadata | None = ...,
         overwrite_geo: global___OverwriteGeo | None = ...,
         delete_geo: global___DeleteGeo | None = ...,
         delete_from_dataset: global___DeleteFromDataset | None = ...,
+        add_to_dataset: global___AddToDataset | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["add_concepts", b"add_concepts", "add_metadata", b"add_metadata", "delete_concepts", b"delete_concepts", "delete_from_dataset", b"delete_from_dataset", "delete_geo", b"delete_geo", "delete_metadata", b"delete_metadata", "operation", b"operation", "overwrite_geo", b"overwrite_geo"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["add_concepts", b"add_concepts", "add_metadata", b"add_metadata", "delete_concepts", b"delete_concepts", "delete_from_dataset", b"delete_from_dataset", "delete_geo", b"delete_geo", "delete_metadata", b"delete_metadata", "operation", b"operation", "overwrite_geo", b"overwrite_geo"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["operation", b"operation"]) -> typing_extensions.Literal["add_concepts", "delete_concepts", "add_metadata", "delete_metadata", "overwrite_geo", "delete_geo", "delete_from_dataset"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["add_concepts", b"add_concepts", "add_metadata", b"add_metadata", "add_to_dataset", b"add_to_dataset", "delete_concepts", b"delete_concepts", "delete_from_dataset", b"delete_from_dataset", "delete_geo", b"delete_geo", "delete_metadata", b"delete_metadata", "operation", b"operation", "overwrite_geo", b"overwrite_geo"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["add_concepts", b"add_concepts", "add_metadata", b"add_metadata", "add_to_dataset", b"add_to_dataset", "delete_concepts", b"delete_concepts", "delete_from_dataset", b"delete_from_dataset", "delete_geo", b"delete_geo", "delete_metadata", b"delete_metadata", "operation", b"operation", "overwrite_geo", b"overwrite_geo"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["operation", b"operation"]) -> typing_extensions.Literal["add_concepts", "delete_concepts", "add_metadata", "delete_metadata", "overwrite_geo", "delete_geo", "delete_from_dataset", "add_to_dataset"] | None: ...
 
 global___Operation = Operation
 
 @typing_extensions.final
 class AddConcepts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -7453,14 +7478,29 @@
     def __init__(
         self,
     ) -> None: ...
 
 global___DeleteGeo = DeleteGeo
 
 @typing_extensions.final
+class AddToDataset(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DATASET_ID_FIELD_NUMBER: builtins.int
+    dataset_id: builtins.str
+    def __init__(
+        self,
+        *,
+        dataset_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset_id", b"dataset_id"]) -> None: ...
+
+global___AddToDataset = AddToDataset
+
+@typing_extensions.final
 class DeleteFromDataset(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATASET_ID_FIELD_NUMBER: builtins.int
     dataset_id: builtins.str
     def __init__(
         self,
@@ -7708,29 +7748,41 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     READ_OBJECTS_COUNT_FIELD_NUMBER: builtins.int
     AUDIO_INPUTS_COUNT_FIELD_NUMBER: builtins.int
     IMAGE_INPUTS_COUNT_FIELD_NUMBER: builtins.int
     VIDEO_INPUTS_COUNT_FIELD_NUMBER: builtins.int
     TEXT_INPUTS_COUNT_FIELD_NUMBER: builtins.int
+    PENDING_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
+    IN_PROGRESS_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
+    COMPLETED_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
+    FAILED_ARCHIVES_COUNT_FIELD_NUMBER: builtins.int
     read_objects_count: builtins.int
     audio_inputs_count: builtins.int
     image_inputs_count: builtins.int
     video_inputs_count: builtins.int
     text_inputs_count: builtins.int
+    pending_archives_count: builtins.int
+    in_progress_archives_count: builtins.int
+    completed_archives_count: builtins.int
+    failed_archives_count: builtins.int
     def __init__(
         self,
         *,
         read_objects_count: builtins.int = ...,
         audio_inputs_count: builtins.int = ...,
         image_inputs_count: builtins.int = ...,
         video_inputs_count: builtins.int = ...,
         text_inputs_count: builtins.int = ...,
+        pending_archives_count: builtins.int = ...,
+        in_progress_archives_count: builtins.int = ...,
+        completed_archives_count: builtins.int = ...,
+        failed_archives_count: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["audio_inputs_count", b"audio_inputs_count", "image_inputs_count", b"image_inputs_count", "read_objects_count", b"read_objects_count", "text_inputs_count", b"text_inputs_count", "video_inputs_count", b"video_inputs_count"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["audio_inputs_count", b"audio_inputs_count", "completed_archives_count", b"completed_archives_count", "failed_archives_count", b"failed_archives_count", "image_inputs_count", b"image_inputs_count", "in_progress_archives_count", b"in_progress_archives_count", "pending_archives_count", b"pending_archives_count", "read_objects_count", b"read_objects_count", "text_inputs_count", b"text_inputs_count", "video_inputs_count", b"video_inputs_count"]) -> None: ...
 
 global___InputsExtractionJobProgress = InputsExtractionJobProgress
 
 @typing_extensions.final
 class InputsDataSource(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/service_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from clarifai_grpc.grpc.api.status import status_code_pb2 as proto_dot_clarifai_dot_api_dot_status_dot_status__code__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n proto/clarifai/api/service.proto\x12\x0c\x63larifai.api\x1a\"proto/clarifai/api/resources.proto\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/auth/scope/scope.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\",\n\nPagination\x12\x0c\n\x04page\x18\x01 \x01(\r\x12\x10\n\x08per_page\x18\x02 \x01(\r\"p\n\x14GetAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rannotation_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb7\x02\n\x16ListAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\x12\x10\n\x08user_ids\x18\t \x03(\t\x12\x19\n\x11model_version_ids\x18\n \x03(\t\x12-\n\x08statuses\x18\x05 \x03(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14list_all_annotations\x18\x06 \x01(\x08\x12\x1b\n\x13return_model_output\x18\x0c \x01(\x08\x12\x0c\n\x04page\x18\x07 \x01(\r\x12\x10\n\x08per_page\x18\x08 \x01(\r\x12\x0f\n\x07task_id\x18\x0b \x01(\tJ\x04\x08\x04\x10\x05\"x\n\x16PostAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\"\x89\x01\n\x17PatchAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\xb9\x01\n\x1dPatchAnnotationsStatusRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0bstatus_code\x18\x02 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\x12\x10\n\x08user_ids\x18\x03 \x03(\t\x12\x0f\n\x07task_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\"v\n\x1ePatchAnnotationsStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08user_ids\x18\x02 \x03(\t\x12\x15\n\rupdated_count\x18\x03 \x01(\r\"s\n\x17\x44\x65leteAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12\x15\n\rannotation_id\x18\x03 \x01(\t\"k\n\x18\x44\x65leteAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"u\n\x18SingleAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12,\n\nannotation\x18\x02 \x01(\x0b\x32\x18.clarifai.api.Annotation\"{\n\x17MultiAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.AnnotationB\x04\x80\xb5\x18\x01\"[\n\rGetAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"\xa5\x02\n\x0fListAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x16\n\x0csort_by_name\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x10\n\x04name\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\tB\t\n\x07sort_by\"c\n\x0fPostAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\"C\n\x10\x44\x65leteAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\xb9\x01\n\x10PatchAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\xb7\x01\n\x0fPatchAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\x81\x01\n\x13PatchAppsIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\xa3\x01\n\x17PostAppsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tapp_query\x18\x02 \x01(\x0b\x32\x16.clarifai.api.AppQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"`\n\x11SingleAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\"f\n\x10MultiAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.AppB\x04\x80\xb5\x18\x01\"\x8b\x01\n\x18ListCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x16list_all_collaborators\x18\x02 \x01(\x08\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x18PostCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\"\x8f\x01\n\x19PatchCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"|\n\x1a\x44\x65leteCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x18\n\x10\x63ollaborator_ids\x18\x02 \x03(\t\x12\x13\n\x0buser_emails\x18\x03 \x03(\t\"\x82\x01\n\x1aMultiCollaboratorsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.CollaboratorB\x04\x80\xb5\x18\x01\"l\n\x19ListCollaborationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x85\x01\n\x1bMultiCollaborationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0e\x63ollaborations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.CollaborationB\x04\x80\xb5\x18\x01\".\n\x14GetStatusCodeRequest\x12\x16\n\x0estatus_code_id\x18\x01 \x01(\t\"\x18\n\x16ListStatusCodesRequest\"G\n\x18SingleStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"u\n\x17MultiStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08statuses\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.status.Status\"X\n\x11GetConceptRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\"f\n\x13ListConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x91\x01\n\x18ListModelConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xaf\x01\n\x1bPostConceptsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rconcept_query\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ConceptQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"o\n\x13PostConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\"\x80\x01\n\x14PatchConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"j\n\x17GetConceptCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x15SingleConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x63oncept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\"r\n\x14MultiConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.ConceptB\x04\x80\xb5\x18\x01\"\x82\x01\n\x19MultiConceptCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x63oncept_counts\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ConceptCountB\x04\x80\xb5\x18\x01\"\xb1\x01\n\x1bListConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x11\n\tpredicate\x18\x03 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\r\x12\x10\n\x08per_page\x18\x06 \x01(\r\"\x9c\x01\n\x1bPostConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_relations\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelation\"q\n\x1d\x44\x65leteConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"M\n\x1aListKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x85\x01\n\x1aPostKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraph\"\x8f\x01\n\x1dPostConceptMappingJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12=\n\x14\x63oncept_mapping_jobs\x18\x02 \x03(\x0b\x32\x1f.clarifai.api.ConceptMappingJob\"\x8b\x01\n\x1cMultiConceptRelationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_relations\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelationB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1bMultiKnowledgeGraphResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraphB\x04\x80\xb5\x18\x01\"Z\n\x1eMultiConceptMappingJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x02 \x03(\t\"r\n\x19GetConceptLanguageRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\x82\x01\n\x1bListConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\xad\x01\n\x1cPatchConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x9c\x01\n\x1bPostConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x85\x01\n\x1dSingleConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10\x63oncept_language\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x8b\x01\n\x1cMultiConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_languages\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguageB\x04\x80\xb5\x18\x01\"T\n\x0fGetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"l\n\x16GetInputSamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9e\x01\n\x11ListInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x04 \x03(\t\"\x92\x01\n\x13StreamInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08per_page\x18\x02 \x01(\r\x12\x0f\n\x07last_id\x18\x03 \x01(\t\x12\x13\n\x0border_by_id\x18\x05 \x01(\x08\x12\x12\n\ndescending\x18\x04 \x01(\x08\"\x84\x01\n\x11PostInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x19\n\x11inputs_add_job_id\x18\x03 \x01(\t\"z\n\x12PatchInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"W\n\x12\x44\x65leteInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"Y\n\x13\x44\x65leteInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\tJ\x04\x08\x03\x10\x04\"f\n\x13SingleInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xa0\x01\n\x12MultiInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.InputB\x04\x80\xb5\x18\x01\x12\x32\n\x0einputs_add_job\x18\x03 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"r\n\x1cMultiInputAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\"q\n\x18SingleInputCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x06\x63ounts\x18\x02 \x01(\x0b\x32\x18.clarifai.api.InputCount\"G\n\x14GetInputCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"f\n\x13ListDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"X\n\x11GetDatasetRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\"o\n\x13PostDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\"\x80\x01\n\x14PatchDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x16PatchDatasetIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0b\x64\x61taset_ids\x18\x02 \x03(\t\"r\n\x14MultiDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.DatasetB\x04\x80\xb5\x18\x01\"l\n\x15SingleDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Dataset\"\x7f\n\x18ListDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"o\n\x16GetDatasetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb9\x01\n\x18PostDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x32\n\x0e\x64\x61taset_inputs\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.DatasetInput\x12$\n\x06search\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\"t\n\x1a\x44\x65leteDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"\xd2\x01\n\x19MultiDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x64\x61taset_inputs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.DatasetInputB\x04\x80\xb5\x18\x01\x12N\n\x1d\x64\x61taset_inputs_search_add_job\x18\x03 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"|\n\x1aSingleDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rdataset_input\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.DatasetInput\"\x81\x01\n\x1aListDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"{\n\x18GetDatasetVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\"\xa4\x02\n&ListDatasetVersionMetricsGroupsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\x12\x14\n\x0cparent_paths\x18\x06 \x03(\t\x12;\n\x05types\x18\x07 \x03(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12&\n\x06values\x18\x08 \x03(\x0b\x32\x16.google.protobuf.Value\"\x99\x01\n\x1aPostDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\"\xaa\x01\n\x1bPatchDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x1c\x44\x65leteDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61taset_version_ids\x18\x03 \x03(\t\"\xb7\x01\n\x1fPutDatasetVersionExportsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x33\n\x07\x65xports\x18\x04 \x03(\x0b\x32\".clarifai.api.DatasetVersionExport\"\x88\x01\n\x1bMultiDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10\x64\x61taset_versions\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersionB\x04\x80\xb5\x18\x01\"\x8b\x01\n!MultiDatasetVersionExportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x07\x65xports\x18\x02 \x03(\x0b\x32\".clarifai.api.DatasetVersionExportB\x04\x80\xb5\x18\x01\"\xae\x01\n\'MultiDatasetVersionMetricsGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12V\n\x1e\x64\x61taset_version_metrics_groups\x18\x02 \x03(\x0b\x32(.clarifai.api.DatasetVersionMetricsGroupB\x04\x80\xb5\x18\x01\"\x82\x01\n\x1cSingleDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x64\x61taset_version\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\"f\n#GetDatasetInputsSearchAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06job_id\x18\x02 \x01(\t\"\x8c\x01\n\'SingleDatasetInputsSearchAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x03job\x18\x02 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"\xb9\x01\n\x17PostModelOutputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12\"\n\x05model\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Model\"\x8f\x01\n\x16ListModelInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"P\n\rGetKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"\x9a\x01\n\x0fListKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x13\n\x0bnot_expired\x18\x04 \x01(\x08\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x11\n\tendpoints\x18\x06 \x03(\t\"e\n\x12ListAppKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"c\n\x0fPostKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\"S\n\x10\x44\x65leteKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"t\n\x10PatchKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"`\n\x11SingleKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03key\x18\x02 \x01(\x0b\x32\x11.clarifai.api.Key\"f\n\x10MultiKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.KeyB\x04\x80\xb5\x18\x01\"\xad\x01\n\x0fGetModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x16\n\x0etrained_before\x18\x05 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\"\xa3\x04\n\x11ListModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\n \x01(\x08\x12\x16\n\x0csort_by_name\x18\x0b \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\x0c \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\r \x01(\x08H\x00\x12\r\n\x05query\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x19\n\x11\x66ilter_by_user_id\x18\x16 \x01(\x08\x12\x15\n\rmodel_type_id\x18\x06 \x01(\t\x12\x14\n\x0ctrained_only\x18\x07 \x01(\x08\x12\x14\n\x0cinput_fields\x18\x08 \x03(\t\x12\x15\n\routput_fields\x18\t \x03(\t\x12\x0f\n\x07license\x18\x0f \x01(\t\x12\x15\n\rfeatured_only\x18\x10 \x01(\x08\x12\x14\n\x0cstarred_only\x18\x14 \x01(\x08\x12\x10\n\x08toolkits\x18\x11 \x03(\t\x12\x11\n\tuse_cases\x18\x12 \x03(\t\x12\x11\n\tlanguages\x18\x15 \x03(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\x12\x1c\n\x14\x64ont_fetch_from_main\x18\x17 \x01(\x08\x42\t\n\x07sort_byJ\x04\x08\x04\x10\x05\"\x80\x01\n\x19PatchModelToolkitsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08toolkits\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1ePatchModelCheckConsentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x16\n\x0e\x63heck_consents\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x19PatchModelUseCasesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08usecases\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x82\x01\n\x1aPatchModelLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x11\n\tlanguages\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"Z\n\x19MultiModelToolkitResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08toolkits\x18\x02 \x03(\t\"e\n\x1eMultiModelCheckConsentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x16\n\x0e\x63heck_consents\x18\x02 \x03(\t\"Z\n\x19MultiModelUseCaseResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08usecases\x18\x02 \x03(\t\"\\\n\x1aMultiModelLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x11\n\tlanguages\x18\x02 \x03(\t\"\x91\x01\n\x11PostModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ModelB\x02\x18\x01\x12#\n\x06models\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Model\"z\n\x12PatchModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Model\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\",\n\x0eIdUpdateSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06new_id\x18\x02 \x01(\t\"\x82\x01\n\x14PatchModelIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"W\n\x12\x44\x65leteModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\"g\n\x13\x44\x65leteModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\xa9\x01\n\x19PostModelsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0bmodel_query\x18\x02 \x01(\x0b\x32\x18.clarifai.api.ModelQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"f\n\x13SingleModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\"l\n\x12MultiModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.ModelB\x04\x80\xb5\x18\x01\"\xa2\x01\n\x19PatchModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"o\n\x16GetModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\"\x92\x01\n\x18ListModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\x12\x13\n\x0b\x63oncept_ids\x18\x05 \x03(\t\"r\n\x19\x44\x65leteModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x12\n\nversion_id\x18\x04 \x01(\t\"|\n\x1aSingleModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rmodel_version\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\"\x82\x01\n\x19MultiModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0emodel_versions\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ModelVersionB\x04\x80\xb5\x18\x01\"\xef\x01\n\x18PostModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\t\x10\n\"\xb1\x01\n$PostWorkflowVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x43\n\x0cpublications\x18\x03 \x03(\x0b\x32-.clarifai.api.WorkflowVersionUnPublishRequest\"\xad\x01\n\"PostWorkflowVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x41\n\x0cpublications\x18\x03 \x03(\x0b\x32+.clarifai.api.WorkflowVersionPublishRequest\"3\n\x1dWorkflowVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"5\n\x1fWorkflowVersionUnPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"0\n\x1aModelVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa4\x01\n\x1fPostModelVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12>\n\x0cpublications\x18\x03 \x03(\x0b\x32(.clarifai.api.ModelVersionPublishRequest\"2\n\x1cModelVersionUnpublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa8\x01\n!PostModelVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12@\n\x0cpublications\x18\x03 \x03(\x0b\x32*.clarifai.api.ModelVersionUnpublishRequest\"\xb2\x01\n\"PostModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12/\n\x0c\x65val_metrics\x18\x04 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xa1\x01\n\"ListModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xc1\x01\n GetModelVersionEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x15\n\revaluation_id\x18\x04 \x01(\t\x12)\n\x06\x66ields\x18\x05 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"y\n\x19SingleEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\"x\n\x18MultiEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xd3\x01\n\x1ePostModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x0btest_search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05\"\xa1\x01\n\x1dGetModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"]\n\x13GetModelTypeRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rmodel_type_id\x18\x02 \x01(\t\"h\n\x15ListModelTypesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x1f\n\x1dListOpenSourceLicensesRequest\"_\n\x1eListOpenSourceLicensesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08licenses\x18\x02 \x03(\t\"y\n\x17SingleModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\nmodel_type\x18\x02 \x01(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\"\xf2\x01\n\x16MultiModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bmodel_types\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\x12\x35\n\x0fmodel_importers\x18\x03 \x01(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12@\n\x16triton_conda_envs_info\x18\x04 \x03(\x0b\x32 .clarifai.api.TritonCondaEnvInfo\"\x95\x01\n\"GetModelVersionInputExampleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x12\n\nexample_id\x18\x04 \x01(\t\"\xa3\x01\n$ListModelVersionInputExamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xa2\x01\n&SingleModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12K\n\x1bmodel_version_input_example\x18\x02 \x01(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\xa2\x01\n%MultiModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cmodel_version_input_examples\x18\x02 \x03(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\x7f\n\x1aListModelReferencesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x82\x01\n\x1bMultiModelReferenceResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10model_references\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.ModelReference\"o\n\x13MultiOutputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07outputs\x18\x02 \x03(\x0b\x32\x14.clarifai.api.OutputB\x04\x80\xb5\x18\x01\"V\n\x11ListScopesRequest\x12\x10\n\x08key_type\x18\x01 \x01(\t\x12/\n\x0buser_app_id\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"B\n\x0fMyScopesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"F\n\x13MyScopesUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x15\n\x13MyScopesRootRequest\"\xa5\x01\n\x16MultiScopeDepsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\nscope_deps\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ScopeDeps\x12\x31\n\rendpoint_deps\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.EndpointDeps\"\xa0\x01\n\x12MultiScopeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x1e\n\x03\x61pp\x18\x03 \x01(\x0b\x32\x11.clarifai.api.App\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeRootResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"O\n\x10GetSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x13ListSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\xc4\x01\n\x13PostSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05query\x18\x02 \x01(\x0b\x32\x13.clarifai.api.QueryB\x02\x18\x01\x12&\n\x08searches\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Pagination\"\x85\x01\n\x1aPatchInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x8a\x01\n\x1fPatchAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x7f\n\x14PatchSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x17PostSearchesByIDRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"R\n\x13\x44\x65leteSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xa7\x01\n\x1ePostAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"c\n$DeleteAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xa2\x01\n\x19PostInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"i\n\x14SingleSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\"\xc1\x01\n\x13MultiSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\x12\"\n\x05query\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Query\x12&\n\x08searches\x18\x05 \x03(\x0b\x32\x14.clarifai.api.Search\"\x94\x02\n\"PostAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12*\n\x0cground_truth\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\x12 \n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x35\n\x0f\x65valuation_type\x18\x06 \x01(\x0e\x32\x1c.clarifai.api.EvaluationType\"`\n!GetAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"U\n\"ListAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x9d\x01\n$MultiAnnotationSearchMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12H\n\x19\x61nnotation_search_metrics\x18\x02 \x03(\x0b\x32%.clarifai.api.AnnotationSearchMetrics\"o\n\x1cListAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"k\n\x1aGetAnnotationFilterRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1c\n\x14\x61nnotation_filter_id\x18\x02 \x01(\t\"\x8b\x01\n\x1cPostAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\x9c\x01\n\x1dPatchAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"p\n\x1e\x44\x65leteAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1d\n\x15\x61nnotation_filter_ids\x18\x02 \x03(\t\"\x8e\x01\n\x1dMultiAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilterB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1eSingleAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x11\x61nnotation_filter\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"x\n\x1bPostValidatePasswordRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12(\n\x08password\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Password\"\x8e\x01\n SinglePasswordValidationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12=\n\x13password_violations\x18\x02 \x01(\x0b\x32 .clarifai.api.PasswordViolations\"\xbb\x01\n\x12GetWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x03 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x04 \x03(\t\x12\"\n\x1a\x65xclude_clarifai_workflows\x18\x05 \x01(\x08\"\xbb\x02\n\x14ListWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x14\n\nsort_by_id\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x0e\n\x02id\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\t\x12\x13\n\x0bsearch_term\x18\x0c \x01(\tB\t\n\x07sort_by\"r\n\x14PostWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\"\x83\x01\n\x15PatchWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x85\x01\n\x17PatchWorkflowIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\"j\n\x16\x44\x65leteWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"o\n\x16SingleWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\"u\n\x15MultiWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.WorkflowB\x04\x80\xb5\x18\x01\"\xa5\x02\n\x1aPostWorkflowResultsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12#\n\x06inputs\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\routput_config\x18\x04 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x05 \x01(\x08\x12\x33\n\x0eworkflow_state\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\xd8\x01\n\x1bPostWorkflowResultsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12-\n\x07results\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.WorkflowResult\x12\x33\n\x0eworkflow_state\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\x91\x02\n$PostWorkflowResultsSimilarityRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12)\n\x0cprobe_inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12(\n\x0bpool_inputs\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Input\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x06 \x01(\x08\"\x8e\x01\n%PostWorkflowResultsSimilarityResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x07results\x18\x02 \x03(\x0b\x32\'.clarifai.api.WorkflowResultsSimilarity\"\x83\x01\n\x1bListWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x19GetWorkflowVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x03 \x01(\t\"\x83\x01\n\x1d\x44\x65leteWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1c\n\x14workflow_version_ids\x18\x03 \x03(\t\"\xae\x01\n\x1cPatchWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x38\n\x11workflow_versions\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1cMultiWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11workflow_versions\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersionB\x04\x80\xb5\x18\x01\"\x85\x01\n\x1dSingleWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10workflow_version\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\"\x85\x01\n\x1aPostAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"g\n\x18GetAppDuplicationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1a\n\x12\x61pp_duplication_id\x18\x02 \x01(\t\"m\n\x1aListAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x83\x01\n\x1cMultiAppDuplicationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"\x82\x01\n\x1cSingleAppDuplicationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x61pp_duplication\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.AppDuplication\"f\n\x10PostTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\"m\n\x0eGetTaskRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\xee\x01\n\x10ListTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x17\n\x0fworker_user_ids\x18\x04 \x03(\t\x12\x17\n\x0freview_user_ids\x18\x05 \x03(\t\x12\x17\n\x0flabel_order_ids\x18\x08 \x03(\t\x12#\n\x1bincluding_label_order_tasks\x18\x06 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x07 \x03(\t\"w\n\x11PatchTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"R\n\x12\x44\x65leteTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x11MultiTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\'\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.TaskB\x04\x80\xb5\x18\x01\"c\n\x12SingleTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04task\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Task\"i\n\x13GetTaskCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9d\x01\n\x17SingleTaskCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0f\n\x07task_id\x18\x03 \x01(\t\x12\x34\n\x06\x63ounts\x18\x04 \x03(\x0b\x32$.clarifai.api.TaskStatusCountPerUser\"y\n\x16PostLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\"_\n\x14GetLabelOrderRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x16\n\x0elabel_order_id\x18\x02 \x01(\t\"i\n\x16ListLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x8a\x01\n\x17PatchLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"X\n\x18\x44\x65leteLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"|\n\x17MultiLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrderB\x04\x80\xb5\x18\x01\"v\n\x18SingleLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x0blabel_order\x18\x02 \x01(\x0b\x32\x18.clarifai.api.LabelOrder\"u\n\x15PostCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"\x86\x01\n\x16PatchCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"k\n\x17\x44\x65leteCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\\\n\x13GetCollectorRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x14\n\x0c\x63ollector_id\x18\x02 \x01(\t\"h\n\x15ListCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"r\n\x16MultiCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"r\n\x17SingleCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12*\n\tcollector\x18\x02 \x01(\x0b\x32\x17.clarifai.api.Collector\"v\n\x15PostStatValuesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12,\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValue\"y\n\x16MultiStatValueResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValueB\x04\x80\xb5\x18\x01\"\x9e\x01\n\x1ePostStatValuesAggregateRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12K\n\x1cstat_value_aggregate_queries\x18\x02 \x03(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"\x9c\x01\n\x1fMultiStatValueAggregateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cstat_value_aggregate_results\x18\x02 \x03(\x0b\x32&.clarifai.api.StatValueAggregateResult\"w\n\x1ePostTrendingMetricsViewRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\"\x85\x01\n\x1fListTrendingMetricsViewsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n MultiTrendingMetricsViewResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x07metrics\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.TrendingMetric\"V\n\x10GetModuleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\"e\n\x12ListModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x12PostModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Module\"}\n\x13PatchModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Module\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"T\n\x14\x44\x65leteModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x14SingleModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06module\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Module\"o\n\x13MultiModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.ModuleB\x04\x80\xb5\x18\x01\"x\n\x17GetModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11module_version_id\x18\x03 \x01(\t\"\x7f\n\x19ListModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x95\x01\n\x19PostModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x34\n\x0fmodule_versions\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersion\"n\n\x1b\x44\x65leteModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"\x7f\n\x1bSingleModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\"\x85\x01\n\x1aMultiModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12:\n\x0fmodule_versions\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersionB\x04\x80\xb5\x18\x01\"x\n GetInstalledModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"u\n\"ListInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x9e\x01\n\"PostInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12G\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersion\"}\n%PostInstalledModuleVersionsKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"d\n$DeleteInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x9b\x01\n$SingleInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x46\n\x18installed_module_version\x18\x02 \x01(\x0b\x32$.clarifai.api.InstalledModuleVersion\"\xa1\x01\n#MultiInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12M\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersionB\x04\x80\xb5\x18\x01\"\x82\x01\n\x19PostBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0f\x62ulk_operations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"l\n\x19ListBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x17GetBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"Z\n\x1a\x43\x61ncelBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"Z\n\x1a\x44\x65leteBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x80\x01\n\x1cSingleBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.BulkOperation\"\x7f\n\x1bMultiBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"k\n\x18ListInputsAddJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"U\n\x16GetInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\x83\x01\n\x19MultiInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0finputs_add_jobs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsAddJobB\x04\x80\xb5\x18\x01\"}\n\x1aSingleInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0einputs_add_job\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"l\n\x12PostUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"T\n\x14\x44\x65leteUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"e\n\x12ListUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x10GetUploadRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\"i\n\x14SingleUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06upload\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Upload\"i\n\x13MultiUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"\x9a\x01\n\x1cPutUploadContentPartsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\x12\x36\n\rcontent_parts\x18\x03 \x03(\x0b\x32\x1f.clarifai.api.UploadContentPart\"\xad\x01\n\x1cPostInputsDataSourcesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.InputsDataSource\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\"r\n\x1dGetInputsExtractionJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12 \n\x18inputs_extraction_job_id\x18\x02 \x01(\t\"r\n\x1fListInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x92\x01\n!SingleInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x15inputs_extraction_job\x18\x02 \x01(\x0b\x32!.clarifai.api.InputsExtractionJob\"\x92\x01\n MultiInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x41\n\x16inputs_extraction_jobs\x18\x02 \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\"a\n!CancelInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x7f\n\x18PostInputsUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x32\n\x0einputs_uploads\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsUpload*p\n\x1cOrganizationInvitationStatus\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x02\x12\r\n\tCANCELLED\x10\x03\x12\x0c\n\x08\x44\x45\x43LINED\x10\x04\x12\x0b\n\x07\x45XPIRED\x10\x05\x32\xb7\xee\x02\n\x02V2\x12\xaa\x02\n\x14ListConceptRelations\x12).clarifai.api.ListConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"\xba\x01\x82\xd3\xe4\x93\x02\xab\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\x98\x9c\'\x05\x90\x9c\'\x0b\x12\xdf\x01\n\x14PostConceptRelations\x12).clarifai.api.PostConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"p\x82\xd3\xe4\x93\x02^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'\n\x90\x9c\'\x0b\x12\xde\x01\n\x16\x44\x65leteConceptRelations\x12+.clarifai.api.DeleteConceptRelationsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'\r\x90\x9c\'\n\x90\x9c\'\x0b\x12\xdc\x01\n\x10GetConceptCounts\x12%.clarifai.api.GetConceptCountsRequest\x1a\'.clarifai.api.MultiConceptCountResponse\"x\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\x15\x12\x13/v2/concepts/status\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd0\x01\n\nGetConcept\x12\x1f.clarifai.api.GetConceptRequest\x1a#.clarifai.api.SingleConceptResponse\"|\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\x1b\x12\x19/v2/concepts/{concept_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xb9\x01\n\x0cListConcepts\x12!.clarifai.api.ListConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"b\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\x0e\x12\x0c/v2/concepts\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xb9\x02\n\x11ListModelConcepts\x12&.clarifai.api.ListModelConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"\xd7\x01\x82\xd3\xe4\x93\x02\xc4\x01\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xea\x01\n\x14PostConceptsSearches\x12).clarifai.api.PostConceptsSearchesRequest\x1a\".clarifai.api.MultiConceptResponse\"\x82\x01\x82\xd3\xe4\x93\x02l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\x01*Z\x1a\"\x15/v2/concepts/searches:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xc3\x01\n\x0cPostConcepts\x12!.clarifai.api.PostConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"l\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\"\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xc5\x01\n\rPatchConcepts\x12\".clarifai.api.PatchConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"l\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\x32\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x94\x02\n\x12GetConceptLanguage\x12\'.clarifai.api.GetConceptLanguageRequest\x1a+.clarifai.api.SingleConceptLanguageResponse\"\xa7\x01\x82\xd3\xe4\x93\x02\x98\x01\x12\x64/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\x12./v2/concepts/{concept_id}/languages/{language}\x98\x9c\'\x02\x90\x9c\'\x0b\x12\x81\x02\n\x14ListConceptLanguages\x12).clarifai.api.ListConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x91\x01\x82\xd3\xe4\x93\x02\x82\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\x12#/v2/concepts/{concept_id}/languages\x98\x9c\'\x02\x90\x9c\'\x0b\x12\x8b\x02\n\x14PostConceptLanguages\x12).clarifai.api.PostConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(\"#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x8d\x02\n\x15PatchConceptLanguages\x12*.clarifai.api.PatchConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x88\x01\x32Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(2#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xf1\x01\n\x13ListKnowledgeGraphs\x12(.clarifai.api.ListKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\x1f\x12\x1d/v2/concepts/knowledge_graphs\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xfb\x01\n\x13PostKnowledgeGraphs\x12(.clarifai.api.PostKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\x01*Z\"\"\x1d/v2/concepts/knowledge_graphs:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xfe\x01\n\x16PostConceptMappingJobs\x12+.clarifai.api.PostConceptMappingJobsRequest\x1a,.clarifai.api.MultiConceptMappingJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\x01*Z\x1f\"\x1a/v2/concepts/mappings/jobs:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x93\x02\n\rGetAnnotation\x12\".clarifai.api.GetAnnotationRequest\x1a&.clarifai.api.SingleAnnotationResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\x9e\x01\x12g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\x12\x31/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xd0\x01\n\x0fListAnnotations\x12$.clarifai.api.ListAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"p\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\x11\x12\x0f/v2/annotations\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe3\x01\n\x0fPostAnnotations\x12$.clarifai.api.PostAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x82\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\"\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe5\x01\n\x10PatchAnnotations\x12%.clarifai.api.PatchAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x82\x01\x82\xd3\xe4\x93\x02`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\x32\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf3\x01\n\x16PatchAnnotationsStatus\x12+.clarifai.api.PatchAnnotationsStatusRequest\x1a,.clarifai.api.PatchAnnotationsStatusResponse\"~\x82\xd3\xe4\x93\x02`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\x9c\x02\n\x10\x44\x65leteAnnotation\x12%.clarifai.api.DeleteAnnotationRequest\x1a!.clarifai.api.status.BaseResponse\"\xbd\x01\x82\xd3\xe4\x93\x02\x9e\x01*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd0\x02\n\x11\x44\x65leteAnnotations\x12&.clarifai.api.DeleteAnnotationsRequest\x1a!.clarifai.api.status.BaseResponse\"\xef\x01\x82\xd3\xe4\x93\x02\xd0\x01*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\x01*Z\x1b*\x16/v2/inputs/annotations:\x01*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14*\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf3\x01\n\x18PatchAnnotationsSearches\x12-.clarifai.api.PatchAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x84\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\x32\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\x81\x02\n\x17PostAnnotationsSearches\x12,.clarifai.api.PostAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x94\x01\x82\xd3\xe4\x93\x02r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\"\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd1\x01\n\rGetInputCount\x12\".clarifai.api.GetInputCountRequest\x1a&.clarifai.api.SingleInputCountResponse\"t\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\x13\x12\x11/v2/inputs/status\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xc9\x01\n\x0cStreamInputs\x12!.clarifai.api.StreamInputsRequest\x1a .clarifai.api.MultiInputResponse\"t\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\x13\x12\x11/v2/inputs/stream\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xfd\x01\n\x0fGetInputSamples\x12$.clarifai.api.GetInputSamplesRequest\x1a*.clarifai.api.MultiInputAnnotationResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\x12\"/v2/tasks/{task_id}/inputs/samples\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xca\x01\n\x08GetInput\x12\x1d.clarifai.api.GetInputRequest\x1a!.clarifai.api.SingleInputResponse\"|\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17\x12\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xb7\x01\n\nListInputs\x12\x1f.clarifai.api.ListInputsRequest\x1a .clarifai.api.MultiInputResponse\"f\x82\xd3\xe4\x93\x02P\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\x0c\x12\n/v2/inputs\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd2\x01\n\nPostInputs\x12\x1f.clarifai.api.PostInputsRequest\x1a .clarifai.api.MultiInputResponse\"\x80\x01\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\"\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xcb\x01\n\x0bPatchInputs\x12 .clarifai.api.PatchInputsRequest\x1a .clarifai.api.MultiInputResponse\"x\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\x32\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x12\xe5\x01\n\x0b\x44\x65leteInput\x12 .clarifai.api.DeleteInputRequest\x1a!.clarifai.api.status.BaseResponse\"\x90\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17*\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xd7\x01\n\x0c\x44\x65leteInputs\x12!.clarifai.api.DeleteInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f*\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xde\x01\n\x13PatchInputsSearches\x12(.clarifai.api.PatchInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"z\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\x32\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\xed\x01\n\x12PostInputsSearches\x12\'.clarifai.api.PostInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\"\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\x9c\x03\n\x10PostModelOutputs\x12%.clarifai.api.PostModelOutputsRequest\x1a!.clarifai.api.MultiOutputResponse\"\xbd\x02\x82\xd3\xe4\x93\x02\xa6\x02\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\x01*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\x01*Z\"\"\x1d/v2/models/{model_id}/outputs:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x02\x12\xbd\x01\n\x0cListDatasets\x12!.clarifai.api.ListDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ\x0e\x12\x0c/v2/datasets\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xd5\x01\n\nGetDataset\x12\x1f.clarifai.api.GetDatasetRequest\x1a#.clarifai.api.SingleDatasetResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\x1b\x12\x19/v2/datasets/{dataset_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xc7\x01\n\x0cPostDatasets\x12!.clarifai.api.PostDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"p\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\"\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xc9\x01\n\rPatchDatasets\x12\".clarifai.api.PatchDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\x32\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xba\x01\n\x0fPatchDatasetIds\x12$.clarifai.api.PatchDatasetIdsRequest\x1a\".clarifai.api.MultiDatasetResponse\"]\x82\xd3\xe4\x93\x02K2F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/ids:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\xca\x01\n\x0e\x44\x65leteDatasets\x12#.clarifai.api.DeleteDatasetsRequest\x1a!.clarifai.api.status.BaseResponse\"p\x82\xd3\xe4\x93\x02Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11*\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xfd\x01\n\x11ListDatasetInputs\x12&.clarifai.api.ListDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\x96\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\x12 /v2/datasets/{dataset_id}/inputs\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x91\x02\n\x0fGetDatasetInput\x12$.clarifai.api.GetDatasetInputRequest\x1a(.clarifai.api.SingleDatasetInputResponse\"\xad\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\x12+/v2/datasets/{dataset_id}/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x88\x02\n\x11PostDatasetInputs\x12&.clarifai.api.PostDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%\" /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x82\x02\n\x13\x44\x65leteDatasetInputs\x12(.clarifai.api.DeleteDatasetInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x82\x01*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%* /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x90\x9c\'\x05\x12\x80\x02\n\x13ListDatasetVersions\x12(.clarifai.api.ListDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\x12\"/v2/datasets/{dataset_id}/versions\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xa7\x02\n\x11GetDatasetVersion\x12&.clarifai.api.GetDatasetVersionRequest\x1a*.clarifai.api.SingleDatasetVersionResponse\"\xbd\x01\x82\xd3\xe4\x93\x02\xaa\x01\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\x12\x37/v2/datasets/{dataset_id}/versions/{dataset_version_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xe6\x02\n\x1fListDatasetVersionMetricsGroups\x12\x34.clarifai.api.ListDatasetVersionMetricsGroupsRequest\x1a\x35.clarifai.api.MultiDatasetVersionMetricsGroupResponse\"\xd5\x01\x82\xd3\xe4\x93\x02\xba\x01\x12u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\x12?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x8e\x02\n\x13PostDatasetVersions\x12(.clarifai.api.PostDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'\"\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x88\x02\n\x14PatchDatasetVersions\x12).clarifai.api.PatchDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x86\x01\x32X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'2\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\x86\x02\n\x15\x44\x65leteDatasetVersions\x12*.clarifai.api.DeleteDatasetVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'*\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xd0\x02\n\x18PutDatasetVersionExports\x12-.clarifai.api.PutDatasetVersionExportsRequest\x1a/.clarifai.api.MultiDatasetVersionExportResponse\"\xd3\x01\x82\xd3\xe4\x93\x02\xc0\x01\x1au/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*ZD\x1a?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\xe5\x01\n\x0cGetModelType\x12!.clarifai.api.GetModelTypeRequest\x1a%.clarifai.api.SingleModelTypeResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\x12 /v2/models/types/{model_type_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x12\x99\x01\n\x16ListOpenSourceLicenses\x12+.clarifai.api.ListOpenSourceLicensesRequest\x1a,.clarifai.api.ListOpenSourceLicensesResponse\"$\x82\xd3\xe4\x93\x02\x1a\x12\x18/v2/open_source_licenses\x98\x9c\'\x01\x12\xc7\x01\n\x0eListModelTypes\x12#.clarifai.api.ListModelTypesRequest\x1a$.clarifai.api.MultiModelTypeResponse\"j\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\x12\x12\x10/v2/models/types\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xc6\x01\n\x08GetModel\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"x\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17\x12\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\x96\x03\n\x12GetModelOutputInfo\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"\xbd\x02\x82\xd3\xe4\x93\x02\xaa\x02\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\x12!/v2/models/{model_id}/output_infoZo\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\x12\x37/v2/models/{model_id}/versions/{version_id}/output_info\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xde\x01\n\nListModels\x12\x1f.clarifai.api.ListModelsRequest\x1a .clarifai.api.MultiModelResponse\"\x8c\x01\x82\xd3\xe4\x93\x02z\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\x12&/v2/users/{user_app_id.user_id}/modelsZ\x0c\x12\n/v2/models\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xdb\x01\n\x12PostModelsSearches\x12\'.clarifai.api.PostModelsSearchesRequest\x1a .clarifai.api.MultiModelResponse\"z\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\x01*Z\x18\"\x13/v2/models/searches:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xc6\x01\n\nPostModels\x12\x1f.clarifai.api.PostModelsRequest\x1a!.clarifai.api.SingleModelResponse\"t\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\"\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x12\xc3\x01\n\x0bPatchModels\x12 .clarifai.api.PatchModelsRequest\x1a .clarifai.api.MultiModelResponse\"p\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\x32\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x12\xb2\x01\n\rPatchModelIds\x12\".clarifai.api.PatchModelIdsRequest\x1a .clarifai.api.MultiModelResponse\"[\x82\xd3\xe4\x93\x02I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\x01*\x98\x9c\'\x02\x90\x9c\'\x0e\x90\x9c\'\x0f\x12\xd9\x01\n\x0b\x44\x65leteModel\x12 .clarifai.api.DeleteModelRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17*\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xca\x01\n\x0c\x44\x65leteModels\x12!.clarifai.api.DeleteModelsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f*\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x91\x02\n\x17PatchModelCheckConsents\x12,.clarifai.api.PatchModelCheckConsentsRequest\x1a,.clarifai.api.MultiModelCheckConsentResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\x01*Z)2$/v2/models/{model_id}/check_consents:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xf5\x01\n\x12PatchModelToolkits\x12\'.clarifai.api.PatchModelToolkitsRequest\x1a\'.clarifai.api.MultiModelToolkitResponse\"\x8c\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\x01*Z#2\x1e/v2/models/{model_id}/toolkits:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xf5\x01\n\x12PatchModelUseCases\x12\'.clarifai.api.PatchModelUseCasesRequest\x1a\'.clarifai.api.MultiModelUseCaseResponse\"\x8c\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\x01*Z#2\x1e/v2/models/{model_id}/usecases:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xfb\x01\n\x13PatchModelLanguages\x12(.clarifai.api.PatchModelLanguagesRequest\x1a(.clarifai.api.MultiModelLanguageResponse\"\x8f\x01\x82\xd3\xe4\x93\x02\x80\x01\x32U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\x01*Z$2\x1f/v2/models/{model_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\x8d\x03\n\x0fListModelInputs\x12$.clarifai.api.ListModelInputsRequest\x1a .clarifai.api.MultiInputResponse\"\xb1\x02\x82\xd3\xe4\x93\x02\x96\x02\x12R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\x1e\x12\x1c/v2/models/{model_id}/inputsZj\x12h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\x12\x32/v2/models/{model_id}/versions/{version_id}/inputs\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x12\x89\x02\n\x0fGetModelVersion\x12$.clarifai.api.GetModelVersionRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\x12+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xf1\x01\n\x11ListModelVersions\x12&.clarifai.api.ListModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"\x8a\x01\x82\xd3\xe4\x93\x02x\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \x12\x1e/v2/models/{model_id}/versions\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xb8\x02\n\x1dPostWorkflowVersionsUnPublish\x12\x32.clarifai.api.PostWorkflowVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbf\x01\x82\xd3\xe4\x93\x02\x8c\x01\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\x01*Z*\"%/v2/workflows/{workflow_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'x\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xb0\x02\n\x1bPostWorkflowVersionsPublish\x12\x30.clarifai.api.PostWorkflowVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbb\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\x01*Z(\"#/v2/workflows/{workflow_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'w\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x9d\x02\n\x18PostModelVersionsPublish\x12-.clarifai.api.PostModelVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xae\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\x01*Z\"\"\x1d/v2/models/{model_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'u\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xa6\x02\n\x1aPostModelVersionsUnPublish\x12/.clarifai.api.PostModelVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb3\x01\x82\xd3\xe4\x93\x02\x80\x01\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\x01*Z$\"\x1f/v2/models/{model_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'v\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x8d\x02\n\x11PostModelVersions\x12&.clarifai.api.PostModelVersionsRequest\x1a!.clarifai.api.SingleModelResponse\"\xac\x01\x82\xd3\xe4\x93\x02~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*Z#\"\x1e/v2/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdb\x01\n\x12PatchModelVersions\x12\'.clarifai.api.PatchModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"s\x82\xd3\xe4\x93\x02Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x0e\x90\x9c\'\x1a\x12\x94\x02\n\x12\x44\x65leteModelVersion\x12\'.clarifai.api.DeleteModelVersionRequest\x1a!.clarifai.api.status.BaseResponse\"\xb1\x01\x82\xd3\xe4\x93\x02\x92\x01*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb3\x02\n\x16GetModelVersionMetrics\x12+.clarifai.api.GetModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\xa2\x01\x12i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\x12\x33/v2/models/{model_id}/versions/{version_id}/metrics\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xcf\x02\n\x17PostModelVersionMetrics\x12,.clarifai.api.PostModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xdb\x01\x82\xd3\xe4\x93\x02\xa8\x01\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xe9\x02\n\x1bPostModelVersionEvaluations\x12\x30.clarifai.api.PostModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xef\x01\x82\xd3\xe4\x93\x02\xbc\x01\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\x01*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xcf\x02\n\x1bListModelVersionEvaluations\x12\x30.clarifai.api.ListModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xd5\x01\x82\xd3\xe4\x93\x02\xb6\x01\x12s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\x12=/v2/models/{model_id}/versions/{model_version_id}/evaluations\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xed\x02\n\x19GetModelVersionEvaluation\x12..clarifai.api.GetModelVersionEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\xf6\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf7\x01\n\x13ListModelReferences\x12(.clarifai.api.ListModelReferencesRequest\x1a).clarifai.api.MultiModelReferenceResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\x12 /v2/models/{model_id}/references\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xee\x02\n\x1bGetModelVersionInputExample\x12\x30.clarifai.api.GetModelVersionInputExampleRequest\x1a\x34.clarifai.api.SingleModelVersionInputExampleResponse\"\xe6\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xd6\x02\n\x1dListModelVersionInputExamples\x12\x32.clarifai.api.ListModelVersionInputExamplesRequest\x1a\x33.clarifai.api.MultiModelVersionInputExampleResponse\"\xcb\x01\x82\xd3\xe4\x93\x02\xbc\x01\x12v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\x12@/v2/models/{model_id}/versions/{model_version_id}/input_examples\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xdc\x01\n\x0bGetWorkflow\x12 .clarifai.api.GetWorkflowRequest\x1a$.clarifai.api.SingleWorkflowResponse\"\x84\x01\x82\xd3\xe4\x93\x02r\x12Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d\x12\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xf1\x01\n\rListWorkflows\x12\".clarifai.api.ListWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"\x96\x01\x82\xd3\xe4\x93\x02\x83\x01\x12\x43/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\x12)/v2/users/{user_app_id.user_id}/workflowsZ\x0f\x12\r/v2/workflows\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xcc\x01\n\rPostWorkflows\x12\".clarifai.api.PostWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"r\x82\xd3\xe4\x93\x02\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\"\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xce\x01\n\x0ePatchWorkflows\x12#.clarifai.api.PatchWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"r\x82\xd3\xe4\x93\x02\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\x32\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xbe\x01\n\x10PatchWorkflowIds\x12%.clarifai.api.PatchWorkflowIdsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"^\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\x01*\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x13\x12\xe3\x01\n\x0e\x44\x65leteWorkflow\x12#.clarifai.api.DeleteWorkflowRequest\x1a!.clarifai.api.status.BaseResponse\"\x88\x01\x82\xd3\xe4\x93\x02r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d*\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\xce\x01\n\x0f\x44\x65leteWorkflows\x12$.clarifai.api.DeleteWorkflowsRequest\x1a!.clarifai.api.status.BaseResponse\"r\x82\xd3\xe4\x93\x02\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12*\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\x86\x03\n\x13PostWorkflowResults\x12(.clarifai.api.PostWorkflowResultsRequest\x1a).clarifai.api.PostWorkflowResultsResponse\"\x99\x02\x82\xd3\xe4\x93\x02\xfe\x01\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\x01*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\x01*Z(\"#/v2/workflows/{workflow_id}/results:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\xc5\x03\n\x1dPostWorkflowResultsSimilarity\x12\x32.clarifai.api.PostWorkflowResultsSimilarityRequest\x1a\x33.clarifai.api.PostWorkflowResultsSimilarityResponse\"\xba\x02\x82\xd3\xe4\x93\x02\x9f\x02\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\x01*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\x01*Z3\"./v2/workflows/{workflow_id}/results/similarity:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\x87\x02\n\x14ListWorkflowVersions\x12).clarifai.api.ListWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\x12$/v2/workflows/{workflow_id}/versions\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb0\x02\n\x12GetWorkflowVersion\x12\'.clarifai.api.GetWorkflowVersionRequest\x1a+.clarifai.api.SingleWorkflowVersionResponse\"\xc3\x01\x82\xd3\xe4\x93\x02\xb0\x01\x12p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\x12:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x8c\x02\n\x16\x44\x65leteWorkflowVersions\x12+.clarifai.api.DeleteWorkflowVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x8a\x01*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)*$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x12\x90\x9c\'\x15\x12\x93\x02\n\x15PatchWorkflowVersions\x12*.clarifai.api.PatchWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)2$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x85\x01\n\x06GetKey\x12\x1b.clarifai.api.GetKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"=\x82\xd3\xe4\x93\x02/\x12-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'0\x12\x7f\n\x08ListKeys\x12\x1d.clarifai.api.ListKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"4\x82\xd3\xe4\x93\x02&\x12$/v2/users/{user_app_id.user_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\x9f\x01\n\x0bListAppKeys\x12 .clarifai.api.ListAppKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"N\x82\xd3\xe4\x93\x02@\x12>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\x95\x01\n\tDeleteKey\x12\x1e.clarifai.api.DeleteKeyRequest\x1a!.clarifai.api.status.BaseResponse\"E\x82\xd3\xe4\x93\x02/*-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'1\x90\x9c\'0\x12\x8a\x01\n\x08PostKeys\x12\x1d.clarifai.api.PostKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"?\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\x88\x01\n\tPatchKeys\x12\x1e.clarifai.api.PatchKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'0\x12\xbc\x01\n\x08MyScopes\x12\x1d.clarifai.api.MyScopesRequest\x1a .clarifai.api.MultiScopeResponse\"o\x82\xd3\xe4\x93\x02\x65\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/myscopesZ\x0e\x12\x0c/v2/myscopesZ\x0f\x12\r/v2/my_scopes\x98\x9c\'\x02\x12\x8d\x01\n\x0cMyScopesUser\x12!.clarifai.api.MyScopesUserRequest\x1a$.clarifai.api.MultiScopeUserResponse\"4\x82\xd3\xe4\x93\x02*\x12(/v2/users/{user_app_id.user_id}/myscopes\x98\x9c\'\x05\x12u\n\x0cMyScopesRoot\x12!.clarifai.api.MyScopesRootRequest\x1a$.clarifai.api.MultiScopeRootResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/myscopesroot\x98\x9c\'\x05\x12\x87\x01\n\nListScopes\x12\x1f.clarifai.api.ListScopesRequest\x1a$.clarifai.api.MultiScopeDepsResponse\"2\x82\xd3\xe4\x93\x02(\x12&/v2/users/{user_app_id.user_id}/scopes\x98\x9c\'\x03\x12\x95\x01\n\x06GetApp\x12\x1b.clarifai.api.GetAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"M\x82\xd3\xe4\x93\x02;\x12\x39/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\x8f\x01\n\x08ListApps\x12\x1d.clarifai.api.ListAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\x12$/v2/users/{user_app_id.user_id}/appsZ\n\x12\x08/v2/apps\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\xa5\x01\n\tDeleteApp\x12\x1e.clarifai.api.DeleteAppRequest\x1a!.clarifai.api.status.BaseResponse\"U\x82\xd3\xe4\x93\x02;*9/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'.\x90\x9c\'-\x90\x9c\'\x13\x12\x92\x01\n\x08PostApps\x12\x1d.clarifai.api.PostAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"G\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x88\x01\n\tPatchApps\x12\x1e.clarifai.api.PatchAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x92\x01\n\x0cPatchAppsIds\x12!.clarifai.api.PatchAppsIdsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"?\x82\xd3\xe4\x93\x02-2(/v2/users/{user_app_id.user_id}/apps/ids:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9c\x01\n\x08PatchApp\x12\x1d.clarifai.api.PatchAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"P\x82\xd3\xe4\x93\x02>29/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9f\x01\n\x10PostAppsSearches\x12%.clarifai.api.PostAppsSearchesRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\"-/v2/users/{user_app_id.user_id}/apps/searches:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\xcf\x01\n\x14PostValidatePassword\x12).clarifai.api.PostValidatePasswordRequest\x1a..clarifai.api.SinglePasswordValidationResponse\"\\\x82\xd3\xe4\x93\x02R\"1/v2/users/{user_app_id.user_id}/validate_password:\x01*Z\x1a\"\x15/v2/validate_password:\x01*\x98\x9c\'\x03\x12\xbd\x01\n\tGetSearch\x12\x1e.clarifai.api.GetSearchRequest\x1a\".clarifai.api.SingleSearchResponse\"l\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13\x12\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'r\x12\xb8\x01\n\x0cListSearches\x12!.clarifai.api.ListSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"b\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\x0e\x12\x0c/v2/searches\x98\x9c\'\x02\x90\x9c\'r\x12\xc4\x01\n\rPatchSearches\x12\".clarifai.api.PatchSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"l\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\x32\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\xd5\x01\n\x0cPostSearches\x12!.clarifai.api.PostSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x7f\x88\x02\x01\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\"\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd4\x01\n\x10PostSearchesByID\x12%.clarifai.api.PostSearchesByIDRequest\x1a!.clarifai.api.MultiSearchResponse\"v\x82\xd3\xe4\x93\x02\x64\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\x01*Z\x16\"\x11/v2/searches/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'\x03\x12\xaf\x02\n\x1bPostAnnotationSearchMetrics\x12\x30.clarifai.api.PostAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\x01*Z%\" /v2/annotations/searches/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x90\x9c\'6\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xa5\x02\n\x1aGetAnnotationSearchMetrics\x12/.clarifai.api.GetAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\x12%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x9c\x02\n\x1bListAnnotationSearchMetrics\x12\x30.clarifai.api.ListAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\x96\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\x12 /v2/annotations/searches/metrics\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x96\x02\n\x1d\x44\x65leteAnnotationSearchMetrics\x12\x32.clarifai.api.DeleteAnnotationSearchMetricsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'5\x90\x9c\'6\x90\x9c\'?\x12\xca\x01\n\x0c\x44\x65leteSearch\x12!.clarifai.api.DeleteSearchRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13*\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x90\x9c\'t\x12\xe8\x01\n\x15ListAnnotationFilters\x12*.clarifai.api.ListAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"v\x82\xd3\xe4\x93\x02h\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\x18\x12\x16/v2/annotation_filters\x98\x9c\'\x02\x90\x9c\'r\x12\x95\x02\n\x13GetAnnotationFilter\x12(.clarifai.api.GetAnnotationFilterRequest\x1a,.clarifai.api.SingleAnnotationFilterResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x96\x01\x12\x63/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\x12-/v2/annotation_filters/{annotation_filter_id}\x98\x9c\'\x02\x90\x9c\'r\x12\xf3\x01\n\x15PostAnnotationFilters\x12*.clarifai.api.PostAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\"\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12\xf5\x01\n\x16PatchAnnotationFilters\x12+.clarifai.api.PatchAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x80\x01\x82\xd3\xe4\x93\x02n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\x32\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12\xed\x01\n\x17\x44\x65leteAnnotationFilters\x12,.clarifai.api.DeleteAnnotationFiltersRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b*\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12|\n\x0fListStatusCodes\x12$.clarifai.api.ListStatusCodesRequest\x1a%.clarifai.api.MultiStatusCodeResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/status_codes\x98\x9c\'\x01\x12\x8a\x01\n\rGetStatusCode\x12\".clarifai.api.GetStatusCodeRequest\x1a&.clarifai.api.SingleStatusCodeResponse\"-\x82\xd3\xe4\x93\x02#\x12!/v2/status_codes/{status_code_id}\x98\x9c\'\x01\x12\xbe\x01\n\x11ListCollaborators\x12&.clarifai.api.ListCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"W\x82\xd3\xe4\x93\x02I\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\x98\x9c\'\x02\x90\x9c\'2\x12\xc5\x01\n\x11PostCollaborators\x12&.clarifai.api.PostCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"^\x82\xd3\xe4\x93\x02L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x12\xcb\x01\n\x12PatchCollaborators\x12\'.clarifai.api.PatchCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"b\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x12\xce\x01\n\x13\x44\x65leteCollaborators\x12(.clarifai.api.DeleteCollaboratorsRequest\x1a!.clarifai.api.status.BaseResponse\"j\x82\xd3\xe4\x93\x02L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x90\x9c\'7\x90\x9c\'8\x12\xa4\x01\n\x12ListCollaborations\x12\'.clarifai.api.ListCollaborationsRequest\x1a).clarifai.api.MultiCollaborationsResponse\":\x82\xd3\xe4\x93\x02\x30\x12./v2/users/{user_app_id.user_id}/collaborations\x98\x9c\'\x03\x12\xef\x01\n\x13PostAppDuplications\x12(.clarifai.api.PostAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"\x81\x01\x82\xd3\xe4\x93\x02K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\x01*\x98\x9c\'\x02\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\n\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x12\x90\x9c\'\x13\x12\xa5\x01\n\x13ListAppDuplications\x12(.clarifai.api.ListAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"8\x82\xd3\xe4\x93\x02.\x12,/v2/users/{user_app_id.user_id}/duplications\x98\x9c\'\x05\x12\xb6\x01\n\x11GetAppDuplication\x12&.clarifai.api.GetAppDuplicationRequest\x1a*.clarifai.api.SingleAppDuplicationResponse\"M\x82\xd3\xe4\x93\x02\x43\x12\x41/v2/users/{user_app_id.user_id}/duplications/{app_duplication_id}\x98\x9c\'\x05\x12\xd5\x01\n\tPostTasks\x12\x1e.clarifai.api.PostTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x86\x01\x82\xd3\xe4\x93\x02T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\"\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'\x03\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xfa\x01\n\x16GetTaskAnnotationCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\x12%/v2/tasks/{task_id}/annotations/count\x98\x9c\'\x02\x90\x9c\'8\x12\xea\x01\n\x11GetTaskInputCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\x12 /v2/tasks/{task_id}/inputs/count\x98\x9c\'\x02\x90\x9c\'8\x12\xcc\x01\n\x07GetTask\x12\x1c.clarifai.api.GetTaskRequest\x1a .clarifai.api.SingleTaskResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\x15\x12\x13/v2/tasks/{task_id}\x98\x9c\'\x02\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xba\x01\n\tListTasks\x12\x1e.clarifai.api.ListTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"l\x82\xd3\xe4\x93\x02N\x12?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\x0b\x12\t/v2/tasks\x98\x9c\'\x02\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd3\x01\n\nPatchTasks\x12\x1f.clarifai.api.PatchTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x82\x01\x82\xd3\xe4\x93\x02T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\x32\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xbe\x01\n\x0b\x44\x65leteTasks\x12 .clarifai.api.DeleteTasksRequest\x1a!.clarifai.api.status.BaseResponse\"j\x82\xd3\xe4\x93\x02T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e*\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xf1\x01\n\x0fPostLabelOrders\x12$.clarifai.api.PostLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x90\x01\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\"\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf2\x01\n\rGetLabelOrder\x12\".clarifai.api.GetLabelOrderRequest\x1a&.clarifai.api.SingleLabelOrderResponse\"\x94\x01\x82\xd3\xe4\x93\x02~\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\x12!/v2/label_orders/{label_order_id}\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xd2\x01\n\x0fListLabelOrders\x12$.clarifai.api.ListLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"r\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\x12\x12\x10/v2/label_orders\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xe7\x01\n\x10PatchLabelOrders\x12%.clarifai.api.PatchLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62\x32\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\x32\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'D\x90\x9c\'\x0b\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xe1\x01\n\x11\x44\x65leteLabelOrders\x12&.clarifai.api.DeleteLabelOrdersRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15*\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'E\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x12\xee\x01\n\x0ePostCollectors\x12#.clarifai.api.PostCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"\x90\x01\x82\xd3\xe4\x93\x02^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\"\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'\x04\x90\x9c\'%\x90\x9c\'&\x90\x9c\')\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xdf\x01\n\x0cGetCollector\x12!.clarifai.api.GetCollectorRequest\x1a%.clarifai.api.SingleCollectorResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\x1f\x12\x1d/v2/collectors/{collector_id}\x98\x9c\'\x02\x90\x9c\'*\x12\xc3\x01\n\x0eListCollectors\x12#.clarifai.api.ListCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"f\x82\xd3\xe4\x93\x02X\x12\x44/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\x10\x12\x0e/v2/collectors\x98\x9c\'\x02\x90\x9c\'*\x12\xcf\x01\n\x0fPatchCollectors\x12$.clarifai.api.PatchCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"p\x82\xd3\xe4\x93\x02^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\x32\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\')\x90\x9c\'*\x12\xd2\x01\n\x10\x44\x65leteCollectors\x12%.clarifai.api.DeleteCollectorsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13*\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\')\x90\x9c\'+\x90\x9c\'*\x12\xc9\x01\n\x0ePostStatValues\x12#.clarifai.api.PostStatValuesRequest\x1a$.clarifai.api.MultiStatValueResponse\"l\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values:\x01*Z\x15\"\x10/v2/stats/values:\x01*\x98\x9c\'\x02\x12\xf9\x01\n\x17PostStatValuesAggregate\x12,.clarifai.api.PostStatValuesAggregateRequest\x1a-.clarifai.api.MultiStatValueAggregateResponse\"\x80\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\x01*Z\x1f\"\x1a/v2/stats/values/aggregate:\x01*\x98\x9c\'\x02\x12\xe3\x01\n\x17PostTrendingMetricsView\x12,.clarifai.api.PostTrendingMetricsViewRequest\x1a!.clarifai.api.status.BaseResponse\"w\x82\xd3\xe4\x93\x02m\"h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}/{object_id}:\x01*\x98\x9c\'\x02\x12\x8f\x02\n\x18ListTrendingMetricsViews\x12-.clarifai.api.ListTrendingMetricsViewsRequest\x1a..clarifai.api.MultiTrendingMetricsViewResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x88\x01\x12\\/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}Z(\x12&/v2/trending_metrics/views/{view_type}\x98\x9c\'\x02\x12\xae\x01\n\tGetModule\x12\x1e.clarifai.api.GetModuleRequest\x1a\".clarifai.api.SingleModuleResponse\"]\x82\xd3\xe4\x93\x02O\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\x98\x9c\'\x02\x90\x9c\'m\x12\xe0\x01\n\x0bListModules\x12 .clarifai.api.ListModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\x8b\x01\x82\xd3\xe4\x93\x02}\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\x12\'/v2/users/{user_app_id.user_id}/modulesZ\r\x12\x0b/v2/modules\x98\x9c\'\x02\x90\x9c\'m\x12\xac\x01\n\x0bPostModules\x12 .clarifai.api.PostModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"X\x82\xd3\xe4\x93\x02\x46\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xae\x01\n\x0cPatchModules\x12!.clarifai.api.PatchModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"X\x82\xd3\xe4\x93\x02\x46\x32\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xb4\x01\n\rDeleteModules\x12\".clarifai.api.DeleteModulesRequest\x1a!.clarifai.api.status.BaseResponse\"\\\x82\xd3\xe4\x93\x02\x46*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x12\xe8\x01\n\x10GetModuleVersion\x12%.clarifai.api.GetModuleVersionRequest\x1a).clarifai.api.SingleModuleVersionResponse\"\x81\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions/{module_version_id}\x98\x9c\'\x02\x90\x9c\'m\x12\xd6\x01\n\x12ListModuleVersions\x12\'.clarifai.api.ListModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"m\x82\xd3\xe4\x93\x02_\x12]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions\x98\x9c\'\x02\x90\x9c\'m\x12\xdd\x01\n\x12PostModuleVersions\x12\'.clarifai.api.PostModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"t\x82\xd3\xe4\x93\x02\x62\"]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xde\x01\n\x14\x44\x65leteModuleVersions\x12).clarifai.api.DeleteModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02\x62*]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x12\x8b\x02\n\x19GetInstalledModuleVersion\x12..clarifai.api.GetInstalledModuleVersionRequest\x1a\x32.clarifai.api.SingleInstalledModuleVersionResponse\"\x89\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\x98\x9c\'\x05\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xef\x01\n\x1bListInstalledModuleVersions\x12\x30.clarifai.api.ListInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"k\x82\xd3\xe4\x93\x02U\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\x98\x9c\'\x05\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf6\x01\n\x1bPostInstalledModuleVersions\x12\x30.clarifai.api.PostInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"r\x82\xd3\xe4\x93\x02X\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x12\xf6\x01\n\x1d\x44\x65leteInstalledModuleVersions\x12\x32.clarifai.api.DeleteInstalledModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"~\x82\xd3\xe4\x93\x02X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'q\x90\x9c\'m\x90\x9c\'1\x90\x9c\'/\x90\x9c\'0\x12\x95\x02\n\x1ePostInstalledModuleVersionsKey\x12\x33.clarifai.api.PostInstalledModuleVersionsKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\"u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}/key:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\xf1\x01\n\x12PostBulkOperations\x12\'.clarifai.api.PostBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"\x86\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\"\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'z\x90\x9c\'y\x90\x9c\'%\x90\x9c\'&\x90\x9c\'(\x12\xda\x01\n\x12ListBulkOperations\x12\'.clarifai.api.ListBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"p\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\x15\x12\x13/v2/bulk_operations\x98\x9c\'\x02\x90\x9c\'z\x12\xe1\x01\n\x10GetBulkOperation\x12%.clarifai.api.GetBulkOperationRequest\x1a*.clarifai.api.SingleBulkOperationsResponse\"z\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\x1a\x12\x18/v2/bulk_operations/{id}\x98\x9c\'\x02\x90\x9c\'z\x12\xe7\x01\n\x14\x43\x61ncelBulkOperations\x12(.clarifai.api.CancelBulkOperationRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"z\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\x32\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'y\x90\x9c\'z\x12\xf0\x01\n\x14\x44\x65leteBulkOperations\x12(.clarifai.api.DeleteBulkOperationRequest\x1a!.clarifai.api.status.BaseResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18*\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'%\x90\x9c\'(\x90\x9c\'y\x90\x9c\'z\x90\x9c\'{\x12\xae\x02\n\x1cGetDatasetInputsSearchAddJob\x12\x31.clarifai.api.GetDatasetInputsSearchAddJobRequest\x1a\x35.clarifai.api.SingleDatasetInputsSearchAddJobResponse\"\xa3\x01\x82\xd3\xe4\x93\x02\x94\x01\x12\x62/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\x12,/v2/datasets/inputs/search_add/jobs/{job_id}\x98\x9c\'\x02\x90\x9c\'i\x12\xd6\x01\n\x11ListInputsAddJobs\x12&.clarifai.api.ListInputsAddJobsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"p\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\x15\x12\x13/v2/inputs/jobs/add\x98\x9c\'\x02\x90\x9c\'\x05\x12\xdd\x01\n\x0fGetInputsAddJob\x12$.clarifai.api.GetInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"z\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\x1a\x12\x18/v2/inputs/jobs/add/{id}\x98\x9c\'\x02\x90\x9c\'\x05\x12\xc0\x01\n\x0bPostUploads\x12 .clarifai.api.PostUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"l\x82\xd3\xe4\x93\x02X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10\"\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\x88\x02\n\x15PutUploadContentParts\x12*.clarifai.api.PutUploadContentPartsRequest\x1a\".clarifai.api.SingleUploadResponse\"\x9e\x01\x82\xd3\xe4\x93\x02\x89\x01\x1a[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\x01*Z\'\x1a%/v2/uploads/{upload_id}/content_parts\x98\x9c\'\x02\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\xca\x01\n\tGetUpload\x12\x1e.clarifai.api.GetUploadRequest\x1a\".clarifai.api.SingleUploadResponse\"y\x82\xd3\xe4\x93\x02j\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\x19\x12\x17/v2/uploads/{upload_id}\x98\x9c\'\x02\x90\x9c\'\x80\x01\x12\xb5\x01\n\x0bListUploads\x12 .clarifai.api.ListUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"a\x82\xd3\xe4\x93\x02R\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\x12\x0b/v2/uploads\x98\x9c\'\x02\x90\x9c\'\x80\x01\x12\xc9\x01\n\rDeleteUploads\x12\".clarifai.api.DeleteUploadsRequest\x1a!.clarifai.api.status.BaseResponse\"q\x82\xd3\xe4\x93\x02X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10*\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'\x80\x01\x90\x9c\'\x81\x01\x90\x9c\'\x82\x01\x12\x89\x02\n\x15PostInputsDataSources\x12*.clarifai.api.PostInputsDataSourcesRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9a\x01\x82\xd3\xe4\x93\x02p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\x01*Z\x1c\"\x17/v2/inputs/data_sources:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xae\x02\n\x16GetInputsExtractionJob\x12+.clarifai.api.GetInputsExtractionJobRequest\x1a/.clarifai.api.SingleInputsExtractionJobResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\xa6\x01\x12k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\x12\x35/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\x98\x9c\'\x02\x90\x9c\'\x05\x12\xf9\x01\n\x18ListInputsExtractionJobs\x12-.clarifai.api.ListInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"~\x82\xd3\xe4\x93\x02p\x12P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\x1c\x12\x1a/v2/inputs/jobs/extraction\x98\x9c\'\x02\x90\x9c\'\x05\x12\x88\x02\n\x1a\x43\x61ncelInputsExtractionJobs\x12/.clarifai.api.CancelInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\x01*Z\x1f\x32\x1a/v2/inputs/jobs/extraction:\x01*\x98\x9c\'\x02\x90\x9c\'\x04\x90\x9c\'\x05\x12\x81\x02\n\x11PostInputsUploads\x12&.clarifai.api.PostInputsUploadsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9a\x01\x82\xd3\xe4\x93\x02\x66\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\x01*Z\x17\"\x12/v2/inputs/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n proto/clarifai/api/service.proto\x12\x0c\x63larifai.api\x1a\"proto/clarifai/api/resources.proto\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/auth/scope/scope.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\",\n\nPagination\x12\x0c\n\x04page\x18\x01 \x01(\r\x12\x10\n\x08per_page\x18\x02 \x01(\r\"p\n\x14GetAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rannotation_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb7\x02\n\x16ListAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\x12\x10\n\x08user_ids\x18\t \x03(\t\x12\x19\n\x11model_version_ids\x18\n \x03(\t\x12-\n\x08statuses\x18\x05 \x03(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14list_all_annotations\x18\x06 \x01(\x08\x12\x1b\n\x13return_model_output\x18\x0c \x01(\x08\x12\x0c\n\x04page\x18\x07 \x01(\r\x12\x10\n\x08per_page\x18\x08 \x01(\r\x12\x0f\n\x07task_id\x18\x0b \x01(\tJ\x04\x08\x04\x10\x05\"x\n\x16PostAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\"\x89\x01\n\x17PatchAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\xb9\x01\n\x1dPatchAnnotationsStatusRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0bstatus_code\x18\x02 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\x12\x10\n\x08user_ids\x18\x03 \x03(\t\x12\x0f\n\x07task_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\"v\n\x1ePatchAnnotationsStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08user_ids\x18\x02 \x03(\t\x12\x15\n\rupdated_count\x18\x03 \x01(\r\"s\n\x17\x44\x65leteAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12\x15\n\rannotation_id\x18\x03 \x01(\t\"k\n\x18\x44\x65leteAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"u\n\x18SingleAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12,\n\nannotation\x18\x02 \x01(\x0b\x32\x18.clarifai.api.Annotation\"{\n\x17MultiAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.AnnotationB\x04\x80\xb5\x18\x01\"[\n\rGetAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"\xa5\x02\n\x0fListAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x16\n\x0csort_by_name\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x10\n\x04name\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\tB\t\n\x07sort_by\"c\n\x0fPostAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\"C\n\x10\x44\x65leteAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\xb9\x01\n\x10PatchAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\xb7\x01\n\x0fPatchAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\x81\x01\n\x13PatchAppsIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\xa3\x01\n\x17PostAppsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tapp_query\x18\x02 \x01(\x0b\x32\x16.clarifai.api.AppQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"`\n\x11SingleAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\"f\n\x10MultiAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.AppB\x04\x80\xb5\x18\x01\"\x8b\x01\n\x18ListCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x16list_all_collaborators\x18\x02 \x01(\x08\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x18PostCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\"\x8f\x01\n\x19PatchCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"|\n\x1a\x44\x65leteCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x18\n\x10\x63ollaborator_ids\x18\x02 \x03(\t\x12\x13\n\x0buser_emails\x18\x03 \x03(\t\"\x82\x01\n\x1aMultiCollaboratorsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.CollaboratorB\x04\x80\xb5\x18\x01\"l\n\x19ListCollaborationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x85\x01\n\x1bMultiCollaborationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0e\x63ollaborations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.CollaborationB\x04\x80\xb5\x18\x01\".\n\x14GetStatusCodeRequest\x12\x16\n\x0estatus_code_id\x18\x01 \x01(\t\"\x18\n\x16ListStatusCodesRequest\"G\n\x18SingleStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"u\n\x17MultiStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08statuses\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.status.Status\"X\n\x11GetConceptRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\"f\n\x13ListConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x91\x01\n\x18ListModelConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xaf\x01\n\x1bPostConceptsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rconcept_query\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ConceptQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"o\n\x13PostConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\"\x80\x01\n\x14PatchConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"j\n\x17GetConceptCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x15SingleConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x63oncept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\"r\n\x14MultiConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.ConceptB\x04\x80\xb5\x18\x01\"\x82\x01\n\x19MultiConceptCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x63oncept_counts\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ConceptCountB\x04\x80\xb5\x18\x01\"\xb1\x01\n\x1bListConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x11\n\tpredicate\x18\x03 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\r\x12\x10\n\x08per_page\x18\x06 \x01(\r\"\x9c\x01\n\x1bPostConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_relations\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelation\"q\n\x1d\x44\x65leteConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"M\n\x1aListKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x85\x01\n\x1aPostKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraph\"\x8f\x01\n\x1dPostConceptMappingJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12=\n\x14\x63oncept_mapping_jobs\x18\x02 \x03(\x0b\x32\x1f.clarifai.api.ConceptMappingJob\"\x8b\x01\n\x1cMultiConceptRelationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_relations\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelationB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1bMultiKnowledgeGraphResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraphB\x04\x80\xb5\x18\x01\"Z\n\x1eMultiConceptMappingJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x02 \x03(\t\"r\n\x19GetConceptLanguageRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\x82\x01\n\x1bListConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\xad\x01\n\x1cPatchConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x9c\x01\n\x1bPostConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x85\x01\n\x1dSingleConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10\x63oncept_language\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x8b\x01\n\x1cMultiConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_languages\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguageB\x04\x80\xb5\x18\x01\"T\n\x0fGetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"l\n\x16GetInputSamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9e\x01\n\x11ListInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x04 \x03(\t\"\x92\x01\n\x13StreamInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08per_page\x18\x02 \x01(\r\x12\x0f\n\x07last_id\x18\x03 \x01(\t\x12\x13\n\x0border_by_id\x18\x05 \x01(\x08\x12\x12\n\ndescending\x18\x04 \x01(\x08\"\x84\x01\n\x11PostInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x19\n\x11inputs_add_job_id\x18\x03 \x01(\t\"z\n\x12PatchInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"W\n\x12\x44\x65leteInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"Y\n\x13\x44\x65leteInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\tJ\x04\x08\x03\x10\x04\"f\n\x13SingleInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xa0\x01\n\x12MultiInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.InputB\x04\x80\xb5\x18\x01\x12\x32\n\x0einputs_add_job\x18\x03 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"r\n\x1cMultiInputAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\"q\n\x18SingleInputCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x06\x63ounts\x18\x02 \x01(\x0b\x32\x18.clarifai.api.InputCount\"G\n\x14GetInputCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"f\n\x13ListDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"X\n\x11GetDatasetRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\"o\n\x13PostDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\"\x80\x01\n\x14PatchDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x16PatchDatasetIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0b\x64\x61taset_ids\x18\x02 \x03(\t\"r\n\x14MultiDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.DatasetB\x04\x80\xb5\x18\x01\"l\n\x15SingleDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Dataset\"\x7f\n\x18ListDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"o\n\x16GetDatasetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb9\x01\n\x18PostDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x32\n\x0e\x64\x61taset_inputs\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.DatasetInput\x12$\n\x06search\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\"t\n\x1a\x44\x65leteDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"\xd2\x01\n\x19MultiDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x64\x61taset_inputs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.DatasetInputB\x04\x80\xb5\x18\x01\x12N\n\x1d\x64\x61taset_inputs_search_add_job\x18\x03 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"|\n\x1aSingleDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rdataset_input\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.DatasetInput\"\x81\x01\n\x1aListDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"{\n\x18GetDatasetVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\"\xa4\x02\n&ListDatasetVersionMetricsGroupsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\x12\x14\n\x0cparent_paths\x18\x06 \x03(\t\x12;\n\x05types\x18\x07 \x03(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12&\n\x06values\x18\x08 \x03(\x0b\x32\x16.google.protobuf.Value\"\x99\x01\n\x1aPostDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\"\xaa\x01\n\x1bPatchDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x1c\x44\x65leteDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61taset_version_ids\x18\x03 \x03(\t\"\xb7\x01\n\x1fPutDatasetVersionExportsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x33\n\x07\x65xports\x18\x04 \x03(\x0b\x32\".clarifai.api.DatasetVersionExport\"\x88\x01\n\x1bMultiDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10\x64\x61taset_versions\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersionB\x04\x80\xb5\x18\x01\"\x8b\x01\n!MultiDatasetVersionExportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x07\x65xports\x18\x02 \x03(\x0b\x32\".clarifai.api.DatasetVersionExportB\x04\x80\xb5\x18\x01\"\xae\x01\n\'MultiDatasetVersionMetricsGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12V\n\x1e\x64\x61taset_version_metrics_groups\x18\x02 \x03(\x0b\x32(.clarifai.api.DatasetVersionMetricsGroupB\x04\x80\xb5\x18\x01\"\x82\x01\n\x1cSingleDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x64\x61taset_version\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\"f\n#GetDatasetInputsSearchAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06job_id\x18\x02 \x01(\t\"\x8c\x01\n\'SingleDatasetInputsSearchAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x03job\x18\x02 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"\xb9\x01\n\x17PostModelOutputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12\"\n\x05model\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Model\"\x8f\x01\n\x16ListModelInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"P\n\rGetKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"\x9a\x01\n\x0fListKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x13\n\x0bnot_expired\x18\x04 \x01(\x08\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x11\n\tendpoints\x18\x06 \x03(\t\"e\n\x12ListAppKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"c\n\x0fPostKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\"S\n\x10\x44\x65leteKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"t\n\x10PatchKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"`\n\x11SingleKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03key\x18\x02 \x01(\x0b\x32\x11.clarifai.api.Key\"f\n\x10MultiKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.KeyB\x04\x80\xb5\x18\x01\"\xad\x01\n\x0fGetModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x16\n\x0etrained_before\x18\x05 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\"\xa3\x04\n\x11ListModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\n \x01(\x08\x12\x16\n\x0csort_by_name\x18\x0b \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\x0c \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\r \x01(\x08H\x00\x12\r\n\x05query\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x19\n\x11\x66ilter_by_user_id\x18\x16 \x01(\x08\x12\x15\n\rmodel_type_id\x18\x06 \x01(\t\x12\x14\n\x0ctrained_only\x18\x07 \x01(\x08\x12\x14\n\x0cinput_fields\x18\x08 \x03(\t\x12\x15\n\routput_fields\x18\t \x03(\t\x12\x0f\n\x07license\x18\x0f \x01(\t\x12\x15\n\rfeatured_only\x18\x10 \x01(\x08\x12\x14\n\x0cstarred_only\x18\x14 \x01(\x08\x12\x10\n\x08toolkits\x18\x11 \x03(\t\x12\x11\n\tuse_cases\x18\x12 \x03(\t\x12\x11\n\tlanguages\x18\x15 \x03(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\x12\x1c\n\x14\x64ont_fetch_from_main\x18\x17 \x01(\x08\x42\t\n\x07sort_byJ\x04\x08\x04\x10\x05\"\x80\x01\n\x19PatchModelToolkitsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08toolkits\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1ePatchModelCheckConsentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x16\n\x0e\x63heck_consents\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x19PatchModelUseCasesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08usecases\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x82\x01\n\x1aPatchModelLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x11\n\tlanguages\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"Z\n\x19MultiModelToolkitResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08toolkits\x18\x02 \x03(\t\"e\n\x1eMultiModelCheckConsentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x16\n\x0e\x63heck_consents\x18\x02 \x03(\t\"Z\n\x19MultiModelUseCaseResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08usecases\x18\x02 \x03(\t\"\\\n\x1aMultiModelLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x11\n\tlanguages\x18\x02 \x03(\t\"\x91\x01\n\x11PostModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ModelB\x02\x18\x01\x12#\n\x06models\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Model\"z\n\x12PatchModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Model\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\",\n\x0eIdUpdateSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06new_id\x18\x02 \x01(\t\"\x82\x01\n\x14PatchModelIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"W\n\x12\x44\x65leteModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\"g\n\x13\x44\x65leteModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\xa9\x01\n\x19PostModelsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0bmodel_query\x18\x02 \x01(\x0b\x32\x18.clarifai.api.ModelQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"f\n\x13SingleModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\"l\n\x12MultiModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.ModelB\x04\x80\xb5\x18\x01\"\xa2\x01\n\x19PatchModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"o\n\x16GetModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\"\xc5\x02\n\x18ListModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\x12\x13\n\x0b\x63oncept_ids\x18\x05 \x03(\t\x12\x14\n\x0ctrained_only\x18\x06 \x01(\x08\x12\x16\n\x0esort_ascending\x18\x07 \x01(\x08\x12\x1d\n\x13sort_by_status_code\x18\x08 \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\t \x01(\x08H\x00\x12\x1d\n\x13sort_by_description\x18\n \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\x0b \x01(\x08H\x00\x42\t\n\x07sort_by\"r\n\x19\x44\x65leteModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x12\n\nversion_id\x18\x04 \x01(\t\"|\n\x1aSingleModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rmodel_version\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\"\x82\x01\n\x19MultiModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0emodel_versions\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ModelVersionB\x04\x80\xb5\x18\x01\"\xef\x01\n\x18PostModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\t\x10\n\"\xb1\x01\n$PostWorkflowVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x43\n\x0cpublications\x18\x03 \x03(\x0b\x32-.clarifai.api.WorkflowVersionUnPublishRequest\"\xad\x01\n\"PostWorkflowVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x41\n\x0cpublications\x18\x03 \x03(\x0b\x32+.clarifai.api.WorkflowVersionPublishRequest\"3\n\x1dWorkflowVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"5\n\x1fWorkflowVersionUnPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"0\n\x1aModelVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa4\x01\n\x1fPostModelVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12>\n\x0cpublications\x18\x03 \x03(\x0b\x32(.clarifai.api.ModelVersionPublishRequest\"2\n\x1cModelVersionUnpublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa8\x01\n!PostModelVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12@\n\x0cpublications\x18\x03 \x03(\x0b\x32*.clarifai.api.ModelVersionUnpublishRequest\"\xb2\x01\n\"PostModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12/\n\x0c\x65val_metrics\x18\x04 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xa1\x01\n\"ListModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xc1\x01\n GetModelVersionEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x15\n\revaluation_id\x18\x04 \x01(\t\x12)\n\x06\x66ields\x18\x05 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"y\n\x19SingleEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\"x\n\x18MultiEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xd3\x01\n\x1ePostModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x0btest_search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05\"\xa1\x01\n\x1dGetModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"]\n\x13GetModelTypeRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rmodel_type_id\x18\x02 \x01(\t\"h\n\x15ListModelTypesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x1f\n\x1dListOpenSourceLicensesRequest\"_\n\x1eListOpenSourceLicensesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08licenses\x18\x02 \x03(\t\"y\n\x17SingleModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\nmodel_type\x18\x02 \x01(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\"\xf2\x01\n\x16MultiModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bmodel_types\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\x12\x35\n\x0fmodel_importers\x18\x03 \x01(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12@\n\x16triton_conda_envs_info\x18\x04 \x03(\x0b\x32 .clarifai.api.TritonCondaEnvInfo\"\x95\x01\n\"GetModelVersionInputExampleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x12\n\nexample_id\x18\x04 \x01(\t\"\xa3\x01\n$ListModelVersionInputExamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xa2\x01\n&SingleModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12K\n\x1bmodel_version_input_example\x18\x02 \x01(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\xa2\x01\n%MultiModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cmodel_version_input_examples\x18\x02 \x03(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\x7f\n\x1aListModelReferencesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x82\x01\n\x1bMultiModelReferenceResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10model_references\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.ModelReference\"o\n\x13MultiOutputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07outputs\x18\x02 \x03(\x0b\x32\x14.clarifai.api.OutputB\x04\x80\xb5\x18\x01\"V\n\x11ListScopesRequest\x12\x10\n\x08key_type\x18\x01 \x01(\t\x12/\n\x0buser_app_id\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"B\n\x0fMyScopesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"F\n\x13MyScopesUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x15\n\x13MyScopesRootRequest\"\xa5\x01\n\x16MultiScopeDepsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\nscope_deps\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ScopeDeps\x12\x31\n\rendpoint_deps\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.EndpointDeps\"\xa0\x01\n\x12MultiScopeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x1e\n\x03\x61pp\x18\x03 \x01(\x0b\x32\x11.clarifai.api.App\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeRootResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"O\n\x10GetSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x13ListSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\xc4\x01\n\x13PostSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05query\x18\x02 \x01(\x0b\x32\x13.clarifai.api.QueryB\x02\x18\x01\x12&\n\x08searches\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Pagination\"\x85\x01\n\x1aPatchInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x8a\x01\n\x1fPatchAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x7f\n\x14PatchSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x17PostSearchesByIDRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"R\n\x13\x44\x65leteSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xa7\x01\n\x1ePostAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"c\n$DeleteAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xb6\x01\n\x19PostInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\x12\x12\n\nonly_count\x18\x04 \x01(\x08\"i\n\x14SingleSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\"\xed\x01\n\x13MultiSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\x12\"\n\x05query\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Query\x12&\n\x08searches\x18\x05 \x03(\x0b\x32\x14.clarifai.api.Search\x12*\n\nhit_counts\x18\x06 \x03(\x0b\x32\x16.clarifai.api.HitCount\"\x94\x02\n\"PostAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12*\n\x0cground_truth\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\x12 \n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x35\n\x0f\x65valuation_type\x18\x06 \x01(\x0e\x32\x1c.clarifai.api.EvaluationType\"`\n!GetAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"U\n\"ListAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x9d\x01\n$MultiAnnotationSearchMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12H\n\x19\x61nnotation_search_metrics\x18\x02 \x03(\x0b\x32%.clarifai.api.AnnotationSearchMetrics\"o\n\x1cListAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"k\n\x1aGetAnnotationFilterRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1c\n\x14\x61nnotation_filter_id\x18\x02 \x01(\t\"\x8b\x01\n\x1cPostAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\x9c\x01\n\x1dPatchAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"p\n\x1e\x44\x65leteAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1d\n\x15\x61nnotation_filter_ids\x18\x02 \x03(\t\"\x8e\x01\n\x1dMultiAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilterB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1eSingleAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x11\x61nnotation_filter\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\\\n\x0eGetUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"c\n\x12SingleUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04user\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\"x\n\x1bPostValidatePasswordRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12(\n\x08password\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Password\"\x8e\x01\n SinglePasswordValidationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12=\n\x13password_violations\x18\x02 \x01(\x0b\x32 .clarifai.api.PasswordViolations\"\xbb\x01\n\x12GetWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x03 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x04 \x03(\t\x12\"\n\x1a\x65xclude_clarifai_workflows\x18\x05 \x01(\x08\"\xbb\x02\n\x14ListWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x14\n\nsort_by_id\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x0e\n\x02id\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\t\x12\x13\n\x0bsearch_term\x18\x0c \x01(\tB\t\n\x07sort_by\"r\n\x14PostWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\"\x83\x01\n\x15PatchWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x85\x01\n\x17PatchWorkflowIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\"j\n\x16\x44\x65leteWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"o\n\x16SingleWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\"u\n\x15MultiWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.WorkflowB\x04\x80\xb5\x18\x01\"\xa5\x02\n\x1aPostWorkflowResultsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12#\n\x06inputs\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\routput_config\x18\x04 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x05 \x01(\x08\x12\x33\n\x0eworkflow_state\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\xd8\x01\n\x1bPostWorkflowResultsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12-\n\x07results\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.WorkflowResult\x12\x33\n\x0eworkflow_state\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\x91\x02\n$PostWorkflowResultsSimilarityRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12)\n\x0cprobe_inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12(\n\x0bpool_inputs\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Input\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x06 \x01(\x08\"\x8e\x01\n%PostWorkflowResultsSimilarityResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x07results\x18\x02 \x03(\x0b\x32\'.clarifai.api.WorkflowResultsSimilarity\"\x83\x01\n\x1bListWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x19GetWorkflowVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x03 \x01(\t\"\x83\x01\n\x1d\x44\x65leteWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1c\n\x14workflow_version_ids\x18\x03 \x03(\t\"\xae\x01\n\x1cPatchWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x38\n\x11workflow_versions\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1cMultiWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11workflow_versions\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersionB\x04\x80\xb5\x18\x01\"\x85\x01\n\x1dSingleWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10workflow_version\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\"\x85\x01\n\x1aPostAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"g\n\x18GetAppDuplicationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1a\n\x12\x61pp_duplication_id\x18\x02 \x01(\t\"m\n\x1aListAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x83\x01\n\x1cMultiAppDuplicationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"\x82\x01\n\x1cSingleAppDuplicationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x61pp_duplication\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.AppDuplication\"f\n\x10PostTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\"m\n\x0eGetTaskRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\xee\x01\n\x10ListTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x17\n\x0fworker_user_ids\x18\x04 \x03(\t\x12\x17\n\x0freview_user_ids\x18\x05 \x03(\t\x12\x17\n\x0flabel_order_ids\x18\x08 \x03(\t\x12#\n\x1bincluding_label_order_tasks\x18\x06 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x07 \x03(\t\"w\n\x11PatchTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"R\n\x12\x44\x65leteTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x11MultiTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\'\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.TaskB\x04\x80\xb5\x18\x01\"c\n\x12SingleTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04task\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Task\"i\n\x13GetTaskCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9d\x01\n\x17SingleTaskCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0f\n\x07task_id\x18\x03 \x01(\t\x12\x34\n\x06\x63ounts\x18\x04 \x03(\x0b\x32$.clarifai.api.TaskStatusCountPerUser\"y\n\x16PostLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\"_\n\x14GetLabelOrderRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x16\n\x0elabel_order_id\x18\x02 \x01(\t\"i\n\x16ListLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x8a\x01\n\x17PatchLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"X\n\x18\x44\x65leteLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"|\n\x17MultiLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrderB\x04\x80\xb5\x18\x01\"v\n\x18SingleLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x0blabel_order\x18\x02 \x01(\x0b\x32\x18.clarifai.api.LabelOrder\"u\n\x15PostCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"\x86\x01\n\x16PatchCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"k\n\x17\x44\x65leteCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\\\n\x13GetCollectorRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x14\n\x0c\x63ollector_id\x18\x02 \x01(\t\"h\n\x15ListCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"r\n\x16MultiCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"r\n\x17SingleCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12*\n\tcollector\x18\x02 \x01(\x0b\x32\x17.clarifai.api.Collector\"v\n\x15PostStatValuesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12,\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValue\"y\n\x16MultiStatValueResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValueB\x04\x80\xb5\x18\x01\"\x9e\x01\n\x1ePostStatValuesAggregateRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12K\n\x1cstat_value_aggregate_queries\x18\x02 \x03(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"\x9c\x01\n\x1fMultiStatValueAggregateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cstat_value_aggregate_results\x18\x02 \x03(\x0b\x32&.clarifai.api.StatValueAggregateResult\"w\n\x1ePostTrendingMetricsViewRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\"\x85\x01\n\x1fListTrendingMetricsViewsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n MultiTrendingMetricsViewResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x07metrics\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.TrendingMetric\"V\n\x10GetModuleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\"e\n\x12ListModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x12PostModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Module\"}\n\x13PatchModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Module\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"T\n\x14\x44\x65leteModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x14SingleModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06module\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Module\"o\n\x13MultiModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.ModuleB\x04\x80\xb5\x18\x01\"x\n\x17GetModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11module_version_id\x18\x03 \x01(\t\"\x7f\n\x19ListModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x95\x01\n\x19PostModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x34\n\x0fmodule_versions\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersion\"n\n\x1b\x44\x65leteModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"\x7f\n\x1bSingleModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\"\x85\x01\n\x1aMultiModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12:\n\x0fmodule_versions\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersionB\x04\x80\xb5\x18\x01\"x\n GetInstalledModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"u\n\"ListInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x9e\x01\n\"PostInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12G\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersion\"}\n%PostInstalledModuleVersionsKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"d\n$DeleteInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x9b\x01\n$SingleInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x46\n\x18installed_module_version\x18\x02 \x01(\x0b\x32$.clarifai.api.InstalledModuleVersion\"\xa1\x01\n#MultiInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12M\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersionB\x04\x80\xb5\x18\x01\"b\n\x1eListNextTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\x82\x01\n\x19PostBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0f\x62ulk_operations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"l\n\x19ListBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x17GetBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"Z\n\x1a\x43\x61ncelBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"Z\n\x1a\x44\x65leteBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x80\x01\n\x1cSingleBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.BulkOperation\"\x7f\n\x1bMultiBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"o\n\x19PutTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"k\n\x18ListInputsAddJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"U\n\x16GetInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\x83\x01\n\x19MultiInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0finputs_add_jobs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsAddJobB\x04\x80\xb5\x18\x01\"}\n\x1aSingleInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0einputs_add_job\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"l\n\x12PostUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"T\n\x14\x44\x65leteUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"e\n\x12ListUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x10GetUploadRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\"i\n\x14SingleUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06upload\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Upload\"i\n\x13MultiUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"\x9a\x01\n\x1cPutUploadContentPartsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\x12\x36\n\rcontent_parts\x18\x03 \x03(\x0b\x32\x1f.clarifai.api.UploadContentPart\"\xad\x01\n\x1cPostInputsDataSourcesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.InputsDataSource\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\"r\n\x1dGetInputsExtractionJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12 \n\x18inputs_extraction_job_id\x18\x02 \x01(\t\"r\n\x1fListInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x92\x01\n!SingleInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x15inputs_extraction_job\x18\x02 \x01(\x0b\x32!.clarifai.api.InputsExtractionJob\"\x92\x01\n MultiInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x41\n\x16inputs_extraction_jobs\x18\x02 \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\"a\n!CancelInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x7f\n\x18PostInputsUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x32\n\x0einputs_uploads\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsUpload*p\n\x1cOrganizationInvitationStatus\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x02\x12\r\n\tCANCELLED\x10\x03\x12\x0c\n\x08\x44\x45\x43LINED\x10\x04\x12\x0b\n\x07\x45XPIRED\x10\x05\x32\x97\xf3\x02\n\x02V2\x12\xaa\x02\n\x14ListConceptRelations\x12).clarifai.api.ListConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"\xba\x01\x82\xd3\xe4\x93\x02\xab\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\x98\x9c\'\x05\x90\x9c\'\x0b\x12\xdf\x01\n\x14PostConceptRelations\x12).clarifai.api.PostConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"p\x82\xd3\xe4\x93\x02^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'\n\x90\x9c\'\x0b\x12\xde\x01\n\x16\x44\x65leteConceptRelations\x12+.clarifai.api.DeleteConceptRelationsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'\r\x90\x9c\'\n\x90\x9c\'\x0b\x12\xdc\x01\n\x10GetConceptCounts\x12%.clarifai.api.GetConceptCountsRequest\x1a\'.clarifai.api.MultiConceptCountResponse\"x\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\x15\x12\x13/v2/concepts/status\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd0\x01\n\nGetConcept\x12\x1f.clarifai.api.GetConceptRequest\x1a#.clarifai.api.SingleConceptResponse\"|\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\x1b\x12\x19/v2/concepts/{concept_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xb9\x01\n\x0cListConcepts\x12!.clarifai.api.ListConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"b\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\x0e\x12\x0c/v2/concepts\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xb9\x02\n\x11ListModelConcepts\x12&.clarifai.api.ListModelConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"\xd7\x01\x82\xd3\xe4\x93\x02\xc4\x01\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xea\x01\n\x14PostConceptsSearches\x12).clarifai.api.PostConceptsSearchesRequest\x1a\".clarifai.api.MultiConceptResponse\"\x82\x01\x82\xd3\xe4\x93\x02l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\x01*Z\x1a\"\x15/v2/concepts/searches:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xc3\x01\n\x0cPostConcepts\x12!.clarifai.api.PostConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"l\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\"\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xc5\x01\n\rPatchConcepts\x12\".clarifai.api.PatchConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"l\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\x32\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x94\x02\n\x12GetConceptLanguage\x12\'.clarifai.api.GetConceptLanguageRequest\x1a+.clarifai.api.SingleConceptLanguageResponse\"\xa7\x01\x82\xd3\xe4\x93\x02\x98\x01\x12\x64/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\x12./v2/concepts/{concept_id}/languages/{language}\x98\x9c\'\x02\x90\x9c\'\x0b\x12\x81\x02\n\x14ListConceptLanguages\x12).clarifai.api.ListConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x91\x01\x82\xd3\xe4\x93\x02\x82\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\x12#/v2/concepts/{concept_id}/languages\x98\x9c\'\x02\x90\x9c\'\x0b\x12\x8b\x02\n\x14PostConceptLanguages\x12).clarifai.api.PostConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(\"#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x8d\x02\n\x15PatchConceptLanguages\x12*.clarifai.api.PatchConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x88\x01\x32Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(2#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xf1\x01\n\x13ListKnowledgeGraphs\x12(.clarifai.api.ListKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\x1f\x12\x1d/v2/concepts/knowledge_graphs\x98\x9c\'\x02\x90\x9c\'\x0b\x12\xfb\x01\n\x13PostKnowledgeGraphs\x12(.clarifai.api.PostKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\x01*Z\"\"\x1d/v2/concepts/knowledge_graphs:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\xfe\x01\n\x16PostConceptMappingJobs\x12+.clarifai.api.PostConceptMappingJobsRequest\x1a,.clarifai.api.MultiConceptMappingJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\x01*Z\x1f\"\x1a/v2/concepts/mappings/jobs:\x01*\x98\x9c\'\x02\x90\x9c\'\n\x90\x9c\'\x0b\x12\x93\x02\n\rGetAnnotation\x12\".clarifai.api.GetAnnotationRequest\x1a&.clarifai.api.SingleAnnotationResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\x9e\x01\x12g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\x12\x31/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xd0\x01\n\x0fListAnnotations\x12$.clarifai.api.ListAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"p\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\x11\x12\x0f/v2/annotations\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe3\x01\n\x0fPostAnnotations\x12$.clarifai.api.PostAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x82\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\"\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe5\x01\n\x10PatchAnnotations\x12%.clarifai.api.PatchAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x82\x01\x82\xd3\xe4\x93\x02`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\x32\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf3\x01\n\x16PatchAnnotationsStatus\x12+.clarifai.api.PatchAnnotationsStatusRequest\x1a,.clarifai.api.PatchAnnotationsStatusResponse\"~\x82\xd3\xe4\x93\x02`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\x9c\x02\n\x10\x44\x65leteAnnotation\x12%.clarifai.api.DeleteAnnotationRequest\x1a!.clarifai.api.status.BaseResponse\"\xbd\x01\x82\xd3\xe4\x93\x02\x9e\x01*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd0\x02\n\x11\x44\x65leteAnnotations\x12&.clarifai.api.DeleteAnnotationsRequest\x1a!.clarifai.api.status.BaseResponse\"\xef\x01\x82\xd3\xe4\x93\x02\xd0\x01*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\x01*Z\x1b*\x16/v2/inputs/annotations:\x01*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14*\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf3\x01\n\x18PatchAnnotationsSearches\x12-.clarifai.api.PatchAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x84\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\x32\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\x81\x02\n\x17PostAnnotationsSearches\x12,.clarifai.api.PostAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x94\x01\x82\xd3\xe4\x93\x02r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\"\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd1\x01\n\rGetInputCount\x12\".clarifai.api.GetInputCountRequest\x1a&.clarifai.api.SingleInputCountResponse\"t\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\x13\x12\x11/v2/inputs/status\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xc9\x01\n\x0cStreamInputs\x12!.clarifai.api.StreamInputsRequest\x1a .clarifai.api.MultiInputResponse\"t\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\x13\x12\x11/v2/inputs/stream\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xfd\x01\n\x0fGetInputSamples\x12$.clarifai.api.GetInputSamplesRequest\x1a*.clarifai.api.MultiInputAnnotationResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\x12\"/v2/tasks/{task_id}/inputs/samples\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xca\x01\n\x08GetInput\x12\x1d.clarifai.api.GetInputRequest\x1a!.clarifai.api.SingleInputResponse\"|\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17\x12\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xb7\x01\n\nListInputs\x12\x1f.clarifai.api.ListInputsRequest\x1a .clarifai.api.MultiInputResponse\"f\x82\xd3\xe4\x93\x02P\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\x0c\x12\n/v2/inputs\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd2\x01\n\nPostInputs\x12\x1f.clarifai.api.PostInputsRequest\x1a .clarifai.api.MultiInputResponse\"\x80\x01\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\"\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xcb\x01\n\x0bPatchInputs\x12 .clarifai.api.PatchInputsRequest\x1a .clarifai.api.MultiInputResponse\"x\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\x32\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x12\xe5\x01\n\x0b\x44\x65leteInput\x12 .clarifai.api.DeleteInputRequest\x1a!.clarifai.api.status.BaseResponse\"\x90\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17*\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xd7\x01\n\x0c\x44\x65leteInputs\x12!.clarifai.api.DeleteInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f*\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xde\x01\n\x13PatchInputsSearches\x12(.clarifai.api.PatchInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"z\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\x32\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\xed\x01\n\x12PostInputsSearches\x12\'.clarifai.api.PostInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\"\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\x9c\x03\n\x10PostModelOutputs\x12%.clarifai.api.PostModelOutputsRequest\x1a!.clarifai.api.MultiOutputResponse\"\xbd\x02\x82\xd3\xe4\x93\x02\xa6\x02\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\x01*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\x01*Z\"\"\x1d/v2/models/{model_id}/outputs:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x02\x12\xbd\x01\n\x0cListDatasets\x12!.clarifai.api.ListDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ\x0e\x12\x0c/v2/datasets\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xd5\x01\n\nGetDataset\x12\x1f.clarifai.api.GetDatasetRequest\x1a#.clarifai.api.SingleDatasetResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\x1b\x12\x19/v2/datasets/{dataset_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xc7\x01\n\x0cPostDatasets\x12!.clarifai.api.PostDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"p\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\"\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xc9\x01\n\rPatchDatasets\x12\".clarifai.api.PatchDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\x32\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xba\x01\n\x0fPatchDatasetIds\x12$.clarifai.api.PatchDatasetIdsRequest\x1a\".clarifai.api.MultiDatasetResponse\"]\x82\xd3\xe4\x93\x02K2F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/ids:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\xca\x01\n\x0e\x44\x65leteDatasets\x12#.clarifai.api.DeleteDatasetsRequest\x1a!.clarifai.api.status.BaseResponse\"p\x82\xd3\xe4\x93\x02Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11*\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xfd\x01\n\x11ListDatasetInputs\x12&.clarifai.api.ListDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\x96\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\x12 /v2/datasets/{dataset_id}/inputs\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x91\x02\n\x0fGetDatasetInput\x12$.clarifai.api.GetDatasetInputRequest\x1a(.clarifai.api.SingleDatasetInputResponse\"\xad\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\x12+/v2/datasets/{dataset_id}/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x88\x02\n\x11PostDatasetInputs\x12&.clarifai.api.PostDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%\" /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x82\x02\n\x13\x44\x65leteDatasetInputs\x12(.clarifai.api.DeleteDatasetInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x82\x01*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%* /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x90\x9c\'\x05\x12\x80\x02\n\x13ListDatasetVersions\x12(.clarifai.api.ListDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\x12\"/v2/datasets/{dataset_id}/versions\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xa7\x02\n\x11GetDatasetVersion\x12&.clarifai.api.GetDatasetVersionRequest\x1a*.clarifai.api.SingleDatasetVersionResponse\"\xbd\x01\x82\xd3\xe4\x93\x02\xaa\x01\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\x12\x37/v2/datasets/{dataset_id}/versions/{dataset_version_id}\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'r\x12\xe6\x02\n\x1fListDatasetVersionMetricsGroups\x12\x34.clarifai.api.ListDatasetVersionMetricsGroupsRequest\x1a\x35.clarifai.api.MultiDatasetVersionMetricsGroupResponse\"\xd5\x01\x82\xd3\xe4\x93\x02\xba\x01\x12u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\x12?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x8e\x02\n\x13PostDatasetVersions\x12(.clarifai.api.PostDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'\"\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x88\x02\n\x14PatchDatasetVersions\x12).clarifai.api.PatchDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x86\x01\x32X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'2\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\x86\x02\n\x15\x44\x65leteDatasetVersions\x12*.clarifai.api.DeleteDatasetVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'*\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xd0\x02\n\x18PutDatasetVersionExports\x12-.clarifai.api.PutDatasetVersionExportsRequest\x1a/.clarifai.api.MultiDatasetVersionExportResponse\"\xd3\x01\x82\xd3\xe4\x93\x02\xc0\x01\x1au/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*ZD\x1a?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'j\x12\xe5\x01\n\x0cGetModelType\x12!.clarifai.api.GetModelTypeRequest\x1a%.clarifai.api.SingleModelTypeResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\x12 /v2/models/types/{model_type_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x12\x99\x01\n\x16ListOpenSourceLicenses\x12+.clarifai.api.ListOpenSourceLicensesRequest\x1a,.clarifai.api.ListOpenSourceLicensesResponse\"$\x82\xd3\xe4\x93\x02\x1a\x12\x18/v2/open_source_licenses\x98\x9c\'\x01\x12\xc7\x01\n\x0eListModelTypes\x12#.clarifai.api.ListModelTypesRequest\x1a$.clarifai.api.MultiModelTypeResponse\"j\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\x12\x12\x10/v2/models/types\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xc6\x01\n\x08GetModel\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"x\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17\x12\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\x96\x03\n\x12GetModelOutputInfo\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"\xbd\x02\x82\xd3\xe4\x93\x02\xaa\x02\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\x12!/v2/models/{model_id}/output_infoZo\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\x12\x37/v2/models/{model_id}/versions/{version_id}/output_info\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xde\x01\n\nListModels\x12\x1f.clarifai.api.ListModelsRequest\x1a .clarifai.api.MultiModelResponse\"\x8c\x01\x82\xd3\xe4\x93\x02z\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\x12&/v2/users/{user_app_id.user_id}/modelsZ\x0c\x12\n/v2/models\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xdb\x01\n\x12PostModelsSearches\x12\'.clarifai.api.PostModelsSearchesRequest\x1a .clarifai.api.MultiModelResponse\"z\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\x01*Z\x18\"\x13/v2/models/searches:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xc6\x01\n\nPostModels\x12\x1f.clarifai.api.PostModelsRequest\x1a!.clarifai.api.SingleModelResponse\"t\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\"\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x12\xc3\x01\n\x0bPatchModels\x12 .clarifai.api.PatchModelsRequest\x1a .clarifai.api.MultiModelResponse\"p\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\x32\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x12\xb2\x01\n\rPatchModelIds\x12\".clarifai.api.PatchModelIdsRequest\x1a .clarifai.api.MultiModelResponse\"[\x82\xd3\xe4\x93\x02I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\x01*\x98\x9c\'\x02\x90\x9c\'\x0e\x90\x9c\'\x0f\x12\xd9\x01\n\x0b\x44\x65leteModel\x12 .clarifai.api.DeleteModelRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17*\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xca\x01\n\x0c\x44\x65leteModels\x12!.clarifai.api.DeleteModelsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f*\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x91\x02\n\x17PatchModelCheckConsents\x12,.clarifai.api.PatchModelCheckConsentsRequest\x1a,.clarifai.api.MultiModelCheckConsentResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\x01*Z)2$/v2/models/{model_id}/check_consents:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xf5\x01\n\x12PatchModelToolkits\x12\'.clarifai.api.PatchModelToolkitsRequest\x1a\'.clarifai.api.MultiModelToolkitResponse\"\x8c\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\x01*Z#2\x1e/v2/models/{model_id}/toolkits:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xf5\x01\n\x12PatchModelUseCases\x12\'.clarifai.api.PatchModelUseCasesRequest\x1a\'.clarifai.api.MultiModelUseCaseResponse\"\x8c\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\x01*Z#2\x1e/v2/models/{model_id}/usecases:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xfb\x01\n\x13PatchModelLanguages\x12(.clarifai.api.PatchModelLanguagesRequest\x1a(.clarifai.api.MultiModelLanguageResponse\"\x8f\x01\x82\xd3\xe4\x93\x02\x80\x01\x32U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\x01*Z$2\x1f/v2/models/{model_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x12\x8d\x03\n\x0fListModelInputs\x12$.clarifai.api.ListModelInputsRequest\x1a .clarifai.api.MultiInputResponse\"\xb1\x02\x82\xd3\xe4\x93\x02\x96\x02\x12R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\x1e\x12\x1c/v2/models/{model_id}/inputsZj\x12h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\x12\x32/v2/models/{model_id}/versions/{version_id}/inputs\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x12\x89\x02\n\x0fGetModelVersion\x12$.clarifai.api.GetModelVersionRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\x12+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xf1\x01\n\x11ListModelVersions\x12&.clarifai.api.ListModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"\x8a\x01\x82\xd3\xe4\x93\x02x\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \x12\x1e/v2/models/{model_id}/versions\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xb8\x02\n\x1dPostWorkflowVersionsUnPublish\x12\x32.clarifai.api.PostWorkflowVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbf\x01\x82\xd3\xe4\x93\x02\x8c\x01\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\x01*Z*\"%/v2/workflows/{workflow_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'x\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xb0\x02\n\x1bPostWorkflowVersionsPublish\x12\x30.clarifai.api.PostWorkflowVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbb\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\x01*Z(\"#/v2/workflows/{workflow_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'w\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x9d\x02\n\x18PostModelVersionsPublish\x12-.clarifai.api.PostModelVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xae\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\x01*Z\"\"\x1d/v2/models/{model_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'u\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xa6\x02\n\x1aPostModelVersionsUnPublish\x12/.clarifai.api.PostModelVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb3\x01\x82\xd3\xe4\x93\x02\x80\x01\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\x01*Z$\"\x1f/v2/models/{model_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'v\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x8d\x02\n\x11PostModelVersions\x12&.clarifai.api.PostModelVersionsRequest\x1a!.clarifai.api.SingleModelResponse\"\xac\x01\x82\xd3\xe4\x93\x02~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*Z#\"\x1e/v2/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdb\x01\n\x12PatchModelVersions\x12\'.clarifai.api.PatchModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"s\x82\xd3\xe4\x93\x02Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x0e\x90\x9c\'\x1a\x12\x94\x02\n\x12\x44\x65leteModelVersion\x12\'.clarifai.api.DeleteModelVersionRequest\x1a!.clarifai.api.status.BaseResponse\"\xb1\x01\x82\xd3\xe4\x93\x02\x92\x01*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb3\x02\n\x16GetModelVersionMetrics\x12+.clarifai.api.GetModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\xa2\x01\x12i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\x12\x33/v2/models/{model_id}/versions/{version_id}/metrics\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xcf\x02\n\x17PostModelVersionMetrics\x12,.clarifai.api.PostModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xdb\x01\x82\xd3\xe4\x93\x02\xa8\x01\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xe9\x02\n\x1bPostModelVersionEvaluations\x12\x30.clarifai.api.PostModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xef\x01\x82\xd3\xe4\x93\x02\xbc\x01\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\x01*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xcf\x02\n\x1bListModelVersionEvaluations\x12\x30.clarifai.api.ListModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xd5\x01\x82\xd3\xe4\x93\x02\xb6\x01\x12s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\x12=/v2/models/{model_id}/versions/{model_version_id}/evaluations\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xed\x02\n\x19GetModelVersionEvaluation\x12..clarifai.api.GetModelVersionEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\xf6\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf7\x01\n\x13ListModelReferences\x12(.clarifai.api.ListModelReferencesRequest\x1a).clarifai.api.MultiModelReferenceResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\x12 /v2/models/{model_id}/references\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xee\x02\n\x1bGetModelVersionInputExample\x12\x30.clarifai.api.GetModelVersionInputExampleRequest\x1a\x34.clarifai.api.SingleModelVersionInputExampleResponse\"\xe6\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xd6\x02\n\x1dListModelVersionInputExamples\x12\x32.clarifai.api.ListModelVersionInputExamplesRequest\x1a\x33.clarifai.api.MultiModelVersionInputExampleResponse\"\xcb\x01\x82\xd3\xe4\x93\x02\xbc\x01\x12v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\x12@/v2/models/{model_id}/versions/{model_version_id}/input_examples\x98\x9c\'\x02\x90\x9c\'\x0f\x12\xdc\x01\n\x0bGetWorkflow\x12 .clarifai.api.GetWorkflowRequest\x1a$.clarifai.api.SingleWorkflowResponse\"\x84\x01\x82\xd3\xe4\x93\x02r\x12Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d\x12\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xf1\x01\n\rListWorkflows\x12\".clarifai.api.ListWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"\x96\x01\x82\xd3\xe4\x93\x02\x83\x01\x12\x43/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\x12)/v2/users/{user_app_id.user_id}/workflowsZ\x0f\x12\r/v2/workflows\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xcc\x01\n\rPostWorkflows\x12\".clarifai.api.PostWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"r\x82\xd3\xe4\x93\x02\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\"\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xce\x01\n\x0ePatchWorkflows\x12#.clarifai.api.PatchWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"r\x82\xd3\xe4\x93\x02\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\x32\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xbe\x01\n\x10PatchWorkflowIds\x12%.clarifai.api.PatchWorkflowIdsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"^\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\x01*\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x13\x12\xe3\x01\n\x0e\x44\x65leteWorkflow\x12#.clarifai.api.DeleteWorkflowRequest\x1a!.clarifai.api.status.BaseResponse\"\x88\x01\x82\xd3\xe4\x93\x02r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d*\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\xce\x01\n\x0f\x44\x65leteWorkflows\x12$.clarifai.api.DeleteWorkflowsRequest\x1a!.clarifai.api.status.BaseResponse\"r\x82\xd3\xe4\x93\x02\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12*\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\x86\x03\n\x13PostWorkflowResults\x12(.clarifai.api.PostWorkflowResultsRequest\x1a).clarifai.api.PostWorkflowResultsResponse\"\x99\x02\x82\xd3\xe4\x93\x02\xfe\x01\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\x01*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\x01*Z(\"#/v2/workflows/{workflow_id}/results:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\xc5\x03\n\x1dPostWorkflowResultsSimilarity\x12\x32.clarifai.api.PostWorkflowResultsSimilarityRequest\x1a\x33.clarifai.api.PostWorkflowResultsSimilarityResponse\"\xba\x02\x82\xd3\xe4\x93\x02\x9f\x02\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\x01*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\x01*Z3\"./v2/workflows/{workflow_id}/results/similarity:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\x87\x02\n\x14ListWorkflowVersions\x12).clarifai.api.ListWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\x12$/v2/workflows/{workflow_id}/versions\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb0\x02\n\x12GetWorkflowVersion\x12\'.clarifai.api.GetWorkflowVersionRequest\x1a+.clarifai.api.SingleWorkflowVersionResponse\"\xc3\x01\x82\xd3\xe4\x93\x02\xb0\x01\x12p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\x12:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x8c\x02\n\x16\x44\x65leteWorkflowVersions\x12+.clarifai.api.DeleteWorkflowVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x8a\x01*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)*$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x12\x90\x9c\'\x15\x12\x93\x02\n\x15PatchWorkflowVersions\x12*.clarifai.api.PatchWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)2$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x85\x01\n\x06GetKey\x12\x1b.clarifai.api.GetKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"=\x82\xd3\xe4\x93\x02/\x12-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'0\x12\x7f\n\x08ListKeys\x12\x1d.clarifai.api.ListKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"4\x82\xd3\xe4\x93\x02&\x12$/v2/users/{user_app_id.user_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\x9f\x01\n\x0bListAppKeys\x12 .clarifai.api.ListAppKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"N\x82\xd3\xe4\x93\x02@\x12>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\x95\x01\n\tDeleteKey\x12\x1e.clarifai.api.DeleteKeyRequest\x1a!.clarifai.api.status.BaseResponse\"E\x82\xd3\xe4\x93\x02/*-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'1\x90\x9c\'0\x12\x8a\x01\n\x08PostKeys\x12\x1d.clarifai.api.PostKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"?\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\x88\x01\n\tPatchKeys\x12\x1e.clarifai.api.PatchKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'0\x12\xbc\x01\n\x08MyScopes\x12\x1d.clarifai.api.MyScopesRequest\x1a .clarifai.api.MultiScopeResponse\"o\x82\xd3\xe4\x93\x02\x65\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/myscopesZ\x0e\x12\x0c/v2/myscopesZ\x0f\x12\r/v2/my_scopes\x98\x9c\'\x02\x12\x8d\x01\n\x0cMyScopesUser\x12!.clarifai.api.MyScopesUserRequest\x1a$.clarifai.api.MultiScopeUserResponse\"4\x82\xd3\xe4\x93\x02*\x12(/v2/users/{user_app_id.user_id}/myscopes\x98\x9c\'\x05\x12u\n\x0cMyScopesRoot\x12!.clarifai.api.MyScopesRootRequest\x1a$.clarifai.api.MultiScopeRootResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/myscopesroot\x98\x9c\'\x05\x12\x87\x01\n\nListScopes\x12\x1f.clarifai.api.ListScopesRequest\x1a$.clarifai.api.MultiScopeDepsResponse\"2\x82\xd3\xe4\x93\x02(\x12&/v2/users/{user_app_id.user_id}/scopes\x98\x9c\'\x03\x12\x95\x01\n\x06GetApp\x12\x1b.clarifai.api.GetAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"M\x82\xd3\xe4\x93\x02;\x12\x39/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\x8f\x01\n\x08ListApps\x12\x1d.clarifai.api.ListAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\x12$/v2/users/{user_app_id.user_id}/appsZ\n\x12\x08/v2/apps\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\xa5\x01\n\tDeleteApp\x12\x1e.clarifai.api.DeleteAppRequest\x1a!.clarifai.api.status.BaseResponse\"U\x82\xd3\xe4\x93\x02;*9/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'.\x90\x9c\'-\x90\x9c\'\x13\x12\x92\x01\n\x08PostApps\x12\x1d.clarifai.api.PostAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"G\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x88\x01\n\tPatchApps\x12\x1e.clarifai.api.PatchAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x92\x01\n\x0cPatchAppsIds\x12!.clarifai.api.PatchAppsIdsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"?\x82\xd3\xe4\x93\x02-2(/v2/users/{user_app_id.user_id}/apps/ids:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9c\x01\n\x08PatchApp\x12\x1d.clarifai.api.PatchAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"P\x82\xd3\xe4\x93\x02>29/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9f\x01\n\x10PostAppsSearches\x12%.clarifai.api.PostAppsSearchesRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\"-/v2/users/{user_app_id.user_id}/apps/searches:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12v\n\x07GetUser\x12\x1c.clarifai.api.GetUserRequest\x1a .clarifai.api.SingleUserResponse\"+\x82\xd3\xe4\x93\x02!\x12\x1f/v2/users/{user_app_id.user_id}\x98\x9c\'\x05\x12\xcf\x01\n\x14PostValidatePassword\x12).clarifai.api.PostValidatePasswordRequest\x1a..clarifai.api.SinglePasswordValidationResponse\"\\\x82\xd3\xe4\x93\x02R\"1/v2/users/{user_app_id.user_id}/validate_password:\x01*Z\x1a\"\x15/v2/validate_password:\x01*\x98\x9c\'\x03\x12\xbd\x01\n\tGetSearch\x12\x1e.clarifai.api.GetSearchRequest\x1a\".clarifai.api.SingleSearchResponse\"l\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13\x12\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'r\x12\xb8\x01\n\x0cListSearches\x12!.clarifai.api.ListSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"b\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\x0e\x12\x0c/v2/searches\x98\x9c\'\x02\x90\x9c\'r\x12\xc4\x01\n\rPatchSearches\x12\".clarifai.api.PatchSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"l\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\x32\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'s\x90\x9c\'r\x12\xd5\x01\n\x0cPostSearches\x12!.clarifai.api.PostSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x7f\x88\x02\x01\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\"\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd4\x01\n\x10PostSearchesByID\x12%.clarifai.api.PostSearchesByIDRequest\x1a!.clarifai.api.MultiSearchResponse\"v\x82\xd3\xe4\x93\x02\x64\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\x01*Z\x16\"\x11/v2/searches/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'\x03\x12\xaf\x02\n\x1bPostAnnotationSearchMetrics\x12\x30.clarifai.api.PostAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\x01*Z%\" /v2/annotations/searches/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x90\x9c\'6\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xa5\x02\n\x1aGetAnnotationSearchMetrics\x12/.clarifai.api.GetAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\x12%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x9c\x02\n\x1bListAnnotationSearchMetrics\x12\x30.clarifai.api.ListAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\x96\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\x12 /v2/annotations/searches/metrics\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x96\x02\n\x1d\x44\x65leteAnnotationSearchMetrics\x12\x32.clarifai.api.DeleteAnnotationSearchMetricsRequest\x1a!.clarifai.api.status.BaseResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'5\x90\x9c\'6\x90\x9c\'?\x12\xca\x01\n\x0c\x44\x65leteSearch\x12!.clarifai.api.DeleteSearchRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13*\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x90\x9c\'t\x12\xe8\x01\n\x15ListAnnotationFilters\x12*.clarifai.api.ListAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"v\x82\xd3\xe4\x93\x02h\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\x18\x12\x16/v2/annotation_filters\x98\x9c\'\x02\x90\x9c\'r\x12\x95\x02\n\x13GetAnnotationFilter\x12(.clarifai.api.GetAnnotationFilterRequest\x1a,.clarifai.api.SingleAnnotationFilterResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x96\x01\x12\x63/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\x12-/v2/annotation_filters/{annotation_filter_id}\x98\x9c\'\x02\x90\x9c\'r\x12\xf3\x01\n\x15PostAnnotationFilters\x12*.clarifai.api.PostAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\"\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12\xf5\x01\n\x16PatchAnnotationFilters\x12+.clarifai.api.PatchAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x80\x01\x82\xd3\xe4\x93\x02n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\x32\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12\xed\x01\n\x17\x44\x65leteAnnotationFilters\x12,.clarifai.api.DeleteAnnotationFiltersRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b*\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'r\x90\x9c\'s\x12|\n\x0fListStatusCodes\x12$.clarifai.api.ListStatusCodesRequest\x1a%.clarifai.api.MultiStatusCodeResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/status_codes\x98\x9c\'\x01\x12\x8a\x01\n\rGetStatusCode\x12\".clarifai.api.GetStatusCodeRequest\x1a&.clarifai.api.SingleStatusCodeResponse\"-\x82\xd3\xe4\x93\x02#\x12!/v2/status_codes/{status_code_id}\x98\x9c\'\x01\x12\xbe\x01\n\x11ListCollaborators\x12&.clarifai.api.ListCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"W\x82\xd3\xe4\x93\x02I\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\x98\x9c\'\x02\x90\x9c\'2\x12\xc5\x01\n\x11PostCollaborators\x12&.clarifai.api.PostCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"^\x82\xd3\xe4\x93\x02L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x12\xcb\x01\n\x12PatchCollaborators\x12\'.clarifai.api.PatchCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"b\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x12\xce\x01\n\x13\x44\x65leteCollaborators\x12(.clarifai.api.DeleteCollaboratorsRequest\x1a!.clarifai.api.status.BaseResponse\"j\x82\xd3\xe4\x93\x02L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x90\x9c\'7\x90\x9c\'8\x12\xa4\x01\n\x12ListCollaborations\x12\'.clarifai.api.ListCollaborationsRequest\x1a).clarifai.api.MultiCollaborationsResponse\":\x82\xd3\xe4\x93\x02\x30\x12./v2/users/{user_app_id.user_id}/collaborations\x98\x9c\'\x03\x12\xef\x01\n\x13PostAppDuplications\x12(.clarifai.api.PostAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"\x81\x01\x82\xd3\xe4\x93\x02K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\x01*\x98\x9c\'\x02\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\n\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x12\x90\x9c\'\x13\x12\xa5\x01\n\x13ListAppDuplications\x12(.clarifai.api.ListAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"8\x82\xd3\xe4\x93\x02.\x12,/v2/users/{user_app_id.user_id}/duplications\x98\x9c\'\x05\x12\xb6\x01\n\x11GetAppDuplication\x12&.clarifai.api.GetAppDuplicationRequest\x1a*.clarifai.api.SingleAppDuplicationResponse\"M\x82\xd3\xe4\x93\x02\x43\x12\x41/v2/users/{user_app_id.user_id}/duplications/{app_duplication_id}\x98\x9c\'\x05\x12\xd5\x01\n\tPostTasks\x12\x1e.clarifai.api.PostTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x86\x01\x82\xd3\xe4\x93\x02T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\"\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'\x03\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xfa\x01\n\x16GetTaskAnnotationCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\x12%/v2/tasks/{task_id}/annotations/count\x98\x9c\'\x02\x90\x9c\'8\x12\xea\x01\n\x11GetTaskInputCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x8a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\x12 /v2/tasks/{task_id}/inputs/count\x98\x9c\'\x02\x90\x9c\'8\x12\xcc\x01\n\x07GetTask\x12\x1c.clarifai.api.GetTaskRequest\x1a .clarifai.api.SingleTaskResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\x15\x12\x13/v2/tasks/{task_id}\x98\x9c\'\x02\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xba\x01\n\tListTasks\x12\x1e.clarifai.api.ListTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"l\x82\xd3\xe4\x93\x02N\x12?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\x0b\x12\t/v2/tasks\x98\x9c\'\x02\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd3\x01\n\nPatchTasks\x12\x1f.clarifai.api.PatchTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x82\x01\x82\xd3\xe4\x93\x02T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\x32\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xbe\x01\n\x0b\x44\x65leteTasks\x12 .clarifai.api.DeleteTasksRequest\x1a!.clarifai.api.status.BaseResponse\"j\x82\xd3\xe4\x93\x02T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e*\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xf1\x01\n\x0fPostLabelOrders\x12$.clarifai.api.PostLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x90\x01\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\"\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf2\x01\n\rGetLabelOrder\x12\".clarifai.api.GetLabelOrderRequest\x1a&.clarifai.api.SingleLabelOrderResponse\"\x94\x01\x82\xd3\xe4\x93\x02~\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\x12!/v2/label_orders/{label_order_id}\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xd2\x01\n\x0fListLabelOrders\x12$.clarifai.api.ListLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"r\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\x12\x12\x10/v2/label_orders\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xe7\x01\n\x10PatchLabelOrders\x12%.clarifai.api.PatchLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62\x32\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\x32\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'C\x90\x9c\'D\x90\x9c\'\x0b\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xe1\x01\n\x11\x44\x65leteLabelOrders\x12&.clarifai.api.DeleteLabelOrdersRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15*\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'E\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x12\xee\x01\n\x0ePostCollectors\x12#.clarifai.api.PostCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"\x90\x01\x82\xd3\xe4\x93\x02^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\"\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'\x04\x90\x9c\'%\x90\x9c\'&\x90\x9c\')\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xdf\x01\n\x0cGetCollector\x12!.clarifai.api.GetCollectorRequest\x1a%.clarifai.api.SingleCollectorResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\x1f\x12\x1d/v2/collectors/{collector_id}\x98\x9c\'\x02\x90\x9c\'*\x12\xc3\x01\n\x0eListCollectors\x12#.clarifai.api.ListCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"f\x82\xd3\xe4\x93\x02X\x12\x44/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\x10\x12\x0e/v2/collectors\x98\x9c\'\x02\x90\x9c\'*\x12\xcf\x01\n\x0fPatchCollectors\x12$.clarifai.api.PatchCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"p\x82\xd3\xe4\x93\x02^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\x32\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\')\x90\x9c\'*\x12\xd2\x01\n\x10\x44\x65leteCollectors\x12%.clarifai.api.DeleteCollectorsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13*\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\')\x90\x9c\'+\x90\x9c\'*\x12\xc9\x01\n\x0ePostStatValues\x12#.clarifai.api.PostStatValuesRequest\x1a$.clarifai.api.MultiStatValueResponse\"l\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values:\x01*Z\x15\"\x10/v2/stats/values:\x01*\x98\x9c\'\x02\x12\xf9\x01\n\x17PostStatValuesAggregate\x12,.clarifai.api.PostStatValuesAggregateRequest\x1a-.clarifai.api.MultiStatValueAggregateResponse\"\x80\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\x01*Z\x1f\"\x1a/v2/stats/values/aggregate:\x01*\x98\x9c\'\x02\x12\xe3\x01\n\x17PostTrendingMetricsView\x12,.clarifai.api.PostTrendingMetricsViewRequest\x1a!.clarifai.api.status.BaseResponse\"w\x82\xd3\xe4\x93\x02m\"h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}/{object_id}:\x01*\x98\x9c\'\x02\x12\x8f\x02\n\x18ListTrendingMetricsViews\x12-.clarifai.api.ListTrendingMetricsViewsRequest\x1a..clarifai.api.MultiTrendingMetricsViewResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x88\x01\x12\\/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}Z(\x12&/v2/trending_metrics/views/{view_type}\x98\x9c\'\x02\x12\xae\x01\n\tGetModule\x12\x1e.clarifai.api.GetModuleRequest\x1a\".clarifai.api.SingleModuleResponse\"]\x82\xd3\xe4\x93\x02O\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\x98\x9c\'\x02\x90\x9c\'m\x12\xe0\x01\n\x0bListModules\x12 .clarifai.api.ListModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\x8b\x01\x82\xd3\xe4\x93\x02}\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\x12\'/v2/users/{user_app_id.user_id}/modulesZ\r\x12\x0b/v2/modules\x98\x9c\'\x02\x90\x9c\'m\x12\xac\x01\n\x0bPostModules\x12 .clarifai.api.PostModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"X\x82\xd3\xe4\x93\x02\x46\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xae\x01\n\x0cPatchModules\x12!.clarifai.api.PatchModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"X\x82\xd3\xe4\x93\x02\x46\x32\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xb4\x01\n\rDeleteModules\x12\".clarifai.api.DeleteModulesRequest\x1a!.clarifai.api.status.BaseResponse\"\\\x82\xd3\xe4\x93\x02\x46*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x12\xe8\x01\n\x10GetModuleVersion\x12%.clarifai.api.GetModuleVersionRequest\x1a).clarifai.api.SingleModuleVersionResponse\"\x81\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions/{module_version_id}\x98\x9c\'\x02\x90\x9c\'m\x12\xd6\x01\n\x12ListModuleVersions\x12\'.clarifai.api.ListModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"m\x82\xd3\xe4\x93\x02_\x12]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions\x98\x9c\'\x02\x90\x9c\'m\x12\xdd\x01\n\x12PostModuleVersions\x12\'.clarifai.api.PostModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"t\x82\xd3\xe4\x93\x02\x62\"]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'m\x12\xde\x01\n\x14\x44\x65leteModuleVersions\x12).clarifai.api.DeleteModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02\x62*]/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/module_versions:\x01*\x98\x9c\'\x02\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x12\x8b\x02\n\x19GetInstalledModuleVersion\x12..clarifai.api.GetInstalledModuleVersionRequest\x1a\x32.clarifai.api.SingleInstalledModuleVersionResponse\"\x89\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\x98\x9c\'\x05\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xef\x01\n\x1bListInstalledModuleVersions\x12\x30.clarifai.api.ListInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"k\x82\xd3\xe4\x93\x02U\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\x98\x9c\'\x05\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf6\x01\n\x1bPostInstalledModuleVersions\x12\x30.clarifai.api.PostInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"r\x82\xd3\xe4\x93\x02X\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x12\xf6\x01\n\x1d\x44\x65leteInstalledModuleVersions\x12\x32.clarifai.api.DeleteInstalledModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"~\x82\xd3\xe4\x93\x02X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'q\x90\x9c\'m\x90\x9c\'1\x90\x9c\'/\x90\x9c\'0\x12\x95\x02\n\x1ePostInstalledModuleVersionsKey\x12\x33.clarifai.api.PostInstalledModuleVersionsKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\"u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}/key:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\xf1\x01\n\x12PostBulkOperations\x12\'.clarifai.api.PostBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"\x86\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\"\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'z\x90\x9c\'y\x90\x9c\'%\x90\x9c\'&\x90\x9c\'(\x12\xda\x01\n\x12ListBulkOperations\x12\'.clarifai.api.ListBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"p\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\x15\x12\x13/v2/bulk_operations\x98\x9c\'\x02\x90\x9c\'z\x12\xe1\x01\n\x10GetBulkOperation\x12%.clarifai.api.GetBulkOperationRequest\x1a*.clarifai.api.SingleBulkOperationsResponse\"z\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\x1a\x12\x18/v2/bulk_operations/{id}\x98\x9c\'\x02\x90\x9c\'z\x12\xe7\x01\n\x14\x43\x61ncelBulkOperations\x12(.clarifai.api.CancelBulkOperationRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"z\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\x32\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'y\x90\x9c\'z\x12\xf0\x01\n\x14\x44\x65leteBulkOperations\x12(.clarifai.api.DeleteBulkOperationRequest\x1a!.clarifai.api.status.BaseResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18*\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'%\x90\x9c\'(\x90\x9c\'y\x90\x9c\'z\x90\x9c\'{\x12\xae\x02\n\x1cGetDatasetInputsSearchAddJob\x12\x31.clarifai.api.GetDatasetInputsSearchAddJobRequest\x1a\x35.clarifai.api.SingleDatasetInputsSearchAddJobResponse\"\xa3\x01\x82\xd3\xe4\x93\x02\x94\x01\x12\x62/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\x12,/v2/datasets/inputs/search_add/jobs/{job_id}\x98\x9c\'\x02\x90\x9c\'i\x12\x84\x02\n\x17ListNextTaskAssignments\x12,.clarifai.api.ListNextTaskAssignmentsRequest\x1a .clarifai.api.MultiInputResponse\"\x98\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\x12\x1f/v2/tasks/{task_id}/assignments\x98\x9c\'\x02\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xde\x01\n\x12PutTaskAssignments\x12\'.clarifai.api.PutTaskAssignmentsRequest\x1a!.clarifai.api.status.BaseResponse\"|\x82\xd3\xe4\x93\x02Z\x1aU/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xd6\x01\n\x11ListInputsAddJobs\x12&.clarifai.api.ListInputsAddJobsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"p\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\x15\x12\x13/v2/inputs/jobs/add\x98\x9c\'\x02\x90\x9c\'\x05\x12\xdd\x01\n\x0fGetInputsAddJob\x12$.clarifai.api.GetInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"z\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\x1a\x12\x18/v2/inputs/jobs/add/{id}\x98\x9c\'\x02\x90\x9c\'\x05\x12\xc0\x01\n\x0bPostUploads\x12 .clarifai.api.PostUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"l\x82\xd3\xe4\x93\x02X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10\"\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\x88\x02\n\x15PutUploadContentParts\x12*.clarifai.api.PutUploadContentPartsRequest\x1a\".clarifai.api.SingleUploadResponse\"\x9e\x01\x82\xd3\xe4\x93\x02\x89\x01\x1a[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\x01*Z\'\x1a%/v2/uploads/{upload_id}/content_parts\x98\x9c\'\x02\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\xca\x01\n\tGetUpload\x12\x1e.clarifai.api.GetUploadRequest\x1a\".clarifai.api.SingleUploadResponse\"y\x82\xd3\xe4\x93\x02j\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\x19\x12\x17/v2/uploads/{upload_id}\x98\x9c\'\x02\x90\x9c\'\x80\x01\x12\xb5\x01\n\x0bListUploads\x12 .clarifai.api.ListUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"a\x82\xd3\xe4\x93\x02R\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\x12\x0b/v2/uploads\x98\x9c\'\x02\x90\x9c\'\x80\x01\x12\xc9\x01\n\rDeleteUploads\x12\".clarifai.api.DeleteUploadsRequest\x1a!.clarifai.api.status.BaseResponse\"q\x82\xd3\xe4\x93\x02X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10*\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'\x80\x01\x90\x9c\'\x81\x01\x90\x9c\'\x82\x01\x12\x89\x02\n\x15PostInputsDataSources\x12*.clarifai.api.PostInputsDataSourcesRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9a\x01\x82\xd3\xe4\x93\x02p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\x01*Z\x1c\"\x17/v2/inputs/data_sources:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xae\x02\n\x16GetInputsExtractionJob\x12+.clarifai.api.GetInputsExtractionJobRequest\x1a/.clarifai.api.SingleInputsExtractionJobResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\xa6\x01\x12k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\x12\x35/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\x98\x9c\'\x02\x90\x9c\'\x05\x12\xf9\x01\n\x18ListInputsExtractionJobs\x12-.clarifai.api.ListInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"~\x82\xd3\xe4\x93\x02p\x12P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\x1c\x12\x1a/v2/inputs/jobs/extraction\x98\x9c\'\x02\x90\x9c\'\x05\x12\x88\x02\n\x1a\x43\x61ncelInputsExtractionJobs\x12/.clarifai.api.CancelInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\x01*Z\x1f\x32\x1a/v2/inputs/jobs/extraction:\x01*\x98\x9c\'\x02\x90\x9c\'\x04\x90\x9c\'\x05\x12\x81\x02\n\x11PostInputsUploads\x12&.clarifai.api.PostInputsUploadsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9a\x01\x82\xd3\xe4\x93\x02\x66\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\x01*Z\x17\"\x12/v2/inputs/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025com.clarifai.grpc.apiP\001Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\242\002\004CAIP'
@@ -341,14 +341,16 @@
   _V2.methods_by_name['PatchApps']._serialized_options = b'\202\323\344\223\002)2$/v2/users/{user_app_id.user_id}/apps:\001*\230\234\'\005\220\234\',\220\234\'-'
   _V2.methods_by_name['PatchAppsIds']._options = None
   _V2.methods_by_name['PatchAppsIds']._serialized_options = b'\202\323\344\223\002-2(/v2/users/{user_app_id.user_id}/apps/ids:\001*\230\234\'\005\220\234\',\220\234\'-'
   _V2.methods_by_name['PatchApp']._options = None
   _V2.methods_by_name['PatchApp']._serialized_options = b'\202\323\344\223\002>29/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}:\001*\230\234\'\005\220\234\',\220\234\'-'
   _V2.methods_by_name['PostAppsSearches']._options = None
   _V2.methods_by_name['PostAppsSearches']._serialized_options = b'\202\323\344\223\0022\"-/v2/users/{user_app_id.user_id}/apps/searches:\001*\230\234\'\005\220\234\'-\220\234\'\023'
+  _V2.methods_by_name['GetUser']._options = None
+  _V2.methods_by_name['GetUser']._serialized_options = b'\202\323\344\223\002!\022\037/v2/users/{user_app_id.user_id}\230\234\'\005'
   _V2.methods_by_name['PostValidatePassword']._options = None
   _V2.methods_by_name['PostValidatePassword']._serialized_options = b'\202\323\344\223\002R\"1/v2/users/{user_app_id.user_id}/validate_password:\001*Z\032\"\025/v2/validate_password:\001*\230\234\'\003'
   _V2.methods_by_name['GetSearch']._options = None
   _V2.methods_by_name['GetSearch']._serialized_options = b'\202\323\344\223\002^\022G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\023\022\021/v2/searches/{id}\230\234\'\002\220\234\'r'
   _V2.methods_by_name['ListSearches']._options = None
   _V2.methods_by_name['ListSearches']._serialized_options = b'\202\323\344\223\002T\022B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\016\022\014/v2/searches\230\234\'\002\220\234\'r'
   _V2.methods_by_name['PatchSearches']._options = None
@@ -475,14 +477,18 @@
   _V2.methods_by_name['GetBulkOperation']._serialized_options = b'\202\323\344\223\002l\022N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\032\022\030/v2/bulk_operations/{id}\230\234\'\002\220\234\'z'
   _V2.methods_by_name['CancelBulkOperations']._options = None
   _V2.methods_by_name['CancelBulkOperations']._serialized_options = b'\202\323\344\223\002h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\0302\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'y\220\234\'z'
   _V2.methods_by_name['DeleteBulkOperations']._options = None
   _V2.methods_by_name['DeleteBulkOperations']._serialized_options = b'\202\323\344\223\002h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\001*Z\030*\023/v2/bulk_operations:\001*\230\234\'\002\220\234\'&\220\234\'%\220\234\'(\220\234\'y\220\234\'z\220\234\'{'
   _V2.methods_by_name['GetDatasetInputsSearchAddJob']._options = None
   _V2.methods_by_name['GetDatasetInputsSearchAddJob']._serialized_options = b'\202\323\344\223\002\224\001\022b/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\022,/v2/datasets/inputs/search_add/jobs/{job_id}\230\234\'\002\220\234\'i'
+  _V2.methods_by_name['ListNextTaskAssignments']._options = None
+  _V2.methods_by_name['ListNextTaskAssignments']._serialized_options = b'\202\323\344\223\002z\022U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\022\037/v2/tasks/{task_id}/assignments\230\234\'\002\220\234\'&\220\234\'\013\220\234\'\005\220\234\'8\220\234\'i'
+  _V2.methods_by_name['PutTaskAssignments']._options = None
+  _V2.methods_by_name['PutTaskAssignments']._serialized_options = b'\202\323\344\223\002Z\032U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\005\220\234\'8\220\234\'i'
   _V2.methods_by_name['ListInputsAddJobs']._options = None
   _V2.methods_by_name['ListInputsAddJobs']._serialized_options = b'\202\323\344\223\002b\022I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\025\022\023/v2/inputs/jobs/add\230\234\'\002\220\234\'\005'
   _V2.methods_by_name['GetInputsAddJob']._options = None
   _V2.methods_by_name['GetInputsAddJob']._serialized_options = b'\202\323\344\223\002l\022N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\032\022\030/v2/inputs/jobs/add/{id}\230\234\'\002\220\234\'\005'
   _V2.methods_by_name['PostUploads']._options = None
   _V2.methods_by_name['PostUploads']._serialized_options = b'\202\323\344\223\002X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\001*Z\020\"\013/v2/uploads:\001*\230\234\'\002\220\234\'\201\001\220\234\'\200\001'
   _V2.methods_by_name['PutUploadContentParts']._options = None
@@ -499,16 +505,16 @@
   _V2.methods_by_name['GetInputsExtractionJob']._serialized_options = b'\202\323\344\223\002\246\001\022k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\0225/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\230\234\'\002\220\234\'\005'
   _V2.methods_by_name['ListInputsExtractionJobs']._options = None
   _V2.methods_by_name['ListInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002p\022P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\034\022\032/v2/inputs/jobs/extraction\230\234\'\002\220\234\'\005'
   _V2.methods_by_name['CancelInputsExtractionJobs']._options = None
   _V2.methods_by_name['CancelInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\001*Z\0372\032/v2/inputs/jobs/extraction:\001*\230\234\'\002\220\234\'\004\220\234\'\005'
   _V2.methods_by_name['PostInputsUploads']._options = None
   _V2.methods_by_name['PostInputsUploads']._serialized_options = b'\202\323\344\223\002f\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\001*Z\027\"\022/v2/inputs/uploads:\001*\230\234\'\002\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023\220\234\'\201\001\220\234\'\200\001'
-  _ORGANIZATIONINVITATIONSTATUS._serialized_start=39082
-  _ORGANIZATIONINVITATIONSTATUS._serialized_end=39194
+  _ORGANIZATIONINVITATIONSTATUS._serialized_start=39733
+  _ORGANIZATIONINVITATIONSTATUS._serialized_end=39845
   _PAGINATION._serialized_start=420
   _PAGINATION._serialized_end=464
   _GETANNOTATIONREQUEST._serialized_start=466
   _GETANNOTATIONREQUEST._serialized_end=578
   _LISTANNOTATIONSREQUEST._serialized_start=581
   _LISTANNOTATIONSREQUEST._serialized_end=892
   _POSTANNOTATIONSREQUEST._serialized_start=894
@@ -758,341 +764,349 @@
   _MULTIMODELRESPONSE._serialized_start=16915
   _MULTIMODELRESPONSE._serialized_end=17023
   _PATCHMODELVERSIONSREQUEST._serialized_start=17026
   _PATCHMODELVERSIONSREQUEST._serialized_end=17188
   _GETMODELVERSIONREQUEST._serialized_start=17190
   _GETMODELVERSIONREQUEST._serialized_end=17301
   _LISTMODELVERSIONSREQUEST._serialized_start=17304
-  _LISTMODELVERSIONSREQUEST._serialized_end=17450
-  _DELETEMODELVERSIONREQUEST._serialized_start=17452
-  _DELETEMODELVERSIONREQUEST._serialized_end=17566
-  _SINGLEMODELVERSIONRESPONSE._serialized_start=17568
-  _SINGLEMODELVERSIONRESPONSE._serialized_end=17692
-  _MULTIMODELVERSIONRESPONSE._serialized_start=17695
-  _MULTIMODELVERSIONRESPONSE._serialized_end=17825
-  _POSTMODELVERSIONSREQUEST._serialized_start=17828
-  _POSTMODELVERSIONSREQUEST._serialized_end=18067
-  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_start=18070
-  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_end=18247
-  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_start=18250
-  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_end=18423
-  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_start=18425
-  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_end=18476
-  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_start=18478
-  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_end=18531
-  _MODELVERSIONPUBLISHREQUEST._serialized_start=18533
-  _MODELVERSIONPUBLISHREQUEST._serialized_end=18581
-  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_start=18584
-  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_end=18748
-  _MODELVERSIONUNPUBLISHREQUEST._serialized_start=18750
-  _MODELVERSIONUNPUBLISHREQUEST._serialized_end=18800
-  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_start=18803
-  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_end=18971
-  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_start=18974
-  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_end=19152
-  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_start=19155
-  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_end=19316
-  _GETMODELVERSIONEVALUATIONREQUEST._serialized_start=19319
-  _GETMODELVERSIONEVALUATIONREQUEST._serialized_end=19512
-  _SINGLEEVALMETRICSRESPONSE._serialized_start=19514
-  _SINGLEEVALMETRICSRESPONSE._serialized_end=19635
-  _MULTIEVALMETRICSRESPONSE._serialized_start=19637
-  _MULTIEVALMETRICSRESPONSE._serialized_end=19757
-  _POSTMODELVERSIONMETRICSREQUEST._serialized_start=19760
-  _POSTMODELVERSIONMETRICSREQUEST._serialized_end=19971
-  _GETMODELVERSIONMETRICSREQUEST._serialized_start=19974
-  _GETMODELVERSIONMETRICSREQUEST._serialized_end=20135
-  _GETMODELTYPEREQUEST._serialized_start=20137
-  _GETMODELTYPEREQUEST._serialized_end=20230
-  _LISTMODELTYPESREQUEST._serialized_start=20232
-  _LISTMODELTYPESREQUEST._serialized_end=20336
-  _LISTOPENSOURCELICENSESREQUEST._serialized_start=20338
-  _LISTOPENSOURCELICENSESREQUEST._serialized_end=20369
-  _LISTOPENSOURCELICENSESRESPONSE._serialized_start=20371
-  _LISTOPENSOURCELICENSESRESPONSE._serialized_end=20466
-  _SINGLEMODELTYPERESPONSE._serialized_start=20468
-  _SINGLEMODELTYPERESPONSE._serialized_end=20589
-  _MULTIMODELTYPERESPONSE._serialized_start=20592
-  _MULTIMODELTYPERESPONSE._serialized_end=20834
-  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_start=20837
-  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_end=20986
-  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_start=20989
-  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_end=21152
-  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=21155
-  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=21317
-  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=21320
-  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=21482
-  _LISTMODELREFERENCESREQUEST._serialized_start=21484
-  _LISTMODELREFERENCESREQUEST._serialized_end=21611
-  _MULTIMODELREFERENCERESPONSE._serialized_start=21614
-  _MULTIMODELREFERENCERESPONSE._serialized_end=21744
-  _MULTIOUTPUTRESPONSE._serialized_start=21746
-  _MULTIOUTPUTRESPONSE._serialized_end=21857
-  _LISTSCOPESREQUEST._serialized_start=21859
-  _LISTSCOPESREQUEST._serialized_end=21945
-  _MYSCOPESREQUEST._serialized_start=21947
-  _MYSCOPESREQUEST._serialized_end=22013
-  _MYSCOPESUSERREQUEST._serialized_start=22015
-  _MYSCOPESUSERREQUEST._serialized_end=22085
-  _MYSCOPESROOTREQUEST._serialized_start=22087
-  _MYSCOPESROOTREQUEST._serialized_end=22108
-  _MULTISCOPEDEPSRESPONSE._serialized_start=22111
-  _MULTISCOPEDEPSRESPONSE._serialized_end=22276
-  _MULTISCOPERESPONSE._serialized_start=22279
-  _MULTISCOPERESPONSE._serialized_end=22439
-  _MULTISCOPEUSERRESPONSE._serialized_start=22442
-  _MULTISCOPEUSERRESPONSE._serialized_end=22574
-  _MULTISCOPEROOTRESPONSE._serialized_start=22577
-  _MULTISCOPEROOTRESPONSE._serialized_end=22709
-  _GETSEARCHREQUEST._serialized_start=22711
-  _GETSEARCHREQUEST._serialized_end=22790
-  _LISTSEARCHESREQUEST._serialized_start=22792
-  _LISTSEARCHESREQUEST._serialized_end=22894
-  _POSTSEARCHESREQUEST._serialized_start=22897
-  _POSTSEARCHESREQUEST._serialized_end=23093
-  _PATCHINPUTSSEARCHESREQUEST._serialized_start=23096
-  _PATCHINPUTSSEARCHESREQUEST._serialized_end=23229
-  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_start=23232
-  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_end=23370
-  _PATCHSEARCHESREQUEST._serialized_start=23372
-  _PATCHSEARCHESREQUEST._serialized_end=23499
-  _POSTSEARCHESBYIDREQUEST._serialized_start=23502
-  _POSTSEARCHESBYIDREQUEST._serialized_end=23634
-  _DELETESEARCHREQUEST._serialized_start=23636
-  _DELETESEARCHREQUEST._serialized_end=23718
-  _POSTANNOTATIONSSEARCHESREQUEST._serialized_start=23721
-  _POSTANNOTATIONSSEARCHESREQUEST._serialized_end=23888
-  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_start=23890
-  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_end=23989
-  _POSTINPUTSSEARCHESREQUEST._serialized_start=23992
-  _POSTINPUTSSEARCHESREQUEST._serialized_end=24154
-  _SINGLESEARCHRESPONSE._serialized_start=24156
-  _SINGLESEARCHRESPONSE._serialized_end=24261
-  _MULTISEARCHRESPONSE._serialized_start=24264
-  _MULTISEARCHRESPONSE._serialized_end=24457
-  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24460
-  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=24736
-  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24738
-  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_end=24834
-  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24836
-  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=24921
-  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_start=24924
-  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_end=25081
-  _LISTANNOTATIONFILTERSREQUEST._serialized_start=25083
-  _LISTANNOTATIONFILTERSREQUEST._serialized_end=25194
-  _GETANNOTATIONFILTERREQUEST._serialized_start=25196
-  _GETANNOTATIONFILTERREQUEST._serialized_end=25303
-  _POSTANNOTATIONFILTERSREQUEST._serialized_start=25306
-  _POSTANNOTATIONFILTERSREQUEST._serialized_end=25445
-  _PATCHANNOTATIONFILTERSREQUEST._serialized_start=25448
-  _PATCHANNOTATIONFILTERSREQUEST._serialized_end=25604
-  _DELETEANNOTATIONFILTERSREQUEST._serialized_start=25606
-  _DELETEANNOTATIONFILTERSREQUEST._serialized_end=25718
-  _MULTIANNOTATIONFILTERRESPONSE._serialized_start=25721
-  _MULTIANNOTATIONFILTERRESPONSE._serialized_end=25863
-  _SINGLEANNOTATIONFILTERRESPONSE._serialized_start=25866
-  _SINGLEANNOTATIONFILTERRESPONSE._serialized_end=26002
-  _POSTVALIDATEPASSWORDREQUEST._serialized_start=26004
-  _POSTVALIDATEPASSWORDREQUEST._serialized_end=26124
-  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_start=26127
-  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_end=26269
-  _GETWORKFLOWREQUEST._serialized_start=26272
-  _GETWORKFLOWREQUEST._serialized_end=26459
-  _LISTWORKFLOWSREQUEST._serialized_start=26462
-  _LISTWORKFLOWSREQUEST._serialized_end=26777
-  _POSTWORKFLOWSREQUEST._serialized_start=26779
-  _POSTWORKFLOWSREQUEST._serialized_end=26893
-  _PATCHWORKFLOWSREQUEST._serialized_start=26896
-  _PATCHWORKFLOWSREQUEST._serialized_end=27027
-  _PATCHWORKFLOWIDSREQUEST._serialized_start=27030
-  _PATCHWORKFLOWIDSREQUEST._serialized_end=27163
-  _DELETEWORKFLOWREQUEST._serialized_start=27165
-  _DELETEWORKFLOWREQUEST._serialized_end=27258
-  _DELETEWORKFLOWSREQUEST._serialized_start=27260
-  _DELETEWORKFLOWSREQUEST._serialized_end=27366
-  _SINGLEWORKFLOWRESPONSE._serialized_start=27368
-  _SINGLEWORKFLOWRESPONSE._serialized_end=27479
-  _MULTIWORKFLOWRESPONSE._serialized_start=27481
-  _MULTIWORKFLOWRESPONSE._serialized_end=27598
-  _POSTWORKFLOWRESULTSREQUEST._serialized_start=27601
-  _POSTWORKFLOWRESULTSREQUEST._serialized_end=27894
-  _POSTWORKFLOWRESULTSRESPONSE._serialized_start=27897
-  _POSTWORKFLOWRESULTSRESPONSE._serialized_end=28113
-  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_start=28116
-  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_end=28389
-  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_start=28392
-  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_end=28534
-  _LISTWORKFLOWVERSIONSREQUEST._serialized_start=28537
-  _LISTWORKFLOWVERSIONSREQUEST._serialized_end=28668
-  _GETWORKFLOWVERSIONREQUEST._serialized_start=28670
-  _GETWORKFLOWVERSIONREQUEST._serialized_end=28796
-  _DELETEWORKFLOWVERSIONSREQUEST._serialized_start=28799
-  _DELETEWORKFLOWVERSIONSREQUEST._serialized_end=28930
-  _PATCHWORKFLOWVERSIONSREQUEST._serialized_start=28933
-  _PATCHWORKFLOWVERSIONSREQUEST._serialized_end=29107
-  _MULTIWORKFLOWVERSIONRESPONSE._serialized_start=29110
-  _MULTIWORKFLOWVERSIONRESPONSE._serialized_end=29249
-  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_start=29252
-  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_end=29385
-  _POSTAPPDUPLICATIONSREQUEST._serialized_start=29388
-  _POSTAPPDUPLICATIONSREQUEST._serialized_end=29521
-  _GETAPPDUPLICATIONREQUEST._serialized_start=29523
-  _GETAPPDUPLICATIONREQUEST._serialized_end=29626
-  _LISTAPPDUPLICATIONSREQUEST._serialized_start=29628
-  _LISTAPPDUPLICATIONSREQUEST._serialized_end=29737
-  _MULTIAPPDUPLICATIONSRESPONSE._serialized_start=29740
-  _MULTIAPPDUPLICATIONSRESPONSE._serialized_end=29871
-  _SINGLEAPPDUPLICATIONRESPONSE._serialized_start=29874
-  _SINGLEAPPDUPLICATIONRESPONSE._serialized_end=30004
-  _POSTTASKSREQUEST._serialized_start=30006
-  _POSTTASKSREQUEST._serialized_end=30108
-  _GETTASKREQUEST._serialized_start=30110
-  _GETTASKREQUEST._serialized_end=30219
-  _LISTTASKSREQUEST._serialized_start=30222
-  _LISTTASKSREQUEST._serialized_end=30460
-  _PATCHTASKSREQUEST._serialized_start=30462
-  _PATCHTASKSREQUEST._serialized_end=30581
-  _DELETETASKSREQUEST._serialized_start=30583
-  _DELETETASKSREQUEST._serialized_end=30665
-  _MULTITASKRESPONSE._serialized_start=30667
-  _MULTITASKRESPONSE._serialized_end=30772
-  _SINGLETASKRESPONSE._serialized_start=30774
-  _SINGLETASKRESPONSE._serialized_end=30873
-  _GETTASKCOUNTREQUEST._serialized_start=30875
-  _GETTASKCOUNTREQUEST._serialized_end=30980
-  _SINGLETASKCOUNTRESPONSE._serialized_start=30983
-  _SINGLETASKCOUNTRESPONSE._serialized_end=31140
-  _POSTLABELORDERSREQUEST._serialized_start=31142
-  _POSTLABELORDERSREQUEST._serialized_end=31263
-  _GETLABELORDERREQUEST._serialized_start=31265
-  _GETLABELORDERREQUEST._serialized_end=31360
-  _LISTLABELORDERSREQUEST._serialized_start=31362
-  _LISTLABELORDERSREQUEST._serialized_end=31467
-  _PATCHLABELORDERSREQUEST._serialized_start=31470
-  _PATCHLABELORDERSREQUEST._serialized_end=31608
-  _DELETELABELORDERSREQUEST._serialized_start=31610
-  _DELETELABELORDERSREQUEST._serialized_end=31698
-  _MULTILABELORDERRESPONSE._serialized_start=31700
-  _MULTILABELORDERRESPONSE._serialized_end=31824
-  _SINGLELABELORDERRESPONSE._serialized_start=31826
-  _SINGLELABELORDERRESPONSE._serialized_end=31944
-  _POSTCOLLECTORSREQUEST._serialized_start=31946
-  _POSTCOLLECTORSREQUEST._serialized_end=32063
-  _PATCHCOLLECTORSREQUEST._serialized_start=32066
-  _PATCHCOLLECTORSREQUEST._serialized_end=32200
-  _DELETECOLLECTORSREQUEST._serialized_start=32202
-  _DELETECOLLECTORSREQUEST._serialized_end=32309
-  _GETCOLLECTORREQUEST._serialized_start=32311
-  _GETCOLLECTORREQUEST._serialized_end=32403
-  _LISTCOLLECTORSREQUEST._serialized_start=32405
-  _LISTCOLLECTORSREQUEST._serialized_end=32509
-  _MULTICOLLECTORRESPONSE._serialized_start=32511
-  _MULTICOLLECTORRESPONSE._serialized_end=32625
-  _SINGLECOLLECTORRESPONSE._serialized_start=32627
-  _SINGLECOLLECTORRESPONSE._serialized_end=32741
-  _POSTSTATVALUESREQUEST._serialized_start=32743
-  _POSTSTATVALUESREQUEST._serialized_end=32861
-  _MULTISTATVALUERESPONSE._serialized_start=32863
-  _MULTISTATVALUERESPONSE._serialized_end=32984
-  _POSTSTATVALUESAGGREGATEREQUEST._serialized_start=32987
-  _POSTSTATVALUESAGGREGATEREQUEST._serialized_end=33145
-  _MULTISTATVALUEAGGREGATERESPONSE._serialized_start=33148
-  _MULTISTATVALUEAGGREGATERESPONSE._serialized_end=33304
-  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_start=33306
-  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_end=33425
-  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_start=33428
-  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_end=33561
-  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_start=33563
-  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_end=33689
-  _GETMODULEREQUEST._serialized_start=33691
-  _GETMODULEREQUEST._serialized_end=33777
-  _LISTMODULESREQUEST._serialized_start=33779
-  _LISTMODULESREQUEST._serialized_end=33880
-  _POSTMODULESREQUEST._serialized_start=33882
-  _POSTMODULESREQUEST._serialized_end=33990
-  _PATCHMODULESREQUEST._serialized_start=33992
-  _PATCHMODULESREQUEST._serialized_end=34117
-  _DELETEMODULESREQUEST._serialized_start=34119
-  _DELETEMODULESREQUEST._serialized_end=34203
-  _SINGLEMODULERESPONSE._serialized_start=34205
-  _SINGLEMODULERESPONSE._serialized_end=34310
-  _MULTIMODULERESPONSE._serialized_start=34312
-  _MULTIMODULERESPONSE._serialized_end=34423
-  _GETMODULEVERSIONREQUEST._serialized_start=34425
-  _GETMODULEVERSIONREQUEST._serialized_end=34545
-  _LISTMODULEVERSIONSREQUEST._serialized_start=34547
-  _LISTMODULEVERSIONSREQUEST._serialized_end=34674
-  _POSTMODULEVERSIONSREQUEST._serialized_start=34677
-  _POSTMODULEVERSIONSREQUEST._serialized_end=34826
-  _DELETEMODULEVERSIONSREQUEST._serialized_start=34828
-  _DELETEMODULEVERSIONSREQUEST._serialized_end=34938
-  _SINGLEMODULEVERSIONRESPONSE._serialized_start=34940
-  _SINGLEMODULEVERSIONRESPONSE._serialized_end=35067
-  _MULTIMODULEVERSIONRESPONSE._serialized_start=35070
-  _MULTIMODULEVERSIONRESPONSE._serialized_end=35203
-  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_start=35205
-  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_end=35325
-  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=35327
-  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=35444
-  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=35447
-  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=35605
-  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_start=35607
-  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_end=35732
-  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_start=35734
-  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_end=35834
-  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_start=35837
-  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_end=35992
-  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_start=35995
-  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_end=36156
-  _POSTBULKOPERATIONSREQUEST._serialized_start=36159
-  _POSTBULKOPERATIONSREQUEST._serialized_end=36289
-  _LISTBULKOPERATIONSREQUEST._serialized_start=36291
-  _LISTBULKOPERATIONSREQUEST._serialized_end=36399
-  _GETBULKOPERATIONREQUEST._serialized_start=36401
-  _GETBULKOPERATIONREQUEST._serialized_end=36487
-  _CANCELBULKOPERATIONREQUEST._serialized_start=36489
-  _CANCELBULKOPERATIONREQUEST._serialized_end=36579
-  _DELETEBULKOPERATIONREQUEST._serialized_start=36581
-  _DELETEBULKOPERATIONREQUEST._serialized_end=36671
-  _SINGLEBULKOPERATIONSRESPONSE._serialized_start=36674
-  _SINGLEBULKOPERATIONSRESPONSE._serialized_end=36802
-  _MULTIBULKOPERATIONSRESPONSE._serialized_start=36804
-  _MULTIBULKOPERATIONSRESPONSE._serialized_end=36931
-  _LISTINPUTSADDJOBSREQUEST._serialized_start=36933
-  _LISTINPUTSADDJOBSREQUEST._serialized_end=37040
-  _GETINPUTSADDJOBREQUEST._serialized_start=37042
-  _GETINPUTSADDJOBREQUEST._serialized_end=37127
-  _MULTIINPUTSADDJOBRESPONSE._serialized_start=37130
-  _MULTIINPUTSADDJOBRESPONSE._serialized_end=37261
-  _SINGLEINPUTSADDJOBRESPONSE._serialized_start=37263
-  _SINGLEINPUTSADDJOBRESPONSE._serialized_end=37388
-  _POSTUPLOADSREQUEST._serialized_start=37390
-  _POSTUPLOADSREQUEST._serialized_end=37498
-  _DELETEUPLOADSREQUEST._serialized_start=37500
-  _DELETEUPLOADSREQUEST._serialized_end=37584
-  _LISTUPLOADSREQUEST._serialized_start=37586
-  _LISTUPLOADSREQUEST._serialized_end=37687
-  _GETUPLOADREQUEST._serialized_start=37689
-  _GETUPLOADREQUEST._serialized_end=37775
-  _SINGLEUPLOADRESPONSE._serialized_start=37777
-  _SINGLEUPLOADRESPONSE._serialized_end=37882
-  _MULTIUPLOADRESPONSE._serialized_start=37884
-  _MULTIUPLOADRESPONSE._serialized_end=37989
-  _PUTUPLOADCONTENTPARTSREQUEST._serialized_start=37992
-  _PUTUPLOADCONTENTPARTSREQUEST._serialized_end=38146
-  _POSTINPUTSDATASOURCESREQUEST._serialized_start=38149
-  _POSTINPUTSDATASOURCESREQUEST._serialized_end=38322
-  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_start=38324
-  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_end=38438
-  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_start=38440
-  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_end=38554
-  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_start=38557
-  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_end=38703
-  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_start=38706
-  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_end=38852
-  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_start=38854
-  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_end=38951
-  _POSTINPUTSUPLOADSREQUEST._serialized_start=38953
-  _POSTINPUTSUPLOADSREQUEST._serialized_end=39080
-  _V2._serialized_start=39198
-  _V2._serialized_end=86101
+  _LISTMODELVERSIONSREQUEST._serialized_end=17629
+  _DELETEMODELVERSIONREQUEST._serialized_start=17631
+  _DELETEMODELVERSIONREQUEST._serialized_end=17745
+  _SINGLEMODELVERSIONRESPONSE._serialized_start=17747
+  _SINGLEMODELVERSIONRESPONSE._serialized_end=17871
+  _MULTIMODELVERSIONRESPONSE._serialized_start=17874
+  _MULTIMODELVERSIONRESPONSE._serialized_end=18004
+  _POSTMODELVERSIONSREQUEST._serialized_start=18007
+  _POSTMODELVERSIONSREQUEST._serialized_end=18246
+  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_start=18249
+  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_end=18426
+  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_start=18429
+  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_end=18602
+  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_start=18604
+  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_end=18655
+  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_start=18657
+  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_end=18710
+  _MODELVERSIONPUBLISHREQUEST._serialized_start=18712
+  _MODELVERSIONPUBLISHREQUEST._serialized_end=18760
+  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_start=18763
+  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_end=18927
+  _MODELVERSIONUNPUBLISHREQUEST._serialized_start=18929
+  _MODELVERSIONUNPUBLISHREQUEST._serialized_end=18979
+  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_start=18982
+  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_end=19150
+  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_start=19153
+  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_end=19331
+  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_start=19334
+  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_end=19495
+  _GETMODELVERSIONEVALUATIONREQUEST._serialized_start=19498
+  _GETMODELVERSIONEVALUATIONREQUEST._serialized_end=19691
+  _SINGLEEVALMETRICSRESPONSE._serialized_start=19693
+  _SINGLEEVALMETRICSRESPONSE._serialized_end=19814
+  _MULTIEVALMETRICSRESPONSE._serialized_start=19816
+  _MULTIEVALMETRICSRESPONSE._serialized_end=19936
+  _POSTMODELVERSIONMETRICSREQUEST._serialized_start=19939
+  _POSTMODELVERSIONMETRICSREQUEST._serialized_end=20150
+  _GETMODELVERSIONMETRICSREQUEST._serialized_start=20153
+  _GETMODELVERSIONMETRICSREQUEST._serialized_end=20314
+  _GETMODELTYPEREQUEST._serialized_start=20316
+  _GETMODELTYPEREQUEST._serialized_end=20409
+  _LISTMODELTYPESREQUEST._serialized_start=20411
+  _LISTMODELTYPESREQUEST._serialized_end=20515
+  _LISTOPENSOURCELICENSESREQUEST._serialized_start=20517
+  _LISTOPENSOURCELICENSESREQUEST._serialized_end=20548
+  _LISTOPENSOURCELICENSESRESPONSE._serialized_start=20550
+  _LISTOPENSOURCELICENSESRESPONSE._serialized_end=20645
+  _SINGLEMODELTYPERESPONSE._serialized_start=20647
+  _SINGLEMODELTYPERESPONSE._serialized_end=20768
+  _MULTIMODELTYPERESPONSE._serialized_start=20771
+  _MULTIMODELTYPERESPONSE._serialized_end=21013
+  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_start=21016
+  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_end=21165
+  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_start=21168
+  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_end=21331
+  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=21334
+  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=21496
+  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=21499
+  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=21661
+  _LISTMODELREFERENCESREQUEST._serialized_start=21663
+  _LISTMODELREFERENCESREQUEST._serialized_end=21790
+  _MULTIMODELREFERENCERESPONSE._serialized_start=21793
+  _MULTIMODELREFERENCERESPONSE._serialized_end=21923
+  _MULTIOUTPUTRESPONSE._serialized_start=21925
+  _MULTIOUTPUTRESPONSE._serialized_end=22036
+  _LISTSCOPESREQUEST._serialized_start=22038
+  _LISTSCOPESREQUEST._serialized_end=22124
+  _MYSCOPESREQUEST._serialized_start=22126
+  _MYSCOPESREQUEST._serialized_end=22192
+  _MYSCOPESUSERREQUEST._serialized_start=22194
+  _MYSCOPESUSERREQUEST._serialized_end=22264
+  _MYSCOPESROOTREQUEST._serialized_start=22266
+  _MYSCOPESROOTREQUEST._serialized_end=22287
+  _MULTISCOPEDEPSRESPONSE._serialized_start=22290
+  _MULTISCOPEDEPSRESPONSE._serialized_end=22455
+  _MULTISCOPERESPONSE._serialized_start=22458
+  _MULTISCOPERESPONSE._serialized_end=22618
+  _MULTISCOPEUSERRESPONSE._serialized_start=22621
+  _MULTISCOPEUSERRESPONSE._serialized_end=22753
+  _MULTISCOPEROOTRESPONSE._serialized_start=22756
+  _MULTISCOPEROOTRESPONSE._serialized_end=22888
+  _GETSEARCHREQUEST._serialized_start=22890
+  _GETSEARCHREQUEST._serialized_end=22969
+  _LISTSEARCHESREQUEST._serialized_start=22971
+  _LISTSEARCHESREQUEST._serialized_end=23073
+  _POSTSEARCHESREQUEST._serialized_start=23076
+  _POSTSEARCHESREQUEST._serialized_end=23272
+  _PATCHINPUTSSEARCHESREQUEST._serialized_start=23275
+  _PATCHINPUTSSEARCHESREQUEST._serialized_end=23408
+  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_start=23411
+  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_end=23549
+  _PATCHSEARCHESREQUEST._serialized_start=23551
+  _PATCHSEARCHESREQUEST._serialized_end=23678
+  _POSTSEARCHESBYIDREQUEST._serialized_start=23681
+  _POSTSEARCHESBYIDREQUEST._serialized_end=23813
+  _DELETESEARCHREQUEST._serialized_start=23815
+  _DELETESEARCHREQUEST._serialized_end=23897
+  _POSTANNOTATIONSSEARCHESREQUEST._serialized_start=23900
+  _POSTANNOTATIONSSEARCHESREQUEST._serialized_end=24067
+  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24069
+  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_end=24168
+  _POSTINPUTSSEARCHESREQUEST._serialized_start=24171
+  _POSTINPUTSSEARCHESREQUEST._serialized_end=24353
+  _SINGLESEARCHRESPONSE._serialized_start=24355
+  _SINGLESEARCHRESPONSE._serialized_end=24460
+  _MULTISEARCHRESPONSE._serialized_start=24463
+  _MULTISEARCHRESPONSE._serialized_end=24700
+  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24703
+  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=24979
+  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24981
+  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25077
+  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25079
+  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25164
+  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_start=25167
+  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_end=25324
+  _LISTANNOTATIONFILTERSREQUEST._serialized_start=25326
+  _LISTANNOTATIONFILTERSREQUEST._serialized_end=25437
+  _GETANNOTATIONFILTERREQUEST._serialized_start=25439
+  _GETANNOTATIONFILTERREQUEST._serialized_end=25546
+  _POSTANNOTATIONFILTERSREQUEST._serialized_start=25549
+  _POSTANNOTATIONFILTERSREQUEST._serialized_end=25688
+  _PATCHANNOTATIONFILTERSREQUEST._serialized_start=25691
+  _PATCHANNOTATIONFILTERSREQUEST._serialized_end=25847
+  _DELETEANNOTATIONFILTERSREQUEST._serialized_start=25849
+  _DELETEANNOTATIONFILTERSREQUEST._serialized_end=25961
+  _MULTIANNOTATIONFILTERRESPONSE._serialized_start=25964
+  _MULTIANNOTATIONFILTERRESPONSE._serialized_end=26106
+  _SINGLEANNOTATIONFILTERRESPONSE._serialized_start=26109
+  _SINGLEANNOTATIONFILTERRESPONSE._serialized_end=26245
+  _GETUSERREQUEST._serialized_start=26247
+  _GETUSERREQUEST._serialized_end=26339
+  _SINGLEUSERRESPONSE._serialized_start=26341
+  _SINGLEUSERRESPONSE._serialized_end=26440
+  _POSTVALIDATEPASSWORDREQUEST._serialized_start=26442
+  _POSTVALIDATEPASSWORDREQUEST._serialized_end=26562
+  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_start=26565
+  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_end=26707
+  _GETWORKFLOWREQUEST._serialized_start=26710
+  _GETWORKFLOWREQUEST._serialized_end=26897
+  _LISTWORKFLOWSREQUEST._serialized_start=26900
+  _LISTWORKFLOWSREQUEST._serialized_end=27215
+  _POSTWORKFLOWSREQUEST._serialized_start=27217
+  _POSTWORKFLOWSREQUEST._serialized_end=27331
+  _PATCHWORKFLOWSREQUEST._serialized_start=27334
+  _PATCHWORKFLOWSREQUEST._serialized_end=27465
+  _PATCHWORKFLOWIDSREQUEST._serialized_start=27468
+  _PATCHWORKFLOWIDSREQUEST._serialized_end=27601
+  _DELETEWORKFLOWREQUEST._serialized_start=27603
+  _DELETEWORKFLOWREQUEST._serialized_end=27696
+  _DELETEWORKFLOWSREQUEST._serialized_start=27698
+  _DELETEWORKFLOWSREQUEST._serialized_end=27804
+  _SINGLEWORKFLOWRESPONSE._serialized_start=27806
+  _SINGLEWORKFLOWRESPONSE._serialized_end=27917
+  _MULTIWORKFLOWRESPONSE._serialized_start=27919
+  _MULTIWORKFLOWRESPONSE._serialized_end=28036
+  _POSTWORKFLOWRESULTSREQUEST._serialized_start=28039
+  _POSTWORKFLOWRESULTSREQUEST._serialized_end=28332
+  _POSTWORKFLOWRESULTSRESPONSE._serialized_start=28335
+  _POSTWORKFLOWRESULTSRESPONSE._serialized_end=28551
+  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_start=28554
+  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_end=28827
+  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_start=28830
+  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_end=28972
+  _LISTWORKFLOWVERSIONSREQUEST._serialized_start=28975
+  _LISTWORKFLOWVERSIONSREQUEST._serialized_end=29106
+  _GETWORKFLOWVERSIONREQUEST._serialized_start=29108
+  _GETWORKFLOWVERSIONREQUEST._serialized_end=29234
+  _DELETEWORKFLOWVERSIONSREQUEST._serialized_start=29237
+  _DELETEWORKFLOWVERSIONSREQUEST._serialized_end=29368
+  _PATCHWORKFLOWVERSIONSREQUEST._serialized_start=29371
+  _PATCHWORKFLOWVERSIONSREQUEST._serialized_end=29545
+  _MULTIWORKFLOWVERSIONRESPONSE._serialized_start=29548
+  _MULTIWORKFLOWVERSIONRESPONSE._serialized_end=29687
+  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_start=29690
+  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_end=29823
+  _POSTAPPDUPLICATIONSREQUEST._serialized_start=29826
+  _POSTAPPDUPLICATIONSREQUEST._serialized_end=29959
+  _GETAPPDUPLICATIONREQUEST._serialized_start=29961
+  _GETAPPDUPLICATIONREQUEST._serialized_end=30064
+  _LISTAPPDUPLICATIONSREQUEST._serialized_start=30066
+  _LISTAPPDUPLICATIONSREQUEST._serialized_end=30175
+  _MULTIAPPDUPLICATIONSRESPONSE._serialized_start=30178
+  _MULTIAPPDUPLICATIONSRESPONSE._serialized_end=30309
+  _SINGLEAPPDUPLICATIONRESPONSE._serialized_start=30312
+  _SINGLEAPPDUPLICATIONRESPONSE._serialized_end=30442
+  _POSTTASKSREQUEST._serialized_start=30444
+  _POSTTASKSREQUEST._serialized_end=30546
+  _GETTASKREQUEST._serialized_start=30548
+  _GETTASKREQUEST._serialized_end=30657
+  _LISTTASKSREQUEST._serialized_start=30660
+  _LISTTASKSREQUEST._serialized_end=30898
+  _PATCHTASKSREQUEST._serialized_start=30900
+  _PATCHTASKSREQUEST._serialized_end=31019
+  _DELETETASKSREQUEST._serialized_start=31021
+  _DELETETASKSREQUEST._serialized_end=31103
+  _MULTITASKRESPONSE._serialized_start=31105
+  _MULTITASKRESPONSE._serialized_end=31210
+  _SINGLETASKRESPONSE._serialized_start=31212
+  _SINGLETASKRESPONSE._serialized_end=31311
+  _GETTASKCOUNTREQUEST._serialized_start=31313
+  _GETTASKCOUNTREQUEST._serialized_end=31418
+  _SINGLETASKCOUNTRESPONSE._serialized_start=31421
+  _SINGLETASKCOUNTRESPONSE._serialized_end=31578
+  _POSTLABELORDERSREQUEST._serialized_start=31580
+  _POSTLABELORDERSREQUEST._serialized_end=31701
+  _GETLABELORDERREQUEST._serialized_start=31703
+  _GETLABELORDERREQUEST._serialized_end=31798
+  _LISTLABELORDERSREQUEST._serialized_start=31800
+  _LISTLABELORDERSREQUEST._serialized_end=31905
+  _PATCHLABELORDERSREQUEST._serialized_start=31908
+  _PATCHLABELORDERSREQUEST._serialized_end=32046
+  _DELETELABELORDERSREQUEST._serialized_start=32048
+  _DELETELABELORDERSREQUEST._serialized_end=32136
+  _MULTILABELORDERRESPONSE._serialized_start=32138
+  _MULTILABELORDERRESPONSE._serialized_end=32262
+  _SINGLELABELORDERRESPONSE._serialized_start=32264
+  _SINGLELABELORDERRESPONSE._serialized_end=32382
+  _POSTCOLLECTORSREQUEST._serialized_start=32384
+  _POSTCOLLECTORSREQUEST._serialized_end=32501
+  _PATCHCOLLECTORSREQUEST._serialized_start=32504
+  _PATCHCOLLECTORSREQUEST._serialized_end=32638
+  _DELETECOLLECTORSREQUEST._serialized_start=32640
+  _DELETECOLLECTORSREQUEST._serialized_end=32747
+  _GETCOLLECTORREQUEST._serialized_start=32749
+  _GETCOLLECTORREQUEST._serialized_end=32841
+  _LISTCOLLECTORSREQUEST._serialized_start=32843
+  _LISTCOLLECTORSREQUEST._serialized_end=32947
+  _MULTICOLLECTORRESPONSE._serialized_start=32949
+  _MULTICOLLECTORRESPONSE._serialized_end=33063
+  _SINGLECOLLECTORRESPONSE._serialized_start=33065
+  _SINGLECOLLECTORRESPONSE._serialized_end=33179
+  _POSTSTATVALUESREQUEST._serialized_start=33181
+  _POSTSTATVALUESREQUEST._serialized_end=33299
+  _MULTISTATVALUERESPONSE._serialized_start=33301
+  _MULTISTATVALUERESPONSE._serialized_end=33422
+  _POSTSTATVALUESAGGREGATEREQUEST._serialized_start=33425
+  _POSTSTATVALUESAGGREGATEREQUEST._serialized_end=33583
+  _MULTISTATVALUEAGGREGATERESPONSE._serialized_start=33586
+  _MULTISTATVALUEAGGREGATERESPONSE._serialized_end=33742
+  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_start=33744
+  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_end=33863
+  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_start=33866
+  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_end=33999
+  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_start=34001
+  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_end=34127
+  _GETMODULEREQUEST._serialized_start=34129
+  _GETMODULEREQUEST._serialized_end=34215
+  _LISTMODULESREQUEST._serialized_start=34217
+  _LISTMODULESREQUEST._serialized_end=34318
+  _POSTMODULESREQUEST._serialized_start=34320
+  _POSTMODULESREQUEST._serialized_end=34428
+  _PATCHMODULESREQUEST._serialized_start=34430
+  _PATCHMODULESREQUEST._serialized_end=34555
+  _DELETEMODULESREQUEST._serialized_start=34557
+  _DELETEMODULESREQUEST._serialized_end=34641
+  _SINGLEMODULERESPONSE._serialized_start=34643
+  _SINGLEMODULERESPONSE._serialized_end=34748
+  _MULTIMODULERESPONSE._serialized_start=34750
+  _MULTIMODULERESPONSE._serialized_end=34861
+  _GETMODULEVERSIONREQUEST._serialized_start=34863
+  _GETMODULEVERSIONREQUEST._serialized_end=34983
+  _LISTMODULEVERSIONSREQUEST._serialized_start=34985
+  _LISTMODULEVERSIONSREQUEST._serialized_end=35112
+  _POSTMODULEVERSIONSREQUEST._serialized_start=35115
+  _POSTMODULEVERSIONSREQUEST._serialized_end=35264
+  _DELETEMODULEVERSIONSREQUEST._serialized_start=35266
+  _DELETEMODULEVERSIONSREQUEST._serialized_end=35376
+  _SINGLEMODULEVERSIONRESPONSE._serialized_start=35378
+  _SINGLEMODULEVERSIONRESPONSE._serialized_end=35505
+  _MULTIMODULEVERSIONRESPONSE._serialized_start=35508
+  _MULTIMODULEVERSIONRESPONSE._serialized_end=35641
+  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_start=35643
+  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_end=35763
+  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=35765
+  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=35882
+  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=35885
+  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36043
+  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_start=36045
+  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_end=36170
+  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36172
+  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36272
+  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_start=36275
+  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_end=36430
+  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_start=36433
+  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_end=36594
+  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_start=36596
+  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_end=36694
+  _POSTBULKOPERATIONSREQUEST._serialized_start=36697
+  _POSTBULKOPERATIONSREQUEST._serialized_end=36827
+  _LISTBULKOPERATIONSREQUEST._serialized_start=36829
+  _LISTBULKOPERATIONSREQUEST._serialized_end=36937
+  _GETBULKOPERATIONREQUEST._serialized_start=36939
+  _GETBULKOPERATIONREQUEST._serialized_end=37025
+  _CANCELBULKOPERATIONREQUEST._serialized_start=37027
+  _CANCELBULKOPERATIONREQUEST._serialized_end=37117
+  _DELETEBULKOPERATIONREQUEST._serialized_start=37119
+  _DELETEBULKOPERATIONREQUEST._serialized_end=37209
+  _SINGLEBULKOPERATIONSRESPONSE._serialized_start=37212
+  _SINGLEBULKOPERATIONSRESPONSE._serialized_end=37340
+  _MULTIBULKOPERATIONSRESPONSE._serialized_start=37342
+  _MULTIBULKOPERATIONSRESPONSE._serialized_end=37469
+  _PUTTASKASSIGNMENTSREQUEST._serialized_start=37471
+  _PUTTASKASSIGNMENTSREQUEST._serialized_end=37582
+  _LISTINPUTSADDJOBSREQUEST._serialized_start=37584
+  _LISTINPUTSADDJOBSREQUEST._serialized_end=37691
+  _GETINPUTSADDJOBREQUEST._serialized_start=37693
+  _GETINPUTSADDJOBREQUEST._serialized_end=37778
+  _MULTIINPUTSADDJOBRESPONSE._serialized_start=37781
+  _MULTIINPUTSADDJOBRESPONSE._serialized_end=37912
+  _SINGLEINPUTSADDJOBRESPONSE._serialized_start=37914
+  _SINGLEINPUTSADDJOBRESPONSE._serialized_end=38039
+  _POSTUPLOADSREQUEST._serialized_start=38041
+  _POSTUPLOADSREQUEST._serialized_end=38149
+  _DELETEUPLOADSREQUEST._serialized_start=38151
+  _DELETEUPLOADSREQUEST._serialized_end=38235
+  _LISTUPLOADSREQUEST._serialized_start=38237
+  _LISTUPLOADSREQUEST._serialized_end=38338
+  _GETUPLOADREQUEST._serialized_start=38340
+  _GETUPLOADREQUEST._serialized_end=38426
+  _SINGLEUPLOADRESPONSE._serialized_start=38428
+  _SINGLEUPLOADRESPONSE._serialized_end=38533
+  _MULTIUPLOADRESPONSE._serialized_start=38535
+  _MULTIUPLOADRESPONSE._serialized_end=38640
+  _PUTUPLOADCONTENTPARTSREQUEST._serialized_start=38643
+  _PUTUPLOADCONTENTPARTSREQUEST._serialized_end=38797
+  _POSTINPUTSDATASOURCESREQUEST._serialized_start=38800
+  _POSTINPUTSDATASOURCESREQUEST._serialized_end=38973
+  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_start=38975
+  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_end=39089
+  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_start=39091
+  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_end=39205
+  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_start=39208
+  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_end=39354
+  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_start=39357
+  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_end=39503
+  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_start=39505
+  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_end=39602
+  _POSTINPUTSUPLOADSREQUEST._serialized_start=39604
+  _POSTINPUTSUPLOADSREQUEST._serialized_end=39731
+  _V2._serialized_start=39849
+  _V2._serialized_end=87360
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/service_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3775,39 +3775,70 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     MODEL_ID_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PER_PAGE_FIELD_NUMBER: builtins.int
     CONCEPT_IDS_FIELD_NUMBER: builtins.int
+    TRAINED_ONLY_FIELD_NUMBER: builtins.int
+    SORT_ASCENDING_FIELD_NUMBER: builtins.int
+    SORT_BY_STATUS_CODE_FIELD_NUMBER: builtins.int
+    SORT_BY_NUM_INPUTS_FIELD_NUMBER: builtins.int
+    SORT_BY_DESCRIPTION_FIELD_NUMBER: builtins.int
+    SORT_BY_CREATED_AT_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     model_id: builtins.str
     page: builtins.int
     """(optional URL parameter) The page number. Pagination is used to split the results into chunks.
     Defaults to 1.
     """
     per_page: builtins.int
     """(optional URL parameter) The number of results that will be contained in each page. Defaults
     to 128.
     """
     @property
     def concept_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """To list only the model versions that have these concept ids present in them."""
+        """Filtering options:
+        To list only the model versions that have these concept ids present in them.
+        """
+    trained_only: builtins.bool
+    """To list only the model versions that have been trained."""
+    sort_ascending: builtins.bool
+    """Sorting options:
+    Whether to sort in ascending order. If false, will order in descending order.
+    """
+    sort_by_status_code: builtins.bool
+    """Whether to order by the status code"""
+    sort_by_num_inputs: builtins.bool
+    """Whether to order by the number of training inputs"""
+    sort_by_description: builtins.bool
+    """Whether to sort by the description"""
+    sort_by_created_at: builtins.bool
+    """Whether to order by the created_at time
+    If neither sort option is set to true, will sort by created_at.
+    """
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         model_id: builtins.str = ...,
         page: builtins.int = ...,
         per_page: builtins.int = ...,
         concept_ids: collections.abc.Iterable[builtins.str] | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["concept_ids", b"concept_ids", "model_id", b"model_id", "page", b"page", "per_page", b"per_page", "user_app_id", b"user_app_id"]) -> None: ...
+        trained_only: builtins.bool = ...,
+        sort_ascending: builtins.bool = ...,
+        sort_by_status_code: builtins.bool = ...,
+        sort_by_num_inputs: builtins.bool = ...,
+        sort_by_description: builtins.bool = ...,
+        sort_by_created_at: builtins.bool = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_description", b"sort_by_description", "sort_by_num_inputs", b"sort_by_num_inputs", "sort_by_status_code", b"sort_by_status_code", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["concept_ids", b"concept_ids", "model_id", b"model_id", "page", b"page", "per_page", b"per_page", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_description", b"sort_by_description", "sort_by_num_inputs", b"sort_by_num_inputs", "sort_by_status_code", b"sort_by_status_code", "trained_only", b"trained_only", "user_app_id", b"user_app_id"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_status_code", "sort_by_num_inputs", "sort_by_description", "sort_by_created_at"] | None: ...
 
 global___ListModelVersionsRequest = ListModelVersionsRequest
 
 @typing_extensions.final
 class DeleteModelVersionRequest(google.protobuf.message.Message):
     """DeleteModelVersionRequest"""
 
@@ -5144,32 +5175,38 @@
     """Execute a new input search and optionally save it"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     SEARCHES_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
+    ONLY_COUNT_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet:
         """The user_id and app_id to query from."""
     @property
     def searches(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.Search]:
         """The searched to be executed or saved"""
     @property
     def pagination(self) -> global___Pagination:
         """Pagination information to paginate through search result Hits."""
+    only_count: builtins.bool
+    """If only_count is set, then the response will not contain hits,
+    but hit_counts instead.
+    """
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         searches: collections.abc.Iterable[proto.clarifai.api.resources_pb2.Search] | None = ...,
         pagination: global___Pagination | None = ...,
+        only_count: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "searches", b"searches", "user_app_id", b"user_app_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["only_count", b"only_count", "pagination", b"pagination", "searches", b"searches", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___PostInputsSearchesRequest = PostInputsSearchesRequest
 
 @typing_extensions.final
 class SingleSearchResponse(google.protobuf.message.Message):
     """SingleSearchResponse returns saved search in response to GetSearchRequest"""
 
@@ -5200,39 +5237,46 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     HITS_FIELD_NUMBER: builtins.int
     QUERY_FIELD_NUMBER: builtins.int
     SEARCHES_FIELD_NUMBER: builtins.int
+    HIT_COUNTS_FIELD_NUMBER: builtins.int
     @property
     def status(self) -> proto.clarifai.api.status.status_pb2.Status:
         """Status of whether the search was successful."""
     id: builtins.str
     """A unique id which uniquely identifies a search"""
     @property
     def hits(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.Hit]:
         """The list of search result Hits."""
     @property
     def query(self) -> proto.clarifai.api.resources_pb2.Query:
         """The original query provided in the request."""
     @property
     def searches(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.Search]:
         """The original Searches provided in the request."""
+    @property
+    def hit_counts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.HitCount]:
+        """The counts of hits for each search, in the same order as searches.
+        Only returned if the request set only_count.
+        """
     def __init__(
         self,
         *,
         status: proto.clarifai.api.status.status_pb2.Status | None = ...,
         id: builtins.str = ...,
         hits: collections.abc.Iterable[proto.clarifai.api.resources_pb2.Hit] | None = ...,
         query: proto.clarifai.api.resources_pb2.Query | None = ...,
         searches: collections.abc.Iterable[proto.clarifai.api.resources_pb2.Search] | None = ...,
+        hit_counts: collections.abc.Iterable[proto.clarifai.api.resources_pb2.HitCount] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["query", b"query", "status", b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["hits", b"hits", "id", b"id", "query", b"query", "searches", b"searches", "status", b"status"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["hit_counts", b"hit_counts", "hits", b"hits", "id", b"id", "query", b"query", "searches", b"searches", "status", b"status"]) -> None: ...
 
 global___MultiSearchResponse = MultiSearchResponse
 
 @typing_extensions.final
 class PostAnnotationSearchMetricsRequest(google.protobuf.message.Message):
     """PostAnnotationSearchMetricsRequest"""
 
@@ -5517,14 +5561,64 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["annotation_filter", b"annotation_filter", "status", b"status"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["annotation_filter", b"annotation_filter", "status", b"status"]) -> None: ...
 
 global___SingleAnnotationFilterResponse = SingleAnnotationFilterResponse
 
 @typing_extensions.final
+class GetUserRequest(google.protobuf.message.Message):
+    """GetUserRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    ADDITIONAL_FIELDS_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet:
+        """we used to have user_id but moved to the standard convention. Since this endpoint
+        hasn't been exposed and only used by portal as a url this won't effect anything external.
+        """
+    @property
+    def additional_fields(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """(optional URL parameter) List of additional fields to be included in the response. Currently supported: all, stars"""
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        additional_fields: collections.abc.Iterable[builtins.str] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___GetUserRequest = GetUserRequest
+
+@typing_extensions.final
+class SingleUserResponse(google.protobuf.message.Message):
+    """SingleUserResponse"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STATUS_FIELD_NUMBER: builtins.int
+    USER_FIELD_NUMBER: builtins.int
+    @property
+    def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
+    @property
+    def user(self) -> proto.clarifai.api.resources_pb2.User: ...
+    def __init__(
+        self,
+        *,
+        status: proto.clarifai.api.status.status_pb2.Status | None = ...,
+        user: proto.clarifai.api.resources_pb2.User | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["status", b"status", "user", b"user"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["status", b"status", "user", b"user"]) -> None: ...
+
+global___SingleUserResponse = SingleUserResponse
+
+@typing_extensions.final
 class PostValidatePasswordRequest(google.protobuf.message.Message):
     """PostValidatePasswordRequest"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     PASSWORD_FIELD_NUMBER: builtins.int
@@ -7639,14 +7733,36 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["installed_module_versions", b"installed_module_versions", "status", b"status"]) -> None: ...
 
 global___MultiInstalledModuleVersionResponse = MultiInstalledModuleVersionResponse
 
 @typing_extensions.final
+class ListNextTaskAssignmentsRequest(google.protobuf.message.Message):
+    """ListNextTaskAssignmentsRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    TASK_ID_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    task_id: builtins.str
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        task_id: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["task_id", b"task_id", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___ListNextTaskAssignmentsRequest = ListNextTaskAssignmentsRequest
+
+@typing_extensions.final
 class PostBulkOperationsRequest(google.protobuf.message.Message):
     """Request to perform bulk operations on a list of inputs based on input source."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     BULK_OPERATIONS_FIELD_NUMBER: builtins.int
@@ -7813,14 +7929,39 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["bulk_operation", b"bulk_operation", "status", b"status"]) -> None: ...
 
 global___MultiBulkOperationsResponse = MultiBulkOperationsResponse
 
 @typing_extensions.final
+class PutTaskAssignmentsRequest(google.protobuf.message.Message):
+    """PutTaskAssignmentsRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    TASK_ID_FIELD_NUMBER: builtins.int
+    INPUT_ID_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    task_id: builtins.str
+    input_id: builtins.str
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        task_id: builtins.str = ...,
+        input_id: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["input_id", b"input_id", "task_id", b"task_id", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___PutTaskAssignmentsRequest = PutTaskAssignmentsRequest
+
+@typing_extensions.final
 class ListInputsAddJobsRequest(google.protobuf.message.Message):
     """List all the input ingestion jobs"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
@@ -8050,15 +8191,17 @@
     def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["status", b"status", "uploads", b"uploads"]) -> None: ...
 
 global___MultiUploadResponse = MultiUploadResponse
 
 @typing_extensions.final
 class PutUploadContentPartsRequest(google.protobuf.message.Message):
-    """Upload part of multipart upload"""
+    """Upload a part of a multipart upload.
+    Behaviour on completion depends on the endpoint that was used to initiate the upload.
+    """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     UPLOAD_ID_FIELD_NUMBER: builtins.int
     CONTENT_PARTS_FIELD_NUMBER: builtins.int
     @property
@@ -8076,15 +8219,28 @@
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["content_parts", b"content_parts", "upload_id", b"upload_id", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___PutUploadContentPartsRequest = PutUploadContentPartsRequest
 
 @typing_extensions.final
 class PostInputsDataSourcesRequest(google.protobuf.message.Message):
-    """Request to initiate ingestion of inputs from cloud storage"""
+    """Initiates retrieval of inputs from cloud storage from a user provided data source.
+    Will create and return an inputs-add-job for tracking progress.
+    Archives will be extracted and their contents will be processed as inputs.
+
+    The cloud URL will be treated as a filter prefix. For example s3:/bucket/images_folder/abc will process
+    files in the images_folder beginning with abc or in a subfolder beginning with abc.
+    For example:
+    bucket/images_folder/abcImage.png
+    bucket/images_folder/abc-1/Data.zip
+
+    If given URL is for a private bucket or file, then credentials should be provided to access the bucket.
+    Credentials should include rights to list the objects in the bucket, except when pointed directly at a file archive,
+    in which case it only requires rights to access that particular file.
+    """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     DATA_SOURCES_FIELD_NUMBER: builtins.int
     CALL_BACK_URL_FIELD_NUMBER: builtins.int
     APP_PAT_FIELD_NUMBER: builtins.int
@@ -8222,14 +8378,21 @@
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["ids", b"ids", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___CancelInputsExtractionJobsRequest = CancelInputsExtractionJobsRequest
 
 @typing_extensions.final
 class PostInputsUploadsRequest(google.protobuf.message.Message):
+    """Start uploading a file archive containing inputs.
+    Will create and return an inputs-add-job for tracking progress.
+
+    Associated inputs-add-job contains an upload id which should be completed through `PutUploadContentParts` endpoint.
+    Completing the upload will automatically begin unpacking the archive and uploading the contents as inputs.
+    """
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     INPUTS_UPLOADS_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     @property
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/service_pb2_grpc.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,14 +630,19 @@
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleAppResponse),
                 )
         self.PostAppsSearches = channel.unary_unary(
                 '/clarifai.api.V2/PostAppsSearches',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostAppsSearchesRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiAppResponse),
                 )
+        self.GetUser = channel.unary_unary(
+                '/clarifai.api.V2/GetUser',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetUserRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleUserResponse),
+                )
         self.PostValidatePassword = channel.unary_unary(
                 '/clarifai.api.V2/PostValidatePassword',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostValidatePasswordRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SinglePasswordValidationResponse),
                 )
         self.GetSearch = channel.unary_unary(
                 '/clarifai.api.V2/GetSearch',
@@ -965,14 +970,24 @@
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse),
                 )
         self.GetDatasetInputsSearchAddJob = channel.unary_unary(
                 '/clarifai.api.V2/GetDatasetInputsSearchAddJob',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetDatasetInputsSearchAddJobRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleDatasetInputsSearchAddJobResponse),
                 )
+        self.ListNextTaskAssignments = channel.unary_unary(
+                '/clarifai.api.V2/ListNextTaskAssignments',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListNextTaskAssignmentsRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputResponse),
+                )
+        self.PutTaskAssignments = channel.unary_unary(
+                '/clarifai.api.V2/PutTaskAssignments',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PutTaskAssignmentsRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse),
+                )
         self.ListInputsAddJobs = channel.unary_unary(
                 '/clarifai.api.V2/ListInputsAddJobs',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListInputsAddJobsRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsAddJobResponse),
                 )
         self.GetInputsAddJob = channel.unary_unary(
                 '/clarifai.api.V2/GetInputsAddJob',
@@ -1929,14 +1944,21 @@
     def PostAppsSearches(self, request, context):
         """Search over the applications to find one or more you're looking for.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetUser(self, request, context):
+        """Get user information
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def PostValidatePassword(self, request, context):
         """Validate new password in real-time for a user
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -2417,14 +2439,28 @@
     def GetDatasetInputsSearchAddJob(self, request, context):
         """Get a specific job.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListNextTaskAssignments(self, request, context):
+        """List next non-labeled and unassigned inputs from task's dataset
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def PutTaskAssignments(self, request, context):
+        """PutTaskAssignments evaluates all the annotations by labeler (authenticated user) for given task (task_id) and input (input_id).
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ListInputsAddJobs(self, request, context):
         """List all the inputs add jobs
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -2438,15 +2474,17 @@
     def PostUploads(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PutUploadContentParts(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Upload a part of a multipart upload.
+        Behaviour on completion depends on the endpoint that was used to initiate the upload.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetUpload(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -2462,15 +2500,28 @@
     def DeleteUploads(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PostInputsDataSources(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Initiates retrieval of inputs from cloud storage from a user provided data source.
+        Will create and return an inputs-add-job for tracking progress.
+        Archives will be extracted and their contents will be processed as inputs.
+
+        The cloud URL will be treated as a filter prefix. For example s3:/bucket/images_folder/abc will process
+        files in the images_folder beginning with abc or in a subfolder beginning with abc.
+        For example:
+        bucket/images_folder/abcImage.png
+        bucket/images_folder/abc-1/Data.zip
+
+        If given URL is for a private bucket or file, then credentials should be provided to access the bucket.
+        Credentials should include rights to list the objects in the bucket, except when pointed directly at a file archive,
+        in which case it only requires rights to access that particular file.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetInputsExtractionJob(self, request, context):
         """Get the input extraction job details by ID
         """
@@ -2488,15 +2539,20 @@
     def CancelInputsExtractionJobs(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PostInputsUploads(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Start uploading a file archive containing inputs.
+        Will create and return an inputs-add-job for tracking progress.
+
+        Associated inputs-add-job contains an upload id which should be completed through `PutUploadContentParts` endpoint.
+        Completing the upload will automatically begin unpacking the archive and uploading the contents as inputs.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_V2Servicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -3096,14 +3152,19 @@
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleAppResponse.SerializeToString,
             ),
             'PostAppsSearches': grpc.unary_unary_rpc_method_handler(
                     servicer.PostAppsSearches,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostAppsSearchesRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiAppResponse.SerializeToString,
             ),
+            'GetUser': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetUser,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetUserRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleUserResponse.SerializeToString,
+            ),
             'PostValidatePassword': grpc.unary_unary_rpc_method_handler(
                     servicer.PostValidatePassword,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostValidatePasswordRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SinglePasswordValidationResponse.SerializeToString,
             ),
             'GetSearch': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSearch,
@@ -3431,14 +3492,24 @@
                     response_serializer=proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse.SerializeToString,
             ),
             'GetDatasetInputsSearchAddJob': grpc.unary_unary_rpc_method_handler(
                     servicer.GetDatasetInputsSearchAddJob,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetDatasetInputsSearchAddJobRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleDatasetInputsSearchAddJobResponse.SerializeToString,
             ),
+            'ListNextTaskAssignments': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListNextTaskAssignments,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListNextTaskAssignmentsRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputResponse.SerializeToString,
+            ),
+            'PutTaskAssignments': grpc.unary_unary_rpc_method_handler(
+                    servicer.PutTaskAssignments,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PutTaskAssignmentsRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse.SerializeToString,
+            ),
             'ListInputsAddJobs': grpc.unary_unary_rpc_method_handler(
                     servicer.ListInputsAddJobs,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListInputsAddJobsRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsAddJobResponse.SerializeToString,
             ),
             'GetInputsAddJob': grpc.unary_unary_rpc_method_handler(
                     servicer.GetInputsAddJob,
@@ -5560,14 +5631,31 @@
         return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PostAppsSearches',
             proto_dot_clarifai_dot_api_dot_service__pb2.PostAppsSearchesRequest.SerializeToString,
             proto_dot_clarifai_dot_api_dot_service__pb2.MultiAppResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetUser(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/GetUser',
+            proto_dot_clarifai_dot_api_dot_service__pb2.GetUserRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.SingleUserResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def PostValidatePassword(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -6699,14 +6787,48 @@
         return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/GetDatasetInputsSearchAddJob',
             proto_dot_clarifai_dot_api_dot_service__pb2.GetDatasetInputsSearchAddJobRequest.SerializeToString,
             proto_dot_clarifai_dot_api_dot_service__pb2.SingleDatasetInputsSearchAddJobResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListNextTaskAssignments(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/ListNextTaskAssignments',
+            proto_dot_clarifai_dot_api_dot_service__pb2.ListNextTaskAssignmentsRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def PutTaskAssignments(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PutTaskAssignments',
+            proto_dot_clarifai_dot_api_dot_service__pb2.PutTaskAssignmentsRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ListInputsAddJobs(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_code_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_code_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+proto/clarifai/api/status/status_code.proto\x12\x13\x63larifai.api.status*\xe1P\n\nStatusCode\x12\x08\n\x04ZERO\x10\x00\x12\x0c\n\x07SUCCESS\x10\x90N\x12\x11\n\x0cMIXED_STATUS\x10\x9aN\x12\x0c\n\x07\x46\x41ILURE\x10\xa4N\x12\x0e\n\tTRY_AGAIN\x10\xaeN\x12\x14\n\x0fNOT_IMPLEMENTED\x10\xb8N\x12\n\n\x05MOVED\x10\xc2N\x12\x18\n\x13\x43ONN_ACCOUNT_ISSUES\x10\xf8U\x12\x1b\n\x12\x43ONN_TOKEN_INVALID\x10\xf9U\x1a\x02\x08\x01\x12\x1d\n\x18\x43ONN_CREDENTIALS_INVALID\x10\xfaU\x12\x1d\n\x18\x43ONN_EXCEED_HOURLY_LIMIT\x10\xfbU\x12\x1e\n\x19\x43ONN_EXCEED_MONTHLY_LIMIT\x10\xfcU\x12\x13\n\x0e\x43ONN_THROTTLED\x10\xfdU\x12\x18\n\x13\x43ONN_EXCEEDS_LIMITS\x10\xfeU\x12\x1d\n\x18\x43ONN_INSUFFICIENT_SCOPES\x10\xffU\x12\x15\n\x10\x43ONN_KEY_INVALID\x10\x80V\x12\x17\n\x12\x43ONN_KEY_NOT_FOUND\x10\x81V\x12\x1c\n\x17\x43ONN_BAD_REQUEST_FORMAT\x10\xdcV\x12\x18\n\x13\x43ONN_DOES_NOT_EXIST\x10\xddV\x12\x19\n\x14\x43ONN_INVALID_REQUEST\x10\xdeV\x12\x1c\n\x17\x43ONN_METHOD_NOT_ALLOWED\x10\xdfV\x12\x19\n\x14\x43ONN_NO_GDPR_CONSENT\x10\xe0V\x12\x1e\n\x19\x43ONN_AUTH_METHOD_DISABLED\x10\xc0W\x12\x13\n\rMODEL_TRAINED\x10\xec\xa4\x01\x12\x14\n\x0eMODEL_TRAINING\x10\xed\xa4\x01\x12\x15\n\x0fMODEL_UNTRAINED\x10\xee\xa4\x01\x12\x1f\n\x19MODEL_QUEUED_FOR_TRAINING\x10\xef\xa4\x01\x12\x15\n\x0fMODEL_UPLOADING\x10\xf0\xa4\x01\x12\x1c\n\x16MODEL_UPLOADING_FAILED\x10\xf1\xa4\x01\x12\x1b\n\x15MODEL_TRAINING_FAILED\x10\xf2\xa4\x01\x12\x1c\n\x16MODEL_TRAINING_NO_DATA\x10\xf6\xa4\x01\x12!\n\x1bMODEL_TRAINING_NO_POSITIVES\x10\xf7\xa4\x01\x12*\n$MODEL_TRAINING_ONE_VS_N_SINGLE_CLASS\x10\xf8\xa4\x01\x12\x1e\n\x18MODEL_TRAINING_TIMED_OUT\x10\xf9\xa4\x01\x12\"\n\x1cMODEL_TRAINING_WAITING_ERROR\x10\xfa\xa4\x01\x12\"\n\x1cMODEL_TRAINING_UNKNOWN_ERROR\x10\xfb\xa4\x01\x12&\n\x1cMODEL_TRAINING_MSG_REDELIVER\x10\xfc\xa4\x01\x1a\x02\x08\x01\x12&\n MODEL_TRAINING_INSUFFICIENT_DATA\x10\xfd\xa4\x01\x12#\n\x1dMODEL_TRAINING_INVALID_PARAMS\x10\xfe\xa4\x01\x12\x34\n.MODEL_TRAINING_INVALID_DATA_TOLERANCE_EXCEEDED\x10\xff\xa4\x01\x12\x1a\n\x14MODEL_MODIFY_SUCCESS\x10\x9e\xa5\x01\x12\x1a\n\x14MODEL_MODIFY_PENDING\x10\x9f\xa5\x01\x12\x19\n\x13MODEL_MODIFY_FAILED\x10\xa0\xa5\x01\x12\x1a\n\x14MODEL_DOES_NOT_EXIST\x10\xd0\xa5\x01\x12\x1d\n\x17MODEL_PERMISSION_DENIED\x10\xd1\xa5\x01\x12\x1c\n\x16MODEL_INVALID_ARGUMENT\x10\xd2\xa5\x01\x12\x1b\n\x15MODEL_INVALID_REQUEST\x10\xd3\xa5\x01\x12\x15\n\x0fMODEL_EVALUATED\x10\xb4\xa6\x01\x12\x16\n\x10MODEL_EVALUATING\x10\xb5\xa6\x01\x12\x19\n\x13MODEL_NOT_EVALUATED\x10\xb6\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_EVALUATION\x10\xb7\xa6\x01\x12 \n\x1aMODEL_EVALUATION_TIMED_OUT\x10\xbe\xa6\x01\x12$\n\x1eMODEL_EVALUATION_WAITING_ERROR\x10\xbf\xa6\x01\x12$\n\x1eMODEL_EVALUATION_UNKNOWN_ERROR\x10\xc0\xa6\x01\x12\x1d\n\x17MODEL_PREDICTION_FAILED\x10\xc1\xa6\x01\x12(\n\x1eMODEL_EVALUATION_MSG_REDELIVER\x10\xc2\xa6\x01\x1a\x02\x08\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_LABELS\x10\xc3\xa6\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_INPUTS\x10\xc4\xa6\x01\x12\x1d\n\x17MODEL_EVALUATION_FAILED\x10\xc5\xa6\x01\x12\x1d\n\x17MODEL_DEPLOYMENT_FAILED\x10\xe6\xa6\x01\x12\x15\n\x0fMODEL_DEPLOYING\x10\xe7\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_DEPLOYMENT\x10\xe8\xa6\x01\x12\x18\n\x12MODEL_NOT_DEPLOYED\x10\xe9\xa6\x01\x12&\n MODEL_REFERENCE_INVALID_ARGUMENT\x10\x98\xa7\x01\x12*\n$MODEL_EXAMPLE_INPUT_INVALID_ARGUMENT\x10\xac\xa7\x01\x12 \n\x1aWORKFLOW_NO_MATCHING_INPUT\x10\xf1\xab\x01\x12$\n\x1eWORKFLOW_REQUIRE_TRAINED_MODEL\x10\xf2\xab\x01\x12\x18\n\x12WORKFLOW_DUPLICATE\x10\xd4\xac\x01\x12!\n\x1bWORKFLOW_UNSUPPORTED_FORMAT\x10\xd5\xac\x01\x12\x1d\n\x17WORKFLOW_DOES_NOT_EXIST\x10\xd6\xac\x01\x12 \n\x1aWORKFLOW_PERMISSION_DENIED\x10\xd7\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_ARGUMENT\x10\xd8\xac\x01\x12\x1d\n\x17WORKFLOW_INVALID_RECIPE\x10\xd9\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_TEMPLATE\x10\xda\xac\x01\x12\x1c\n\x16WORKFLOW_INVALID_GRAPH\x10\xdb\xac\x01\x12\x1f\n\x19WORKFLOW_INTERNAL_FAILURE\x10\xdc\xac\x01\x12\x1e\n\x18WORKFLOW_INVALID_REQUEST\x10\xd7\xb3\x01\x12\x1d\n\x17WORKFLOW_MODIFY_SUCCESS\x10\x86\xad\x01\x12\x1d\n\x17WORKFLOW_MODIFY_PENDING\x10\x87\xad\x01\x12\x1c\n\x16WORKFLOW_MODIFY_FAILED\x10\x88\xad\x01\x12\x1d\n\x17WORKFLOW_REINDEX_FAILED\x10\x89\xad\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_SUCCESS\x10\xee\xb4\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_PENDING\x10\xef\xb4\x01\x12\x1b\n\x15\x43ONCEPT_MODIFY_FAILED\x10\xf0\xb4\x01\x12\x18\n\x12\x41NNOTATION_SUCCESS\x10\xd6\xbc\x01\x12\x18\n\x12\x41NNOTATION_PENDING\x10\xd7\xbc\x01\x12\x17\n\x11\x41NNOTATION_FAILED\x10\xd8\xbc\x01\x12\x1f\n\x19\x41NNOTATION_UNKNOWN_STATUS\x10\xda\xbc\x01\x12!\n\x1b\x41NNOTATION_INVALID_ARGUMENT\x10\xdb\xbc\x01\x12\"\n\x1c\x41NNOTATION_PERMISSION_DENIED\x10\xdc\xbc\x01\x12 \n\x1a\x41NNOTATION_AWAITING_REVIEW\x10\xdd\xbc\x01\x12*\n$ANNOTATION_AWAITING_CONSENSUS_REVIEW\x10\xdf\xbc\x01\x12\x1e\n\x18\x41NNOTATION_REVIEW_DENIED\x10\xde\xbc\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_SUCCESS\x10\xba\xbd\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_PENDING\x10\xbb\xbd\x01\x12\x1e\n\x18\x41NNOTATION_MODIFY_FAILED\x10\xbc\xbd\x01\x12&\n METADATA_INVALID_PATCH_ARGUMENTS\x10\xc4\xc2\x01\x12\x1c\n\x16METADATA_PARSING_ISSUE\x10\xc5\xc2\x01\x12!\n\x1bMETADATA_MANIPULATION_ISSUE\x10\xc6\xc2\x01\x12\x1c\n\x16TRAINER_JOB_STATE_NONE\x10\xa8\xc3\x01\x12\x1e\n\x18TRAINER_JOB_STATE_QUEUED\x10\xa9\xc3\x01\x12\x1f\n\x19TRAINER_JOB_STATE_RUNNING\x10\xaa\xc3\x01\x12 \n\x1aTRAINER_JOB_STATE_COMPLETE\x10\xab\xc3\x01\x12\x1d\n\x17TRAINER_JOB_STATE_ERROR\x10\xac\xc3\x01\x12\x17\n\x11\x44\x41TA_DUMP_SUCCESS\x10\xbe\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_PENDING\x10\xbf\xc4\x01\x12\x16\n\x10\x44\x41TA_DUMP_FAILED\x10\xc0\xc4\x01\x12\x1b\n\x15\x44\x41TA_DUMP_IN_PROGRESS\x10\xc1\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_NO_DATA\x10\xc2\xc4\x01\x12 \n\x1a\x44\x41TA_DUMP_UNEXPECTED_ERROR\x10\xc3\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_SUCCESS\x10\xd2\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_PENDING\x10\xd3\xc4\x01\x12\x1d\n\x17\x44\x41TA_DUMP_EXPORT_FAILED\x10\xd4\xc4\x01\x12\"\n\x1c\x44\x41TA_DUMP_EXPORT_IN_PROGRESS\x10\xd5\xc4\x01\x12\'\n!DATA_DUMP_EXPORT_UNEXPECTED_ERROR\x10\xd6\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_SUCCESS\x10\xf0\xc4\x01\x12\x1c\n\x16\x41PP_DUPLICATION_FAILED\x10\xf1\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_PENDING\x10\xf2\xc4\x01\x12!\n\x1b\x41PP_DUPLICATION_IN_PROGRESS\x10\xf3\xc4\x01\x12%\n\x1f\x41PP_DUPLICATION_INVALID_REQUEST\x10\xf4\xc4\x01\x12\x1b\n\x15MODULE_DOES_NOT_EXIST\x10\xd4\xc5\x01\x12\x1e\n\x18MODULE_PERMISSION_DENIED\x10\xd5\xc5\x01\x12\x1d\n\x17MODULE_INVALID_ARGUMENT\x10\xd6\xc5\x01\x12\x1c\n\x16MODULE_INVALID_REQUEST\x10\xd7\xc5\x01\x12\x1c\n\x16\x42ULK_OPERATION_SUCCESS\x10\xb8\xc6\x01\x12\x1b\n\x15\x42ULK_OPERATION_FAILED\x10\xb9\xc6\x01\x12\x1c\n\x16\x42ULK_OPERATION_PENDING\x10\xba\xc6\x01\x12 \n\x1a\x42ULK_OPERATION_IN_PROGRESS\x10\xbb\xc6\x01\x12$\n\x1e\x42ULK_OPERATION_INVALID_REQUEST\x10\xbc\xc6\x01\x12\x1e\n\x18\x42ULK_OPERATION_CANCELLED\x10\xbd\xc6\x01\x12%\n\x1f\x42ULK_OPERATION_UNEXPECTED_ERROR\x10\xbe\xc6\x01\x12\x1c\n\x16INPUT_DOWNLOAD_SUCCESS\x10\xb0\xea\x01\x12\x1c\n\x16INPUT_DOWNLOAD_PENDING\x10\xb1\xea\x01\x12\x1b\n\x15INPUT_DOWNLOAD_FAILED\x10\xb2\xea\x01\x12 \n\x1aINPUT_DOWNLOAD_IN_PROGRESS\x10\xb3\xea\x01\x12 \n\x1aINPUT_STATUS_UPDATE_FAILED\x10\xb4\xea\x01\x12\x19\n\x13INPUT_DELETE_FAILED\x10\xb5\xea\x01\x12\x15\n\x0fINPUT_DUPLICATE\x10\x94\xeb\x01\x12\x1e\n\x18INPUT_UNSUPPORTED_FORMAT\x10\x95\xeb\x01\x12\x1a\n\x14INPUT_DOES_NOT_EXIST\x10\x96\xeb\x01\x12\x1d\n\x17INPUT_PERMISSION_DENIED\x10\x97\xeb\x01\x12\x1c\n\x16INPUT_INVALID_ARGUMENT\x10\x98\xeb\x01\x12\x16\n\x10INPUT_OVER_LIMIT\x10\x99\xeb\x01\x12\x17\n\x11INPUT_INVALID_URL\x10\x9a\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_SUCCESS\x10\xf8\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_PENDING\x10\xf9\xeb\x01\x12\x19\n\x13INPUT_MODIFY_FAILED\x10\xfb\xeb\x01\x12\x1f\n\x19INPUT_STORAGE_HOST_FAILED\x10\x82\xec\x01\x12\x1d\n\x17\x41LL_INPUT_INVALID_BYTES\x10\xdc\xec\x01\x12\x1b\n\x15INPUT_CLUSTER_SUCCESS\x10\xc0\xed\x01\x12\x1b\n\x15INPUT_CLUSTER_PENDING\x10\xc1\xed\x01\x12\x1a\n\x14INPUT_CLUSTER_FAILED\x10\xc2\xed\x01\x12\x1f\n\x19INPUT_CLUSTER_IN_PROGRESS\x10\xc3\xed\x01\x12\x1b\n\x15INPUT_REINDEX_SUCCESS\x10\xa4\xee\x01\x12\x1b\n\x15INPUT_REINDEX_PENDING\x10\xa5\xee\x01\x12\x1a\n\x14INPUT_REINDEX_FAILED\x10\xa6\xee\x01\x12\x1f\n\x19INPUT_REINDEX_IN_PROGRESS\x10\xa7\xee\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_SUCCESS\x10\x98\xf2\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_PENDING\x10\x99\xf2\x01\x12!\n\x1bINPUT_VIDEO_DOWNLOAD_FAILED\x10\x9a\xf2\x01\x12\x1b\n\x15INPUT_VIDEO_DUPLICATE\x10\xfc\xf2\x01\x12$\n\x1eINPUT_VIDEO_UNSUPPORTED_FORMAT\x10\xfd\xf2\x01\x12 \n\x1aINPUT_VIDEO_DOES_NOT_EXIST\x10\xfe\xf2\x01\x12#\n\x1dINPUT_VIDEO_PERMISSION_DENIED\x10\xff\xf2\x01\x12\"\n\x1cINPUT_VIDEO_INVALID_ARGUMENT\x10\x80\xf3\x01\x12\x1c\n\x16INPUT_VIDEO_OVER_LIMIT\x10\x81\xf3\x01\x12\x1d\n\x17INPUT_VIDEO_INVALID_URL\x10\x82\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_SUCCESS\x10\xe0\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_PENDING\x10\xe1\xf3\x01\x12\x1f\n\x19INPUT_VIDEO_MODIFY_FAILED\x10\xe3\xf3\x01\x12%\n\x1fINPUT_VIDEO_STORAGE_HOST_FAILED\x10\xea\xf3\x01\x12$\n\x1e\x41LL_INPUT_VIDEOS_INVALID_BYTES\x10\xc4\xf4\x01\x12\x1d\n\x17INPUT_CONNECTION_FAILED\x10\xbc\xb8\x02\x12&\n REQUEST_DISABLED_FOR_MAINTENANCE\x10\xbd\xb8\x02\x12+\n%INPUT_WRITES_DISABLED_FOR_MAINTENANCE\x10\xbe\xb8\x02\x12\x1b\n\x15INPUT_INVALID_REQUEST\x10\xbf\xb8\x02\x12\x1d\n\x17PREDICT_INVALID_REQUEST\x10\xc1\xb8\x02\x12\x1c\n\x16SEARCH_INVALID_REQUEST\x10\xc2\xb8\x02\x12\x1e\n\x18\x43ONCEPTS_INVALID_REQUEST\x10\xc3\xb8\x02\x12\x1b\n\x15STATS_INVALID_REQUEST\x10\xc4\xb8\x02\x12\x1c\n\x16\x44\x41TABASE_DUPLICATE_KEY\x10\xca\xb8\x02\x12 \n\x1a\x44\x41TABASE_STATEMENT_TIMEOUT\x10\xcb\xb8\x02\x12$\n\x1e\x44\x41TABASE_INVALID_ROWS_AFFECTED\x10\xcc\xb8\x02\x12 \n\x1a\x44\x41TABASE_DEADLOCK_DETECTED\x10\xcd\xb8\x02\x12\x18\n\x12\x44\x41TABASE_FAIL_TASK\x10\xce\xb8\x02\x12&\n DATABASE_FAIL_TO_GET_CONNECTIONS\x10\xcf\xb8\x02\x12\x1f\n\x19\x44\x41TABASE_TOO_MANY_CLIENTS\x10\xd0\xb8\x02\x12\"\n\x1c\x44\x41TABASE_CONSTRAINT_VIOLATED\x10\xd1\xb8\x02\x12\x1f\n\x19\x41SYNC_WORKER_MULTI_ERRORS\x10\xd4\xb8\x02\x12\x1c\n\x16RPC_REQUEST_QUEUE_FULL\x10\xde\xb8\x02\x12\x1c\n\x16RPC_SERVER_UNAVAILABLE\x10\xdf\xb8\x02\x12\x19\n\x13RPC_REQUEST_TIMEOUT\x10\xe0\xb8\x02\x12#\n\x1dRPC_MAX_MESSAGE_SIZE_EXCEEDED\x10\xe1\xb8\x02\x12\x12\n\x0cRPC_CANCELED\x10\xe3\xb8\x02\x12\x18\n\x12RPC_UNKNOWN_METHOD\x10\xe4\xb8\x02\x12\x1e\n\x18REQUEST_CANCELED_BY_USER\x10\xe5\xb8\x02\x12\x1e\n\x18\x43LUSTER_INTERNAL_FAILURE\x10\xa0\xd0\x02\x12\x1f\n\x19\x45XTERNAL_CONNECTION_ERROR\x10\xe2\xb8\x02\x12\x1a\n\x14QUERY_INVALID_SYNTAX\x10\xf2\xb8\x02\x12\x16\n\x10QUEUE_CONN_ERROR\x10\xa8\xc0\x02\x12!\n\x1bQUEUE_CLOSE_REQUEST_TIMEOUT\x10\xaa\xc0\x02\x12\x17\n\x11QUEUE_CONN_CLOSED\x10\xab\xc0\x02\x12\x1f\n\x19QUEUE_PUBLISH_ACK_TIMEOUT\x10\xac\xc0\x02\x12\x19\n\x13QUEUE_PUBLISH_ERROR\x10\xad\xc0\x02\x12 \n\x1aQUEUE_SUBSCRIPTION_TIMEOUT\x10\xae\xc0\x02\x12\x1e\n\x18QUEUE_SUBSCRIPTION_ERROR\x10\xaf\xc0\x02\x12\x1e\n\x18QUEUE_MARSHALLING_FAILED\x10\xb0\xc0\x02\x12 \n\x1aQUEUE_UNMARSHALLING_FAILED\x10\xb1\xc0\x02\x12\'\n!QUEUE_MAX_MSG_REDELIVERY_EXCEEDED\x10\xb2\xc0\x02\x12\x17\n\x11QUEUE_ACK_FAILURE\x10\xb3\xc0\x02\x12\x13\n\rSQS_OVERLIMIT\x10\x8c\xc1\x02\x12 \n\x1aSQS_INVALID_RECEIPT_HANDLE\x10\x8d\xc1\x02\x12\x11\n\x0bSQS_UNKNOWN\x10\x8e\xc1\x02\x12\x1d\n\x17SEARCH_INTERNAL_FAILURE\x10\xf9\xcf\x02\x12\x1f\n\x19SEARCH_PROJECTION_FAILURE\x10\xfa\xcf\x02\x12\x1f\n\x19SEARCH_PREDICTION_FAILURE\x10\xfb\xcf\x02\x12\'\n!SEARCH_BY_NOT_FULLY_INDEXED_INPUT\x10\xfc\xcf\x02\x12 \n\x1aSAVED_SEARCH_MODIFY_FAILED\x10\xfd\xcf\x02\x12\x17\n\x11\x45VALUATION_QUEUED\x10\xdc\xd0\x02\x12\x1c\n\x16\x45VALUATION_IN_PROGRESS\x10\xdd\xd0\x02\x12\x18\n\x12\x45VALUATION_SUCCESS\x10\xde\xd0\x02\x12(\n\"EVALUATION_FAILED_TO_RETRIEVE_DATA\x10\xdf\xd0\x02\x12!\n\x1b\x45VALUATION_INVALID_ARGUMENT\x10\xe0\xd0\x02\x12\x17\n\x11\x45VALUATION_FAILED\x10\xe1\xd0\x02\x12\x18\n\x12\x45VALUATION_PENDING\x10\xe2\xd0\x02\x12\x1a\n\x14\x45VALUATION_TIMED_OUT\x10\xe3\xd0\x02\x12!\n\x1b\x45VALUATION_UNEXPECTED_ERROR\x10\xe4\xd0\x02\x12\x16\n\x10\x45VALUATION_MIXED\x10\xe5\xd0\x02\x12\x18\n\x12STRIPE_EVENT_ERROR\x10\xe1\xd7\x02\x12\x10\n\nCACHE_MISS\x10\xc9\xdf\x02\x12&\n REDIS_SCRIPT_EXITED_WITH_FAILURE\x10\xca\xdf\x02\x12\x16\n\x10REDIS_STREAM_ERR\x10\xcb\xdf\x02\x12\x18\n\x12REDIS_NO_CONSUMERS\x10\xcc\xdf\x02\x12\x1a\n\x14REDIS_STREAM_BACKOFF\x10\xcd\xdf\x02\x12\x18\n\x12SIGNUP_EVENT_ERROR\x10\xb1\xe7\x02\x12\x14\n\x0eSIGNUP_FLAGGED\x10\xb2\xe7\x02\x12\x1a\n\x14\x46ILETYPE_UNSUPPORTED\x10\xb3\xe7\x02\x12\x1f\n\x19\x41PP_COUNT_INVALID_MESSAGE\x10\x99\xef\x02\x12\'\n!APP_COUNT_UPDATE_INCREMENT_FAILED\x10\x9a\xef\x02\x12\x1e\n\x18\x41PP_COUNT_REBUILD_FAILED\x10\x9b\xef\x02\x12 \n\x1a\x41PP_COUNT_INTERNAL_FAILURE\x10\x9c\xef\x02\x12\x17\n\x11MP_DOWNLOAD_ERROR\x10\xfd\xef\x02\x12\x1a\n\x14MP_RESOLVE_DNS_ERROR\x10\xfe\xef\x02\x12)\n#MP_DOWNLOAD_MAX_SIZE_EXCEEDED_ERROR\x10\xff\xef\x02\x12\x1b\n\x15MP_IMAGE_DECODE_ERROR\x10\x80\xf0\x02\x12\x19\n\x13MP_INVALID_ARGUMENT\x10\x81\xf0\x02\x12\x1f\n\x19MP_IMAGE_PROCESSING_ERROR\x10\x82\xf0\x02\x12\x19\n\x13\x44\x41TATIER_CONN_ERROR\x10\xe1\xf0\x02\x12\x17\n\x11USER_CONSENT_FACE\x10\xd1\x86\x03\x12\x14\n\x0eWORKER_MISSING\x10\xb8\x8e\x03\x12\x13\n\rWORKER_ACTIVE\x10\xb9\x8e\x03\x12\x15\n\x0fWORKER_INACTIVE\x10\xba\x8e\x03\x12\x17\n\x11\x43OLLECTOR_MISSING\x10\xa0\x96\x03\x12\x16\n\x10\x43OLLECTOR_ACTIVE\x10\xa1\x96\x03\x12\x18\n\x12\x43OLLECTOR_INACTIVE\x10\xa2\x96\x03\x12!\n\x1b\x43OLLECTOR_POST_INPUT_FAILED\x10\xa3\x96\x03\x12*\n$SSO_IDENTITY_PROVIDER_DOES_NOT_EXIST\x10\x89\x9e\x03\x12\x16\n\x10TASK_IN_PROGRESS\x10\xf1\xa5\x03\x12\x0f\n\tTASK_DONE\x10\xf2\xa5\x03\x12\x12\n\x0cTASK_WONT_DO\x10\xf3\xa5\x03\x12\"\n\x1cTASK_ADD_ANNOTATIONS_FAILURE\x10\xf5\xa5\x03\x12\x13\n\rTASK_CONFLICT\x10\xd4\xa6\x03\x12\x1a\n\x14TASK_NOT_IMPLEMENTED\x10\xd5\xa6\x03\x12\x12\n\x0cTASK_MISSING\x10\xd6\xa6\x03\x12\x19\n\x13LABEL_ORDER_PENDING\x10\xd9\xad\x03\x12\x1d\n\x17LABEL_ORDER_IN_PROGRESS\x10\xda\xad\x03\x12\x19\n\x13LABEL_ORDER_SUCCESS\x10\xdb\xad\x03\x12\x1a\n\x14LABEL_ORDER_CANCELED\x10\xdc\xad\x03\x12\x14\n\x0eLICENSE_ACTIVE\x10\xe0\xd4\x03\x12\x1c\n\x16LICENSE_DOES_NOT_EXIST\x10\xe1\xd4\x03\x12\x19\n\x13LICENSE_NEED_UPDATE\x10\xe2\xd4\x03\x12\x15\n\x0fLICENSE_EXPIRED\x10\xe3\xd4\x03\x12\x15\n\x0fLICENSE_REVOKED\x10\xe4\xd4\x03\x12\x15\n\x0fLICENSE_DELETED\x10\xe5\xd4\x03\x12\x1d\n\x17LICENSE_VOLUME_EXCEEDED\x10\xe6\xd4\x03\x12!\n\x1bPASSWORD_VALIDATION_SUCCESS\x10\xc8\xdc\x03\x12 \n\x1aPASSWORD_VALIDATION_FAILED\x10\xc9\xdc\x03\x12%\n\x1fPASSWORDPOLICY_INVALID_ARGUMENT\x10\xca\xdc\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_CONFIG_NOT_FOUND\x10\xb0\xe4\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_INVALID_ARGUMENT\x10\xb1\xe4\x03\x12\x19\n\x13\x46\x45\x41TUREFLAG_BLOCKED\x10\xb2\xe4\x03\x12\x19\n\x13MAINTENANCE_SUCCESS\x10\x98\xec\x03\x12\x18\n\x12MAINTENANCE_FAILED\x10\x99\xec\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_PENDING\x10\x85\xf4\x03\x12!\n\x1b\x44\x41TASET_VERSION_IN_PROGRESS\x10\x8a\xf4\x03\x12\x1b\n\x15\x44\x41TASET_VERSION_READY\x10\x8f\xf4\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_FAILURE\x10\x94\xf4\x03\x12&\n DATASET_VERSION_UNEXPECTED_ERROR\x10\x99\xf4\x03\x12\x1e\n\x18\x44\x41TASET_VERSION_CONFLICT\x10\x9e\xf4\x03\x12\x1b\n\x15\x44\x41TASET_INPUT_SUCCESS\x10\xe4\xf4\x03\x12\x1d\n\x17\x44\x41TASET_INPUT_DUPLICATE\x10\xe5\xf4\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_SUCCESS\x10\xc8\xf5\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_PENDING\x10\xc9\xf5\x03\x12#\n\x1d\x44\x41TASET_VERSION_EXPORT_FAILED\x10\xca\xf5\x03\x12(\n\"DATASET_VERSION_EXPORT_IN_PROGRESS\x10\xcb\xf5\x03\x12-\n\'DATASET_VERSION_EXPORT_UNEXPECTED_ERROR\x10\xcc\xf5\x03\x12\x10\n\nJOB_QUEUED\x10\x80\xf4\x03\x12\x11\n\x0bJOB_RUNNING\x10\x81\xf4\x03\x12\x13\n\rJOB_COMPLETED\x10\x82\xf4\x03\x12\x10\n\nJOB_FAILED\x10\x83\xf4\x03\x12\x13\n\rJOB_CANCELLED\x10\x84\xf4\x03\x12\x1a\n\x14JOB_UNEXPECTED_ERROR\x10\x86\xf4\x03\x12\x1c\n\x16\x41UTH_MISSING_IDP_ASSOC\x10\xe8\xfb\x03\x12\x19\n\x13LIST_OBJECTS_FAILED\x10\xd0\x83\x04\x12\x1c\n\x16\x41RCHIVE_EXTRACT_FAILED\x10\xb8\x8b\x04\x12\x18\n\x12UPLOAD_IN_PROGRESS\x10\xa0\x93\x04\x12\x11\n\x0bUPLOAD_DONE\x10\xa1\x93\x04\x12\x13\n\rUPLOAD_FAILED\x10\xa2\x93\x04\x12\x1d\n\x17UPLOAD_UNEXPECTED_ERROR\x10\xa3\x93\x04\x12\x14\n\x0eUPLOAD_EXPIRED\x10\xa4\x93\x04\x12\x1a\n\x14\x42ILLING_INVALID_INFO\x10\x88\x9b\x04\x12\x1b\n\x15INTERNAL_SERVER_ISSUE\x10\xd4\xfd\x05\x12\x1d\n\x17INTERNAL_FETCHING_ISSUE\x10\xd5\xfd\x05\x12\x1d\n\x17INTERNAL_DATABASE_ISSUE\x10\xd6\xfd\x05\x12!\n\x1bINTERNAL_UNEXPECTED_TIMEOUT\x10\xd9\xfd\x05\x12\x1c\n\x16INTERNAL_UNEXPECTED_V1\x10\xda\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_PANIC\x10\xdb\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_SPIRE\x10\xdc\xfd\x05\x12 \n\x1aINTERNAL_REDIS_UNAVAILABLE\x10\xdd\xfd\x05\x12!\n\x1bINTERNAL_RESOURCE_EXHAUSTED\x10\xde\xfd\x05\x12\"\n\x1cINTERNAL_REDIS_UNCATEGORIZED\x10\xdf\xfd\x05\x12 \n\x1aINTERNAL_AWS_UNCATEGORIZED\x10\xe0\xfd\x05\x12\"\n\x1cINTERNAL_AZURE_UNCATEGORIZED\x10\xe1\xfd\x05\x12\x18\n\x12\x43ONN_UNCATEGORIZED\x10\xb9\x85\x06\x12\x19\n\x13MODEL_UNCATEGORIZED\x10\xba\x85\x06\x12\x19\n\x13INPUT_UNCATEGORIZED\x10\xbb\x85\x06\x12\x1e\n\x18\x41NNOTATION_UNCATEGORIZED\x10\xbc\x85\x06\x12\x1b\n\x15\x42ILLING_UNCATEGORIZED\x10\xbd\x85\x06\x12\x1c\n\x16INTERNAL_UNCATEGORIZED\x10\xc1\x85\x06\x12\x11\n\x0b\x42\x41\x44_REQUEST\x10\xa0\xc2\x05\x12\x12\n\x0cSERVER_ERROR\x10\x84\xc3\x05\"\x08\x08\xbf\xc6\x01\x10\xbf\xc6\x01\"\x08\x08\xe8\x81\x02\x10\xe8\x81\x02\"\x08\x08\xe9\x81\x02\x10\xe9\x81\x02\"\x08\x08\xea\x81\x02\x10\xea\x81\x02\"\x08\x08\xcc\x82\x02\x10\xcc\x82\x02\"\x08\x08\xcd\x82\x02\x10\xcd\x82\x02\"\x08\x08\xce\x82\x02\x10\xce\x82\x02\"\x08\x08\xcf\x82\x02\x10\xcf\x82\x02\"\x08\x08\xd0\x82\x02\x10\xd0\x82\x02\"\x08\x08\xd1\x82\x02\x10\xd1\x82\x02\"\x08\x08\xd2\x82\x02\x10\xd2\x82\x02\"\x08\x08\xb0\x83\x02\x10\xb0\x83\x02\"\x08\x08\xb1\x83\x02\x10\xb1\x83\x02\"\x08\x08\xb3\x83\x02\x10\xb3\x83\x02\"\x08\x08\xba\x83\x02\x10\xba\x83\x02\"\x08\x08\xbb\xb8\x02\x10\xbb\xb8\x02\"\x08\x08\xd2\xb8\x02\x10\xd2\xb8\x02\"\x08\x08\xd3\xb8\x02\x10\xd3\xb8\x02\"\x08\x08\xf0\xc1\x02\x10\xf0\xc1\x02\"\x08\x08\xf1\xc1\x02\x10\xf1\xc1\x02\"\x08\x08\xf2\xc1\x02\x10\xf2\xc1\x02\"\x08\x08\xf3\xc1\x02\x10\xf3\xc1\x02\"\x08\x08\xf4\xc1\x02\x10\xf4\xc1\x02\"\x08\x08\x9c\xc7\x01\x10\x9c\xc7\x01\"\x08\x08\x9d\xc7\x01\x10\x9d\xc7\x01\"\x08\x08\x9e\xc7\x01\x10\x9e\xc7\x01\"\x08\x08\x9f\xc7\x01\x10\x9f\xc7\x01\"\x08\x08\xa1\xc7\x01\x10\xa1\xc7\x01\"\x08\x08\xa2\xc7\x01\x10\xa2\xc7\x01\x42g\n\x1c\x63om.clarifai.grpc.api.statusP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+proto/clarifai/api/status/status_code.proto\x12\x13\x63larifai.api.status*\x9bQ\n\nStatusCode\x12\x08\n\x04ZERO\x10\x00\x12\x0c\n\x07SUCCESS\x10\x90N\x12\x11\n\x0cMIXED_STATUS\x10\x9aN\x12\x0c\n\x07\x46\x41ILURE\x10\xa4N\x12\x0e\n\tTRY_AGAIN\x10\xaeN\x12\x14\n\x0fNOT_IMPLEMENTED\x10\xb8N\x12\n\n\x05MOVED\x10\xc2N\x12\x18\n\x13\x43ONN_ACCOUNT_ISSUES\x10\xf8U\x12\x1b\n\x12\x43ONN_TOKEN_INVALID\x10\xf9U\x1a\x02\x08\x01\x12\x1d\n\x18\x43ONN_CREDENTIALS_INVALID\x10\xfaU\x12\x1d\n\x18\x43ONN_EXCEED_HOURLY_LIMIT\x10\xfbU\x12\x1e\n\x19\x43ONN_EXCEED_MONTHLY_LIMIT\x10\xfcU\x12\x13\n\x0e\x43ONN_THROTTLED\x10\xfdU\x12\x18\n\x13\x43ONN_EXCEEDS_LIMITS\x10\xfeU\x12\x1d\n\x18\x43ONN_INSUFFICIENT_SCOPES\x10\xffU\x12\x15\n\x10\x43ONN_KEY_INVALID\x10\x80V\x12\x17\n\x12\x43ONN_KEY_NOT_FOUND\x10\x81V\x12\x1c\n\x17\x43ONN_BAD_REQUEST_FORMAT\x10\xdcV\x12\x18\n\x13\x43ONN_DOES_NOT_EXIST\x10\xddV\x12\x19\n\x14\x43ONN_INVALID_REQUEST\x10\xdeV\x12\x1c\n\x17\x43ONN_METHOD_NOT_ALLOWED\x10\xdfV\x12\x19\n\x14\x43ONN_NO_GDPR_CONSENT\x10\xe0V\x12\x1e\n\x19\x43ONN_AUTH_METHOD_DISABLED\x10\xc0W\x12\x13\n\rMODEL_TRAINED\x10\xec\xa4\x01\x12\x14\n\x0eMODEL_TRAINING\x10\xed\xa4\x01\x12\x15\n\x0fMODEL_UNTRAINED\x10\xee\xa4\x01\x12\x1f\n\x19MODEL_QUEUED_FOR_TRAINING\x10\xef\xa4\x01\x12\x15\n\x0fMODEL_UPLOADING\x10\xf0\xa4\x01\x12\x1c\n\x16MODEL_UPLOADING_FAILED\x10\xf1\xa4\x01\x12\x1b\n\x15MODEL_TRAINING_FAILED\x10\xf2\xa4\x01\x12\x1c\n\x16MODEL_TRAINING_NO_DATA\x10\xf6\xa4\x01\x12!\n\x1bMODEL_TRAINING_NO_POSITIVES\x10\xf7\xa4\x01\x12*\n$MODEL_TRAINING_ONE_VS_N_SINGLE_CLASS\x10\xf8\xa4\x01\x12\x1e\n\x18MODEL_TRAINING_TIMED_OUT\x10\xf9\xa4\x01\x12\"\n\x1cMODEL_TRAINING_WAITING_ERROR\x10\xfa\xa4\x01\x12\"\n\x1cMODEL_TRAINING_UNKNOWN_ERROR\x10\xfb\xa4\x01\x12&\n\x1cMODEL_TRAINING_MSG_REDELIVER\x10\xfc\xa4\x01\x1a\x02\x08\x01\x12&\n MODEL_TRAINING_INSUFFICIENT_DATA\x10\xfd\xa4\x01\x12#\n\x1dMODEL_TRAINING_INVALID_PARAMS\x10\xfe\xa4\x01\x12\x34\n.MODEL_TRAINING_INVALID_DATA_TOLERANCE_EXCEEDED\x10\xff\xa4\x01\x12\x1a\n\x14MODEL_MODIFY_SUCCESS\x10\x9e\xa5\x01\x12\x1a\n\x14MODEL_MODIFY_PENDING\x10\x9f\xa5\x01\x12\x19\n\x13MODEL_MODIFY_FAILED\x10\xa0\xa5\x01\x12\x1a\n\x14MODEL_DOES_NOT_EXIST\x10\xd0\xa5\x01\x12\x1d\n\x17MODEL_PERMISSION_DENIED\x10\xd1\xa5\x01\x12\x1c\n\x16MODEL_INVALID_ARGUMENT\x10\xd2\xa5\x01\x12\x1b\n\x15MODEL_INVALID_REQUEST\x10\xd3\xa5\x01\x12\x15\n\x0fMODEL_EVALUATED\x10\xb4\xa6\x01\x12\x16\n\x10MODEL_EVALUATING\x10\xb5\xa6\x01\x12\x19\n\x13MODEL_NOT_EVALUATED\x10\xb6\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_EVALUATION\x10\xb7\xa6\x01\x12 \n\x1aMODEL_EVALUATION_TIMED_OUT\x10\xbe\xa6\x01\x12$\n\x1eMODEL_EVALUATION_WAITING_ERROR\x10\xbf\xa6\x01\x12$\n\x1eMODEL_EVALUATION_UNKNOWN_ERROR\x10\xc0\xa6\x01\x12\x1d\n\x17MODEL_PREDICTION_FAILED\x10\xc1\xa6\x01\x12(\n\x1eMODEL_EVALUATION_MSG_REDELIVER\x10\xc2\xa6\x01\x1a\x02\x08\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_LABELS\x10\xc3\xa6\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_INPUTS\x10\xc4\xa6\x01\x12\x1d\n\x17MODEL_EVALUATION_FAILED\x10\xc5\xa6\x01\x12\x1d\n\x17MODEL_DEPLOYMENT_FAILED\x10\xe6\xa6\x01\x12\x15\n\x0fMODEL_DEPLOYING\x10\xe7\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_DEPLOYMENT\x10\xe8\xa6\x01\x12\x18\n\x12MODEL_NOT_DEPLOYED\x10\xe9\xa6\x01\x12&\n MODEL_REFERENCE_INVALID_ARGUMENT\x10\x98\xa7\x01\x12*\n$MODEL_EXAMPLE_INPUT_INVALID_ARGUMENT\x10\xac\xa7\x01\x12 \n\x1aWORKFLOW_NO_MATCHING_INPUT\x10\xf1\xab\x01\x12$\n\x1eWORKFLOW_REQUIRE_TRAINED_MODEL\x10\xf2\xab\x01\x12\x18\n\x12WORKFLOW_DUPLICATE\x10\xd4\xac\x01\x12!\n\x1bWORKFLOW_UNSUPPORTED_FORMAT\x10\xd5\xac\x01\x12\x1d\n\x17WORKFLOW_DOES_NOT_EXIST\x10\xd6\xac\x01\x12 \n\x1aWORKFLOW_PERMISSION_DENIED\x10\xd7\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_ARGUMENT\x10\xd8\xac\x01\x12\x1d\n\x17WORKFLOW_INVALID_RECIPE\x10\xd9\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_TEMPLATE\x10\xda\xac\x01\x12\x1c\n\x16WORKFLOW_INVALID_GRAPH\x10\xdb\xac\x01\x12\x1f\n\x19WORKFLOW_INTERNAL_FAILURE\x10\xdc\xac\x01\x12\x1e\n\x18WORKFLOW_INVALID_REQUEST\x10\xd7\xb3\x01\x12\x1d\n\x17WORKFLOW_MODIFY_SUCCESS\x10\x86\xad\x01\x12\x1d\n\x17WORKFLOW_MODIFY_PENDING\x10\x87\xad\x01\x12\x1c\n\x16WORKFLOW_MODIFY_FAILED\x10\x88\xad\x01\x12\x1d\n\x17WORKFLOW_REINDEX_FAILED\x10\x89\xad\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_SUCCESS\x10\xee\xb4\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_PENDING\x10\xef\xb4\x01\x12\x1b\n\x15\x43ONCEPT_MODIFY_FAILED\x10\xf0\xb4\x01\x12\x18\n\x12\x41NNOTATION_SUCCESS\x10\xd6\xbc\x01\x12\x18\n\x12\x41NNOTATION_PENDING\x10\xd7\xbc\x01\x12\x17\n\x11\x41NNOTATION_FAILED\x10\xd8\xbc\x01\x12\x1f\n\x19\x41NNOTATION_UNKNOWN_STATUS\x10\xda\xbc\x01\x12!\n\x1b\x41NNOTATION_INVALID_ARGUMENT\x10\xdb\xbc\x01\x12\"\n\x1c\x41NNOTATION_PERMISSION_DENIED\x10\xdc\xbc\x01\x12 \n\x1a\x41NNOTATION_AWAITING_REVIEW\x10\xdd\xbc\x01\x12*\n$ANNOTATION_AWAITING_CONSENSUS_REVIEW\x10\xdf\xbc\x01\x12\x1e\n\x18\x41NNOTATION_REVIEW_DENIED\x10\xde\xbc\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_SUCCESS\x10\xba\xbd\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_PENDING\x10\xbb\xbd\x01\x12\x1e\n\x18\x41NNOTATION_MODIFY_FAILED\x10\xbc\xbd\x01\x12&\n METADATA_INVALID_PATCH_ARGUMENTS\x10\xc4\xc2\x01\x12\x1c\n\x16METADATA_PARSING_ISSUE\x10\xc5\xc2\x01\x12!\n\x1bMETADATA_MANIPULATION_ISSUE\x10\xc6\xc2\x01\x12\x1c\n\x16TRAINER_JOB_STATE_NONE\x10\xa8\xc3\x01\x12\x1e\n\x18TRAINER_JOB_STATE_QUEUED\x10\xa9\xc3\x01\x12\x1f\n\x19TRAINER_JOB_STATE_RUNNING\x10\xaa\xc3\x01\x12 \n\x1aTRAINER_JOB_STATE_COMPLETE\x10\xab\xc3\x01\x12\x1d\n\x17TRAINER_JOB_STATE_ERROR\x10\xac\xc3\x01\x12\x17\n\x11\x44\x41TA_DUMP_SUCCESS\x10\xbe\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_PENDING\x10\xbf\xc4\x01\x12\x16\n\x10\x44\x41TA_DUMP_FAILED\x10\xc0\xc4\x01\x12\x1b\n\x15\x44\x41TA_DUMP_IN_PROGRESS\x10\xc1\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_NO_DATA\x10\xc2\xc4\x01\x12 \n\x1a\x44\x41TA_DUMP_UNEXPECTED_ERROR\x10\xc3\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_SUCCESS\x10\xd2\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_PENDING\x10\xd3\xc4\x01\x12\x1d\n\x17\x44\x41TA_DUMP_EXPORT_FAILED\x10\xd4\xc4\x01\x12\"\n\x1c\x44\x41TA_DUMP_EXPORT_IN_PROGRESS\x10\xd5\xc4\x01\x12\'\n!DATA_DUMP_EXPORT_UNEXPECTED_ERROR\x10\xd6\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_SUCCESS\x10\xf0\xc4\x01\x12\x1c\n\x16\x41PP_DUPLICATION_FAILED\x10\xf1\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_PENDING\x10\xf2\xc4\x01\x12!\n\x1b\x41PP_DUPLICATION_IN_PROGRESS\x10\xf3\xc4\x01\x12%\n\x1f\x41PP_DUPLICATION_INVALID_REQUEST\x10\xf4\xc4\x01\x12\x1b\n\x15MODULE_DOES_NOT_EXIST\x10\xd4\xc5\x01\x12\x1e\n\x18MODULE_PERMISSION_DENIED\x10\xd5\xc5\x01\x12\x1d\n\x17MODULE_INVALID_ARGUMENT\x10\xd6\xc5\x01\x12\x1c\n\x16MODULE_INVALID_REQUEST\x10\xd7\xc5\x01\x12\x1c\n\x16\x42ULK_OPERATION_SUCCESS\x10\xb8\xc6\x01\x12\x1b\n\x15\x42ULK_OPERATION_FAILED\x10\xb9\xc6\x01\x12\x1c\n\x16\x42ULK_OPERATION_PENDING\x10\xba\xc6\x01\x12 \n\x1a\x42ULK_OPERATION_IN_PROGRESS\x10\xbb\xc6\x01\x12$\n\x1e\x42ULK_OPERATION_INVALID_REQUEST\x10\xbc\xc6\x01\x12\x1e\n\x18\x42ULK_OPERATION_CANCELLED\x10\xbd\xc6\x01\x12%\n\x1f\x42ULK_OPERATION_UNEXPECTED_ERROR\x10\xbe\xc6\x01\x12\x1c\n\x16INPUT_DOWNLOAD_SUCCESS\x10\xb0\xea\x01\x12\x1c\n\x16INPUT_DOWNLOAD_PENDING\x10\xb1\xea\x01\x12\x1b\n\x15INPUT_DOWNLOAD_FAILED\x10\xb2\xea\x01\x12 \n\x1aINPUT_DOWNLOAD_IN_PROGRESS\x10\xb3\xea\x01\x12 \n\x1aINPUT_STATUS_UPDATE_FAILED\x10\xb4\xea\x01\x12\x19\n\x13INPUT_DELETE_FAILED\x10\xb5\xea\x01\x12\x15\n\x0fINPUT_DUPLICATE\x10\x94\xeb\x01\x12\x1e\n\x18INPUT_UNSUPPORTED_FORMAT\x10\x95\xeb\x01\x12\x1a\n\x14INPUT_DOES_NOT_EXIST\x10\x96\xeb\x01\x12\x1d\n\x17INPUT_PERMISSION_DENIED\x10\x97\xeb\x01\x12\x1c\n\x16INPUT_INVALID_ARGUMENT\x10\x98\xeb\x01\x12\x16\n\x10INPUT_OVER_LIMIT\x10\x99\xeb\x01\x12\x17\n\x11INPUT_INVALID_URL\x10\x9a\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_SUCCESS\x10\xf8\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_PENDING\x10\xf9\xeb\x01\x12\x19\n\x13INPUT_MODIFY_FAILED\x10\xfb\xeb\x01\x12\x1f\n\x19INPUT_STORAGE_HOST_FAILED\x10\x82\xec\x01\x12\x1d\n\x17\x41LL_INPUT_INVALID_BYTES\x10\xdc\xec\x01\x12\x1b\n\x15INPUT_CLUSTER_SUCCESS\x10\xc0\xed\x01\x12\x1b\n\x15INPUT_CLUSTER_PENDING\x10\xc1\xed\x01\x12\x1a\n\x14INPUT_CLUSTER_FAILED\x10\xc2\xed\x01\x12\x1f\n\x19INPUT_CLUSTER_IN_PROGRESS\x10\xc3\xed\x01\x12\x1b\n\x15INPUT_REINDEX_SUCCESS\x10\xa4\xee\x01\x12\x1b\n\x15INPUT_REINDEX_PENDING\x10\xa5\xee\x01\x12\x1a\n\x14INPUT_REINDEX_FAILED\x10\xa6\xee\x01\x12\x1f\n\x19INPUT_REINDEX_IN_PROGRESS\x10\xa7\xee\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_SUCCESS\x10\x98\xf2\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_PENDING\x10\x99\xf2\x01\x12!\n\x1bINPUT_VIDEO_DOWNLOAD_FAILED\x10\x9a\xf2\x01\x12\x1b\n\x15INPUT_VIDEO_DUPLICATE\x10\xfc\xf2\x01\x12$\n\x1eINPUT_VIDEO_UNSUPPORTED_FORMAT\x10\xfd\xf2\x01\x12 \n\x1aINPUT_VIDEO_DOES_NOT_EXIST\x10\xfe\xf2\x01\x12#\n\x1dINPUT_VIDEO_PERMISSION_DENIED\x10\xff\xf2\x01\x12\"\n\x1cINPUT_VIDEO_INVALID_ARGUMENT\x10\x80\xf3\x01\x12\x1c\n\x16INPUT_VIDEO_OVER_LIMIT\x10\x81\xf3\x01\x12\x1d\n\x17INPUT_VIDEO_INVALID_URL\x10\x82\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_SUCCESS\x10\xe0\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_PENDING\x10\xe1\xf3\x01\x12\x1f\n\x19INPUT_VIDEO_MODIFY_FAILED\x10\xe3\xf3\x01\x12%\n\x1fINPUT_VIDEO_STORAGE_HOST_FAILED\x10\xea\xf3\x01\x12$\n\x1e\x41LL_INPUT_VIDEOS_INVALID_BYTES\x10\xc4\xf4\x01\x12\x1d\n\x17INPUT_CONNECTION_FAILED\x10\xbc\xb8\x02\x12&\n REQUEST_DISABLED_FOR_MAINTENANCE\x10\xbd\xb8\x02\x12+\n%INPUT_WRITES_DISABLED_FOR_MAINTENANCE\x10\xbe\xb8\x02\x12\x1b\n\x15INPUT_INVALID_REQUEST\x10\xbf\xb8\x02\x12\x1d\n\x17PREDICT_INVALID_REQUEST\x10\xc1\xb8\x02\x12\x1c\n\x16SEARCH_INVALID_REQUEST\x10\xc2\xb8\x02\x12\x1e\n\x18\x43ONCEPTS_INVALID_REQUEST\x10\xc3\xb8\x02\x12\x1b\n\x15STATS_INVALID_REQUEST\x10\xc4\xb8\x02\x12\x1c\n\x16\x44\x41TABASE_DUPLICATE_KEY\x10\xca\xb8\x02\x12 \n\x1a\x44\x41TABASE_STATEMENT_TIMEOUT\x10\xcb\xb8\x02\x12$\n\x1e\x44\x41TABASE_INVALID_ROWS_AFFECTED\x10\xcc\xb8\x02\x12 \n\x1a\x44\x41TABASE_DEADLOCK_DETECTED\x10\xcd\xb8\x02\x12\x18\n\x12\x44\x41TABASE_FAIL_TASK\x10\xce\xb8\x02\x12&\n DATABASE_FAIL_TO_GET_CONNECTIONS\x10\xcf\xb8\x02\x12\x1f\n\x19\x44\x41TABASE_TOO_MANY_CLIENTS\x10\xd0\xb8\x02\x12\"\n\x1c\x44\x41TABASE_CONSTRAINT_VIOLATED\x10\xd1\xb8\x02\x12\x17\n\x11\x44\x41TABASE_CANCELED\x10\xd5\xb8\x02\x12\x1f\n\x19\x41SYNC_WORKER_MULTI_ERRORS\x10\xd4\xb8\x02\x12\x1c\n\x16RPC_REQUEST_QUEUE_FULL\x10\xde\xb8\x02\x12\x1c\n\x16RPC_SERVER_UNAVAILABLE\x10\xdf\xb8\x02\x12\x19\n\x13RPC_REQUEST_TIMEOUT\x10\xe0\xb8\x02\x12#\n\x1dRPC_MAX_MESSAGE_SIZE_EXCEEDED\x10\xe1\xb8\x02\x12\x12\n\x0cRPC_CANCELED\x10\xe3\xb8\x02\x12\x18\n\x12RPC_UNKNOWN_METHOD\x10\xe4\xb8\x02\x12\x1e\n\x18REQUEST_CANCELED_BY_USER\x10\xe5\xb8\x02\x12\x1e\n\x18\x43LUSTER_INTERNAL_FAILURE\x10\xa0\xd0\x02\x12\x1f\n\x19\x45XTERNAL_CONNECTION_ERROR\x10\xe2\xb8\x02\x12\x1a\n\x14QUERY_INVALID_SYNTAX\x10\xf2\xb8\x02\x12\x16\n\x10QUEUE_CONN_ERROR\x10\xa8\xc0\x02\x12!\n\x1bQUEUE_CLOSE_REQUEST_TIMEOUT\x10\xaa\xc0\x02\x12\x17\n\x11QUEUE_CONN_CLOSED\x10\xab\xc0\x02\x12\x1f\n\x19QUEUE_PUBLISH_ACK_TIMEOUT\x10\xac\xc0\x02\x12\x19\n\x13QUEUE_PUBLISH_ERROR\x10\xad\xc0\x02\x12 \n\x1aQUEUE_SUBSCRIPTION_TIMEOUT\x10\xae\xc0\x02\x12\x1e\n\x18QUEUE_SUBSCRIPTION_ERROR\x10\xaf\xc0\x02\x12\x1e\n\x18QUEUE_MARSHALLING_FAILED\x10\xb0\xc0\x02\x12 \n\x1aQUEUE_UNMARSHALLING_FAILED\x10\xb1\xc0\x02\x12\'\n!QUEUE_MAX_MSG_REDELIVERY_EXCEEDED\x10\xb2\xc0\x02\x12\x17\n\x11QUEUE_ACK_FAILURE\x10\xb3\xc0\x02\x12\x13\n\rSQS_OVERLIMIT\x10\x8c\xc1\x02\x12 \n\x1aSQS_INVALID_RECEIPT_HANDLE\x10\x8d\xc1\x02\x12\x11\n\x0bSQS_UNKNOWN\x10\x8e\xc1\x02\x12\x1d\n\x17SEARCH_INTERNAL_FAILURE\x10\xf9\xcf\x02\x12\x1f\n\x19SEARCH_PROJECTION_FAILURE\x10\xfa\xcf\x02\x12\x1f\n\x19SEARCH_PREDICTION_FAILURE\x10\xfb\xcf\x02\x12\'\n!SEARCH_BY_NOT_FULLY_INDEXED_INPUT\x10\xfc\xcf\x02\x12 \n\x1aSAVED_SEARCH_MODIFY_FAILED\x10\xfd\xcf\x02\x12\x1f\n\x19SEARCH_COUNTS_UNAVAILABLE\x10\xfe\xcf\x02\x12\x17\n\x11\x45VALUATION_QUEUED\x10\xdc\xd0\x02\x12\x1c\n\x16\x45VALUATION_IN_PROGRESS\x10\xdd\xd0\x02\x12\x18\n\x12\x45VALUATION_SUCCESS\x10\xde\xd0\x02\x12(\n\"EVALUATION_FAILED_TO_RETRIEVE_DATA\x10\xdf\xd0\x02\x12!\n\x1b\x45VALUATION_INVALID_ARGUMENT\x10\xe0\xd0\x02\x12\x17\n\x11\x45VALUATION_FAILED\x10\xe1\xd0\x02\x12\x18\n\x12\x45VALUATION_PENDING\x10\xe2\xd0\x02\x12\x1a\n\x14\x45VALUATION_TIMED_OUT\x10\xe3\xd0\x02\x12!\n\x1b\x45VALUATION_UNEXPECTED_ERROR\x10\xe4\xd0\x02\x12\x16\n\x10\x45VALUATION_MIXED\x10\xe5\xd0\x02\x12\x18\n\x12STRIPE_EVENT_ERROR\x10\xe1\xd7\x02\x12\x10\n\nCACHE_MISS\x10\xc9\xdf\x02\x12&\n REDIS_SCRIPT_EXITED_WITH_FAILURE\x10\xca\xdf\x02\x12\x16\n\x10REDIS_STREAM_ERR\x10\xcb\xdf\x02\x12\x18\n\x12REDIS_NO_CONSUMERS\x10\xcc\xdf\x02\x12\x1a\n\x14REDIS_STREAM_BACKOFF\x10\xcd\xdf\x02\x12\x18\n\x12SIGNUP_EVENT_ERROR\x10\xb1\xe7\x02\x12\x14\n\x0eSIGNUP_FLAGGED\x10\xb2\xe7\x02\x12\x1a\n\x14\x46ILETYPE_UNSUPPORTED\x10\xb3\xe7\x02\x12\x1f\n\x19\x41PP_COUNT_INVALID_MESSAGE\x10\x99\xef\x02\x12\'\n!APP_COUNT_UPDATE_INCREMENT_FAILED\x10\x9a\xef\x02\x12\x1e\n\x18\x41PP_COUNT_REBUILD_FAILED\x10\x9b\xef\x02\x12 \n\x1a\x41PP_COUNT_INTERNAL_FAILURE\x10\x9c\xef\x02\x12\x17\n\x11MP_DOWNLOAD_ERROR\x10\xfd\xef\x02\x12\x1a\n\x14MP_RESOLVE_DNS_ERROR\x10\xfe\xef\x02\x12)\n#MP_DOWNLOAD_MAX_SIZE_EXCEEDED_ERROR\x10\xff\xef\x02\x12\x1b\n\x15MP_IMAGE_DECODE_ERROR\x10\x80\xf0\x02\x12\x19\n\x13MP_INVALID_ARGUMENT\x10\x81\xf0\x02\x12\x1f\n\x19MP_IMAGE_PROCESSING_ERROR\x10\x82\xf0\x02\x12\x19\n\x13\x44\x41TATIER_CONN_ERROR\x10\xe1\xf0\x02\x12\x17\n\x11USER_CONSENT_FACE\x10\xd1\x86\x03\x12\x14\n\x0eWORKER_MISSING\x10\xb8\x8e\x03\x12\x13\n\rWORKER_ACTIVE\x10\xb9\x8e\x03\x12\x15\n\x0fWORKER_INACTIVE\x10\xba\x8e\x03\x12\x17\n\x11\x43OLLECTOR_MISSING\x10\xa0\x96\x03\x12\x16\n\x10\x43OLLECTOR_ACTIVE\x10\xa1\x96\x03\x12\x18\n\x12\x43OLLECTOR_INACTIVE\x10\xa2\x96\x03\x12!\n\x1b\x43OLLECTOR_POST_INPUT_FAILED\x10\xa3\x96\x03\x12*\n$SSO_IDENTITY_PROVIDER_DOES_NOT_EXIST\x10\x89\x9e\x03\x12\x16\n\x10TASK_IN_PROGRESS\x10\xf1\xa5\x03\x12\x0f\n\tTASK_DONE\x10\xf2\xa5\x03\x12\x12\n\x0cTASK_WONT_DO\x10\xf3\xa5\x03\x12\"\n\x1cTASK_ADD_ANNOTATIONS_FAILURE\x10\xf5\xa5\x03\x12\x13\n\rTASK_CONFLICT\x10\xd4\xa6\x03\x12\x1a\n\x14TASK_NOT_IMPLEMENTED\x10\xd5\xa6\x03\x12\x12\n\x0cTASK_MISSING\x10\xd6\xa6\x03\x12\x19\n\x13LABEL_ORDER_PENDING\x10\xd9\xad\x03\x12\x1d\n\x17LABEL_ORDER_IN_PROGRESS\x10\xda\xad\x03\x12\x19\n\x13LABEL_ORDER_SUCCESS\x10\xdb\xad\x03\x12\x1a\n\x14LABEL_ORDER_CANCELED\x10\xdc\xad\x03\x12\x14\n\x0eLICENSE_ACTIVE\x10\xe0\xd4\x03\x12\x1c\n\x16LICENSE_DOES_NOT_EXIST\x10\xe1\xd4\x03\x12\x19\n\x13LICENSE_NEED_UPDATE\x10\xe2\xd4\x03\x12\x15\n\x0fLICENSE_EXPIRED\x10\xe3\xd4\x03\x12\x15\n\x0fLICENSE_REVOKED\x10\xe4\xd4\x03\x12\x15\n\x0fLICENSE_DELETED\x10\xe5\xd4\x03\x12\x1d\n\x17LICENSE_VOLUME_EXCEEDED\x10\xe6\xd4\x03\x12!\n\x1bPASSWORD_VALIDATION_SUCCESS\x10\xc8\xdc\x03\x12 \n\x1aPASSWORD_VALIDATION_FAILED\x10\xc9\xdc\x03\x12%\n\x1fPASSWORDPOLICY_INVALID_ARGUMENT\x10\xca\xdc\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_CONFIG_NOT_FOUND\x10\xb0\xe4\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_INVALID_ARGUMENT\x10\xb1\xe4\x03\x12\x19\n\x13\x46\x45\x41TUREFLAG_BLOCKED\x10\xb2\xe4\x03\x12\x19\n\x13MAINTENANCE_SUCCESS\x10\x98\xec\x03\x12\x18\n\x12MAINTENANCE_FAILED\x10\x99\xec\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_PENDING\x10\x85\xf4\x03\x12!\n\x1b\x44\x41TASET_VERSION_IN_PROGRESS\x10\x8a\xf4\x03\x12\x1b\n\x15\x44\x41TASET_VERSION_READY\x10\x8f\xf4\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_FAILURE\x10\x94\xf4\x03\x12&\n DATASET_VERSION_UNEXPECTED_ERROR\x10\x99\xf4\x03\x12\x1e\n\x18\x44\x41TASET_VERSION_CONFLICT\x10\x9e\xf4\x03\x12\x1b\n\x15\x44\x41TASET_INPUT_SUCCESS\x10\xe4\xf4\x03\x12\x1d\n\x17\x44\x41TASET_INPUT_DUPLICATE\x10\xe5\xf4\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_SUCCESS\x10\xc8\xf5\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_PENDING\x10\xc9\xf5\x03\x12#\n\x1d\x44\x41TASET_VERSION_EXPORT_FAILED\x10\xca\xf5\x03\x12(\n\"DATASET_VERSION_EXPORT_IN_PROGRESS\x10\xcb\xf5\x03\x12-\n\'DATASET_VERSION_EXPORT_UNEXPECTED_ERROR\x10\xcc\xf5\x03\x12\x10\n\nJOB_QUEUED\x10\x80\xf4\x03\x12\x11\n\x0bJOB_RUNNING\x10\x81\xf4\x03\x12\x13\n\rJOB_COMPLETED\x10\x82\xf4\x03\x12\x10\n\nJOB_FAILED\x10\x83\xf4\x03\x12\x13\n\rJOB_CANCELLED\x10\x84\xf4\x03\x12\x1a\n\x14JOB_UNEXPECTED_ERROR\x10\x86\xf4\x03\x12\x1c\n\x16\x41UTH_MISSING_IDP_ASSOC\x10\xe8\xfb\x03\x12\x19\n\x13LIST_OBJECTS_FAILED\x10\xd0\x83\x04\x12\x1c\n\x16\x41RCHIVE_EXTRACT_FAILED\x10\xb8\x8b\x04\x12\x18\n\x12UPLOAD_IN_PROGRESS\x10\xa0\x93\x04\x12\x11\n\x0bUPLOAD_DONE\x10\xa1\x93\x04\x12\x13\n\rUPLOAD_FAILED\x10\xa2\x93\x04\x12\x1d\n\x17UPLOAD_UNEXPECTED_ERROR\x10\xa3\x93\x04\x12\x14\n\x0eUPLOAD_EXPIRED\x10\xa4\x93\x04\x12\x1a\n\x14\x42ILLING_INVALID_INFO\x10\x88\x9b\x04\x12\x1b\n\x15INTERNAL_SERVER_ISSUE\x10\xd4\xfd\x05\x12\x1d\n\x17INTERNAL_FETCHING_ISSUE\x10\xd5\xfd\x05\x12\x1d\n\x17INTERNAL_DATABASE_ISSUE\x10\xd6\xfd\x05\x12!\n\x1bINTERNAL_UNEXPECTED_TIMEOUT\x10\xd9\xfd\x05\x12\x1c\n\x16INTERNAL_UNEXPECTED_V1\x10\xda\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_PANIC\x10\xdb\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_SPIRE\x10\xdc\xfd\x05\x12 \n\x1aINTERNAL_REDIS_UNAVAILABLE\x10\xdd\xfd\x05\x12!\n\x1bINTERNAL_RESOURCE_EXHAUSTED\x10\xde\xfd\x05\x12\"\n\x1cINTERNAL_REDIS_UNCATEGORIZED\x10\xdf\xfd\x05\x12 \n\x1aINTERNAL_AWS_UNCATEGORIZED\x10\xe0\xfd\x05\x12\"\n\x1cINTERNAL_AZURE_UNCATEGORIZED\x10\xe1\xfd\x05\x12\x18\n\x12\x43ONN_UNCATEGORIZED\x10\xb9\x85\x06\x12\x19\n\x13MODEL_UNCATEGORIZED\x10\xba\x85\x06\x12\x19\n\x13INPUT_UNCATEGORIZED\x10\xbb\x85\x06\x12\x1e\n\x18\x41NNOTATION_UNCATEGORIZED\x10\xbc\x85\x06\x12\x1b\n\x15\x42ILLING_UNCATEGORIZED\x10\xbd\x85\x06\x12\x1c\n\x16INTERNAL_UNCATEGORIZED\x10\xc1\x85\x06\x12\x11\n\x0b\x42\x41\x44_REQUEST\x10\xa0\xc2\x05\x12\x12\n\x0cSERVER_ERROR\x10\x84\xc3\x05\"\x08\x08\xbf\xc6\x01\x10\xbf\xc6\x01\"\x08\x08\xe8\x81\x02\x10\xe8\x81\x02\"\x08\x08\xe9\x81\x02\x10\xe9\x81\x02\"\x08\x08\xea\x81\x02\x10\xea\x81\x02\"\x08\x08\xcc\x82\x02\x10\xcc\x82\x02\"\x08\x08\xcd\x82\x02\x10\xcd\x82\x02\"\x08\x08\xce\x82\x02\x10\xce\x82\x02\"\x08\x08\xcf\x82\x02\x10\xcf\x82\x02\"\x08\x08\xd0\x82\x02\x10\xd0\x82\x02\"\x08\x08\xd1\x82\x02\x10\xd1\x82\x02\"\x08\x08\xd2\x82\x02\x10\xd2\x82\x02\"\x08\x08\xb0\x83\x02\x10\xb0\x83\x02\"\x08\x08\xb1\x83\x02\x10\xb1\x83\x02\"\x08\x08\xb3\x83\x02\x10\xb3\x83\x02\"\x08\x08\xba\x83\x02\x10\xba\x83\x02\"\x08\x08\xbb\xb8\x02\x10\xbb\xb8\x02\"\x08\x08\xd2\xb8\x02\x10\xd2\xb8\x02\"\x08\x08\xd3\xb8\x02\x10\xd3\xb8\x02\"\x08\x08\xf0\xc1\x02\x10\xf0\xc1\x02\"\x08\x08\xf1\xc1\x02\x10\xf1\xc1\x02\"\x08\x08\xf2\xc1\x02\x10\xf2\xc1\x02\"\x08\x08\xf3\xc1\x02\x10\xf3\xc1\x02\"\x08\x08\xf4\xc1\x02\x10\xf4\xc1\x02\"\x08\x08\x9c\xc7\x01\x10\x9c\xc7\x01\"\x08\x08\x9d\xc7\x01\x10\x9d\xc7\x01\"\x08\x08\x9e\xc7\x01\x10\x9e\xc7\x01\"\x08\x08\x9f\xc7\x01\x10\x9f\xc7\x01\"\x08\x08\xa1\xc7\x01\x10\xa1\xc7\x01\"\x08\x08\xa2\xc7\x01\x10\xa2\xc7\x01\x42g\n\x1c\x63om.clarifai.grpc.api.statusP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.status.status_code_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.clarifai.grpc.api.statusP\001Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\242\002\004CAIP'
   _STATUSCODE.values_by_name["CONN_TOKEN_INVALID"]._options = None
   _STATUSCODE.values_by_name["CONN_TOKEN_INVALID"]._serialized_options = b'\010\001'
   _STATUSCODE.values_by_name["MODEL_TRAINING_MSG_REDELIVER"]._options = None
   _STATUSCODE.values_by_name["MODEL_TRAINING_MSG_REDELIVER"]._serialized_options = b'\010\001'
   _STATUSCODE.values_by_name["MODEL_EVALUATION_MSG_REDELIVER"]._options = None
   _STATUSCODE.values_by_name["MODEL_EVALUATION_MSG_REDELIVER"]._serialized_options = b'\010\001'
   _STATUSCODE._serialized_start=69
-  _STATUSCODE._serialized_end=10406
+  _STATUSCODE._serialized_end=10464
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
     DATABASE_STATEMENT_TIMEOUT: _StatusCode.ValueType  # 40011
     DATABASE_INVALID_ROWS_AFFECTED: _StatusCode.ValueType  # 40012
     DATABASE_DEADLOCK_DETECTED: _StatusCode.ValueType  # 40013
     DATABASE_FAIL_TASK: _StatusCode.ValueType  # 40014
     DATABASE_FAIL_TO_GET_CONNECTIONS: _StatusCode.ValueType  # 40015
     DATABASE_TOO_MANY_CLIENTS: _StatusCode.ValueType  # 40016
     DATABASE_CONSTRAINT_VIOLATED: _StatusCode.ValueType  # 40017
+    DATABASE_CANCELED: _StatusCode.ValueType  # 40021
     ASYNC_WORKER_MULTI_ERRORS: _StatusCode.ValueType  # 40020
     RPC_REQUEST_QUEUE_FULL: _StatusCode.ValueType  # 40030
     RPC_SERVER_UNAVAILABLE: _StatusCode.ValueType  # 40031
     RPC_REQUEST_TIMEOUT: _StatusCode.ValueType  # 40032
     RPC_MAX_MESSAGE_SIZE_EXCEEDED: _StatusCode.ValueType  # 40033
     RPC_CANCELED: _StatusCode.ValueType  # 40035
     RPC_UNKNOWN_METHOD: _StatusCode.ValueType  # 40036
@@ -318,14 +319,15 @@
     SQS_UNKNOWN: _StatusCode.ValueType  # 41102
     SEARCH_INTERNAL_FAILURE: _StatusCode.ValueType  # 43001
     """Search related errors 43xxxx"""
     SEARCH_PROJECTION_FAILURE: _StatusCode.ValueType  # 43002
     SEARCH_PREDICTION_FAILURE: _StatusCode.ValueType  # 43003
     SEARCH_BY_NOT_FULLY_INDEXED_INPUT: _StatusCode.ValueType  # 43004
     SAVED_SEARCH_MODIFY_FAILED: _StatusCode.ValueType  # 43005
+    SEARCH_COUNTS_UNAVAILABLE: _StatusCode.ValueType  # 43006
     EVALUATION_QUEUED: _StatusCode.ValueType  # 43100
     """Workflow evaluation err code"""
     EVALUATION_IN_PROGRESS: _StatusCode.ValueType  # 43101
     EVALUATION_SUCCESS: _StatusCode.ValueType  # 43102
     EVALUATION_FAILED_TO_RETRIEVE_DATA: _StatusCode.ValueType  # 43103
     EVALUATION_INVALID_ARGUMENT: _StatusCode.ValueType  # 43104
     EVALUATION_FAILED: _StatusCode.ValueType  # 43105
@@ -754,14 +756,15 @@
 DATABASE_STATEMENT_TIMEOUT: StatusCode.ValueType  # 40011
 DATABASE_INVALID_ROWS_AFFECTED: StatusCode.ValueType  # 40012
 DATABASE_DEADLOCK_DETECTED: StatusCode.ValueType  # 40013
 DATABASE_FAIL_TASK: StatusCode.ValueType  # 40014
 DATABASE_FAIL_TO_GET_CONNECTIONS: StatusCode.ValueType  # 40015
 DATABASE_TOO_MANY_CLIENTS: StatusCode.ValueType  # 40016
 DATABASE_CONSTRAINT_VIOLATED: StatusCode.ValueType  # 40017
+DATABASE_CANCELED: StatusCode.ValueType  # 40021
 ASYNC_WORKER_MULTI_ERRORS: StatusCode.ValueType  # 40020
 RPC_REQUEST_QUEUE_FULL: StatusCode.ValueType  # 40030
 RPC_SERVER_UNAVAILABLE: StatusCode.ValueType  # 40031
 RPC_REQUEST_TIMEOUT: StatusCode.ValueType  # 40032
 RPC_MAX_MESSAGE_SIZE_EXCEEDED: StatusCode.ValueType  # 40033
 RPC_CANCELED: StatusCode.ValueType  # 40035
 RPC_UNKNOWN_METHOD: StatusCode.ValueType  # 40036
@@ -788,14 +791,15 @@
 SQS_UNKNOWN: StatusCode.ValueType  # 41102
 SEARCH_INTERNAL_FAILURE: StatusCode.ValueType  # 43001
 """Search related errors 43xxxx"""
 SEARCH_PROJECTION_FAILURE: StatusCode.ValueType  # 43002
 SEARCH_PREDICTION_FAILURE: StatusCode.ValueType  # 43003
 SEARCH_BY_NOT_FULLY_INDEXED_INPUT: StatusCode.ValueType  # 43004
 SAVED_SEARCH_MODIFY_FAILED: StatusCode.ValueType  # 43005
+SEARCH_COUNTS_UNAVAILABLE: StatusCode.ValueType  # 43006
 EVALUATION_QUEUED: StatusCode.ValueType  # 43100
 """Workflow evaluation err code"""
 EVALUATION_IN_PROGRESS: StatusCode.ValueType  # 43101
 EVALUATION_SUCCESS: StatusCode.ValueType  # 43102
 EVALUATION_FAILED_TO_RETRIEVE_DATA: StatusCode.ValueType  # 43103
 EVALUATION_INVALID_ARGUMENT: StatusCode.ValueType  # 43104
 EVALUATION_FAILED: StatusCode.ValueType  # 43105
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/status/status_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/status/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/types/types_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/util/extension_pb2.py` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/util/extension_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi` & `clarifai-grpc-9.4.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc.egg-info/PKG-INFO` & `clarifai-grpc-9.4.0/clarifai_grpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai-grpc
-Version: 9.3.0
+Version: 9.4.0
 Summary: Clarifai gRPC API Client
 Home-page: https://github.com/Clarifai/clarifai-python-grpc
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-grpc-9.3.0/clarifai_grpc.egg-info/SOURCES.txt` & `clarifai-grpc-9.4.0/clarifai_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.3.0/setup.py` & `clarifai-grpc-9.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_packages(include=["clarifai_grpc*"])
 
 setuptools.setup(
     name="clarifai-grpc",
-    version="9.3.0",
+    version="9.4.0",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai gRPC API Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-grpc",
     packages=packages,
```

