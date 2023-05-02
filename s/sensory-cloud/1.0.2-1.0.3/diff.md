# Comparing `tmp/sensory_cloud-1.0.2.tar.gz` & `tmp/sensory_cloud-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensory_cloud-1.0.2.tar", last modified: Fri Apr 21 18:52:01 2023, max compression
+gzip compressed data, was "sensory_cloud-1.0.3.tar", last modified: Tue May  2 13:35:40 2023, max compression
```

## Comparing `sensory_cloud-1.0.2.tar` & `sensory_cloud-1.0.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.647934 sensory_cloud-1.0.2/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    11357 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/LICENSE.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)       24 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/MANIFEST.in
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-04-21 18:52:01.647278 sensory_cloud-1.0.2/PKG-INFO
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      948 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/README.md
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/requirements.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)       38 2023-04-21 18:52:01.648256 sensory_cloud-1.0.2/setup.cfg
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      740 2023-04-21 18:52:01.000000 sensory_cloud-1.0.2/setup.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.590201 sensory_cloud-1.0.2/src/
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.600577 sensory_cloud-1.0.2/src/sensory_cloud/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2923 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/config.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.603914 sensory_cloud-1.0.2/src/sensory_cloud/generated/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/__init__.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.605601 sensory_cloud-1.0.2/src/sensory_cloud/generated/common/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/common/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    59354 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/common/common_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/common/common_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.607461 sensory_cloud-1.0.2/src/sensory_cloud/generated/health/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/health/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2976 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/health/health_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2592 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/health/health_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.609865 sensory_cloud-1.0.2/src/sensory_cloud/generated/oauth/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/oauth/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    15147 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/oauth/oauth_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     8049 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.611037 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/__init__.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.614035 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/assistant/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/assistant/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     8671 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2827 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.617702 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/audio/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/audio/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)   125215 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/audio/audio_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    18777 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.620240 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/event/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/event/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    37387 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/event/event_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     8197 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.622638 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/file/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/file/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    24268 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/file/file_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     7750 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.627332 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    26140 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/device_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    13034 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    43642 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/enrollment_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    18293 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.630442 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/video/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/video/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    52347 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/video/video_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     9870 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.633102 sensory_cloud-1.0.2/src/sensory_cloud/generated/validate/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/validate/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)   113401 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/validate/validate_pb2.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-04-21 13:35:41.000000 sensory_cloud-1.0.2/src/sensory_cloud/generated/validate/validate_pb2_grpc.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     9344 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/initializer.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.640991 sensory_cloud-1.0.2/src/sensory_cloud/services/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/services/__init__.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    25738 2023-02-28 14:22:02.000000 sensory_cloud-1.0.2/src/sensory_cloud/services/audio_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      642 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/services/crypto_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1253 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/services/health_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     6001 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/services/management_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     9735 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/services/oauth_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    11253 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/services/video_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2170 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/src/sensory_cloud/token_manager.py
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.603398 sensory_cloud-1.0.2/src/sensory_cloud.egg-info/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-04-21 18:52:01.000000 sensory_cloud-1.0.2/src/sensory_cloud.egg-info/PKG-INFO
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     2664 2023-04-21 18:52:01.000000 sensory_cloud-1.0.2/src/sensory_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)        1 2023-04-21 18:52:01.000000 sensory_cloud-1.0.2/src/sensory_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-04-21 18:52:01.000000 sensory_cloud-1.0.2/src/sensory_cloud.egg-info/requires.txt
--rw-r--r--   0 jonathanhersch   (504) staff       (20)       14 2023-04-21 18:52:01.000000 sensory_cloud-1.0.2/src/sensory_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-04-21 18:52:01.646354 sensory_cloud-1.0.2/test/
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    23719 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/test/test_audio_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)      638 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/test/test_crypto_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     1450 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/test/test_health_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     6780 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/test/test_management_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    10159 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/test/test_oauth_service.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)     3756 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/test/test_token_manager.py
--rw-r--r--   0 jonathanhersch   (504) staff       (20)    10951 2023-02-08 16:23:22.000000 sensory_cloud-1.0.2/test/test_video_service.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.036136 sensory_cloud-1.0.3/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    11357 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/LICENSE.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)       24 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/MANIFEST.in
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-05-02 13:35:40.035353 sensory_cloud-1.0.3/PKG-INFO
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      948 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/README.md
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/requirements.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)       38 2023-05-02 13:35:40.036548 sensory_cloud-1.0.3/setup.cfg
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      740 2023-05-02 12:48:44.000000 sensory_cloud-1.0.3/setup.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.978559 sensory_cloud-1.0.3/src/
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.989224 sensory_cloud-1.0.3/src/sensory_cloud/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2799 2023-05-02 13:20:01.000000 sensory_cloud-1.0.3/src/sensory_cloud/config.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.992920 sensory_cloud-1.0.3/src/sensory_cloud/generated/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/__init__.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.994446 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    59354 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/common_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/common/common_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.996389 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2976 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2592 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.998243 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    15147 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     8049 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.998940 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/__init__.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.001145 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     8671 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2827 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.003533 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)   125215 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    18777 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.005836 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    37387 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     8197 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.007820 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    24268 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     7750 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.011634 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    26140 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    13034 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    43642 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    18293 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.014717 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    52347 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     9870 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.017110 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)   113401 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/validate_pb2.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      159 2023-04-21 13:35:41.000000 sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/validate_pb2_grpc.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    12350 2023-05-02 13:35:32.000000 sensory_cloud-1.0.3/src/sensory_cloud/initializer.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.024253 sensory_cloud-1.0.3/src/sensory_cloud/services/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        0 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/__init__.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    25738 2023-02-28 14:22:02.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/audio_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      642 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/crypto_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1253 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/health_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     6001 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/management_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     9735 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/oauth_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    11253 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/services/video_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2170 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/src/sensory_cloud/token_manager.py
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:39.992243 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1249 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     2664 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)        1 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      146 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/requires.txt
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)       14 2023-05-02 13:35:39.000000 sensory_cloud-1.0.3/src/sensory_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 jonathanhersch   (504) staff       (20)        0 2023-05-02 13:35:40.033724 sensory_cloud-1.0.3/test/
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    23719 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_audio_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)      638 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_crypto_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     1450 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_health_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     6780 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_management_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    10159 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_oauth_service.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)     3756 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_token_manager.py
+-rw-r--r--   0 jonathanhersch   (504) staff       (20)    10951 2023-02-08 16:23:22.000000 sensory_cloud-1.0.3/test/test_video_service.py
```

### Comparing `sensory_cloud-1.0.2/LICENSE.txt` & `sensory_cloud-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/PKG-INFO` & `sensory_cloud-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensory_cloud
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for Sensory Cloud
 Home-page: https://github.com/Sensory-Cloud/python-sdk
 Author: Jonathan Hersch
 Author-email: jhersch@sensoryinc.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `sensory_cloud-1.0.2/README.md` & `sensory_cloud-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/setup.py` & `sensory_cloud-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = requirements_txt.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sensory_cloud",
-    version="1.0.2",
+    version="1.0.3",
     description="Python SDK for Sensory Cloud",
     author="Jonathan Hersch",
     author_email="jhersch@sensoryinc.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=requirements,
     python_requires='>=3.6',
```

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/config.py` & `sensory_cloud-1.0.3/src/sensory_cloud/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,25 +16,21 @@
     def __init__(
         self,
         fully_qualified_domain_name: str,
         tenant_id: str,
         is_connection_secure: bool,
         enrollment_type: EnrollmentType,
         credential: str,
-        device_id: str,
-        device_name: str,
     ):
 
         self.fully_qualified_domain_name = fully_qualified_domain_name
         self.tenant_id = tenant_id
         self.is_connection_secure = is_connection_secure
         self.enrollment_type = enrollment_type
         self.credential = credential
-        self.device_id = device_id
-        self.device_name = device_name
 
 
 class CloudHost:
     """
     Class for providing info on a cloud host
     """
```

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/common/common_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/health/health_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/health/health_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/health/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/oauth/oauth_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/oauth/oauth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/assistant/assistant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/audio/audio_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/audio/audio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/event/event_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/event/event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/file/file_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/file/file_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/device_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/enrollment_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/management/enrollment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/video/video_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/v1/video/video_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/generated/validate/validate_pb2.py` & `sensory_cloud-1.0.3/src/sensory_cloud/generated/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/initializer.py` & `sensory_cloud-1.0.3/src/sensory_cloud/initializer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 import binascii
 import typing
 import base64
 import configparser
+import uuid
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
 
 from sensory_cloud.config import (
     Config,
     CloudHost,
     EnrollmentType,
     SDKConfig,
@@ -18,14 +19,49 @@
     ISecureCredentialStore,
     GenericCredentialStore,
 )
 
 import sensory_cloud.generated.v1.management.device_pb2 as device_pb2
 
 
+class FileSystemCredentialStore:
+    """A file-system--based credential storage manager."""
+
+    def __init__(self, root_path: str, package: str = "sensory-cloud"):
+        """Initialize a new secure credential storage interface."""
+        self._root_path = root_path
+        self._package = package
+
+    def __setitem__(self, key: str, value: str):
+        """Emplace or replace a key/value pair in the secure credential store.
+
+        Unlike most key-value store abstractions in the STL, this implementation of
+        emplace will overwrite existing values in the key-value store.
+        """
+        with open(self._key_path(key), "w") as output_file:
+            output_file.write(value)
+
+    def __contains__(self, key: str) -> bool:
+        """Return True if the key exists in the secure credential store."""
+        return os.path.isfile(self._key_path(key))
+
+    def __getitem__(self, key: str) -> str:
+        """Look-up a secret value in the secure credential store."""
+        with open(self._key_path(key)) as input_file:
+            return input_file.read().strip()
+
+    def __delitem__(self, key: str):
+        """Remove a secret key-value pair in the secure credential store."""
+        os.remove(self._key_path(key))
+
+    def _key_path(self, key: str) -> str:
+        """Return the path of the given key."""
+        return os.path.join(self._root_path, f"{self._package}.{key}")
+
+
 class Initializer:
     """
     Initialization class used to register a device
     """
 
     _enrollment_type_map: dict = {
         "none": EnrollmentType.none,
@@ -33,32 +69,70 @@
         "jwt": EnrollmentType.jwt,
     }
 
     def __init__(
         self,
         init_config: typing.Union[str, SDKConfig],
         secure_credential_store: ISecureCredentialStore = None,
+        keychain: FileSystemCredentialStore = None,
     ):
         """
         Constructor method to generate an Initializer object
 
         Arguments:
             init_config (str or SDKConfig): The init_config argument can either be a string
                 containing the path to a .ini config file or an SDKConfig object containing
                 the required configuration information
             secure_credential_store (ISecureCredentialStore): The secure_credential_store
                 argument is an ISecureCredentialStore abstract class object.  If it is set to
                 None then the client credentials will be written to a GenericCredentialStore
                 object
+            keychain (FileSystemCredentialStore): The keychain will store the location of
+                and the values of the device id and device name if they are not set as
+                environment variables
         """
 
         self.init_config: typing.Union[str, SDKConfig] = init_config
         self.secure_credential_store: ISecureCredentialStore = secure_credential_store
+        self.keychain = keychain
         self.sdk_config: SDKConfig = None
         self.config_parser: configparser.ConfigParser = None
+        self.device_id = None
+        self.device_name = None
+
+    def _get_device_information(self) -> None:
+        """
+        Private method that first checks environment variables for device information.
+        If the device information is not set as environment variables then the device information
+        will be retrieved from the keychain initialization argument.  If the keychain does not 
+        contain the device information then it will be randomly generated and written to the current
+        working directory.
+        """
+        
+        device_id = os.environ.get("SENSORYCLOUD_DEVICE_ID")
+        device_name = os.environ.get("SENSORYCLOUD_DEVICE_NAME")
+        
+        if device_id is None:
+            if self.keychain is None:
+                self.keychain = FileSystemCredentialStore(root_path=os.getcwd())
+                
+            if 'deviceID' in self.keychain:
+                device_id = self.keychain["deviceID"]
+            else:
+                device_id = str(uuid.uuid1())
+                self.keychain["deviceID"] = device_id
+                
+            if 'deviceName' in self.keychain:
+                device_name = self.keychain["deviceName"]
+            else:
+                device_name = str(uuid.uuid1())
+                self.keychain["deviceName"] = device_name
+                
+        self.device_id = device_id
+        self.device_name = device_name
 
     def _read_config_from_file(self) -> None:
         """
         Private method that sets the sdk_config attribute in the case that the init_config
         attribute is a path to a config file
         """
 
@@ -75,16 +149,14 @@
             ),
             tenant_id=sdk_config_parser.get("tenantId"),
             is_connection_secure=sdk_config_parser.getboolean("isSecure"),
             enrollment_type=self._enrollment_type_map[
                 sdk_config_parser.get("enrollmentType")
             ],
             credential=sdk_config_parser.get("credential"),
-            device_id=sdk_config_parser.get("deviceId"),
-            device_name=sdk_config_parser.get("deviceName"),
         )
 
         if (
             "client-configuration" in self.config_parser
             and self.secure_credential_store is None
         ):
             client_config_parser: configparser.SectionProxy = self.config_parser[
@@ -207,14 +279,16 @@
         Returns:
             If the device enrollment is successful then a device_pb2.DeviceResponse
             object will be returned.  If the device is already enrolled or another
             device is enrolled with the client credentials specified, then an
             Exception will be returned.
         """
 
+        self._get_device_information()
+
         if isinstance(self.init_config, str):
             if not os.path.exists(self.init_config):
                 raise Exception(f"The path, {self.init_config}, does not exist")
             self._read_config_from_file()
         elif isinstance(self.init_config, SDKConfig):
             self.sdk_config = self.init_config
         else:
@@ -234,27 +308,27 @@
         config: Config = self._get_config()
         oauth_service: OauthService = OauthService(
             config=config, secure_credential_store=self.secure_credential_store
         )
 
         try:
             device_response = oauth_service.get_who_am_i()
-            device_is_registered = self.sdk_config.device_id == device_response.deviceId
+            device_is_registered = self.device_id == device_response.deviceId
             if not device_is_registered:
                 err: str = f"Another device with deviceId = {device_response.deviceId} is already enrolled with this client"
                 print(err)
                 return Exception(err)
         except Exception as e:
             device_is_registered = False
 
         if not device_is_registered:
             credential: str = self._get_credential()
             response: device_pb2.DeviceResponse = oauth_service.register(
-                device_id=self.sdk_config.device_id,
-                device_name=self.sdk_config.device_name,
+                device_id=self.device_id,
+                device_name=self.device_name,
                 credential=credential,
             )
             if self.config_parser is not None:
                 self._update_config_file()
         else:
             err: str = "This device is already enrolled"
             print(err)
```

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/services/audio_service.py` & `sensory_cloud-1.0.3/src/sensory_cloud/services/audio_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/services/crypto_service.py` & `sensory_cloud-1.0.3/src/sensory_cloud/services/crypto_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/services/health_service.py` & `sensory_cloud-1.0.3/src/sensory_cloud/services/health_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/services/management_service.py` & `sensory_cloud-1.0.3/src/sensory_cloud/services/management_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/services/oauth_service.py` & `sensory_cloud-1.0.3/src/sensory_cloud/services/oauth_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/services/video_service.py` & `sensory_cloud-1.0.3/src/sensory_cloud/services/video_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud/token_manager.py` & `sensory_cloud-1.0.3/src/sensory_cloud/token_manager.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud.egg-info/PKG-INFO` & `sensory_cloud-1.0.3/src/sensory_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensory-cloud
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for Sensory Cloud
 Home-page: https://github.com/Sensory-Cloud/python-sdk
 Author: Jonathan Hersch
 Author-email: jhersch@sensoryinc.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `sensory_cloud-1.0.2/src/sensory_cloud.egg-info/SOURCES.txt` & `sensory_cloud-1.0.3/src/sensory_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/test/test_audio_service.py` & `sensory_cloud-1.0.3/test/test_audio_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/test/test_crypto_service.py` & `sensory_cloud-1.0.3/test/test_crypto_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/test/test_health_service.py` & `sensory_cloud-1.0.3/test/test_health_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/test/test_management_service.py` & `sensory_cloud-1.0.3/test/test_management_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/test/test_oauth_service.py` & `sensory_cloud-1.0.3/test/test_oauth_service.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/test/test_token_manager.py` & `sensory_cloud-1.0.3/test/test_token_manager.py`

 * *Files identical despite different names*

### Comparing `sensory_cloud-1.0.2/test/test_video_service.py` & `sensory_cloud-1.0.3/test/test_video_service.py`

 * *Files identical despite different names*

