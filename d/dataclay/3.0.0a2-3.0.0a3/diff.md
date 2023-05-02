# Comparing `tmp/dataClay-3.0.0a2.tar.gz` & `tmp/dataClay-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataClay-3.0.0a2.tar", last modified: Thu Feb 23 12:17:20 2023, max compression
+gzip compressed data, was "dataClay-3.0.0a3.tar", last modified: Mon Mar  6 12:54:35 2023, max compression
```

## Comparing `dataClay-3.0.0a2.tar` & `dataClay-3.0.0a3.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/
--rw-rw-r--   0 marc      (1000) marc      (1000)     1529 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/LICENSE.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)       25 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/MANIFEST.in
--rw-rw-r--   0 marc      (1000) marc      (1000)     2492 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)     1495 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/README.md
--rw-rw-r--   0 marc      (1000) marc      (1000)      263 2022-12-23 16:56:00.000000 dataClay-3.0.0a2/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1000)     1219 2023-02-23 12:17:20.415231 dataClay-3.0.0a2/setup.cfg
--rw-rw-r--   0 marc      (1000) marc      (1000)       69 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/setup.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.391231 dataClay-3.0.0a2/src/
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.391231 dataClay-3.0.0a2/src/dataClay.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1000)     2492 2023-02-23 12:17:20.000000 dataClay-3.0.0a2/src/dataClay.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)     6739 2023-02-23 12:17:20.000000 dataClay-3.0.0a2/src/dataClay.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        1 2023-02-23 12:17:20.000000 dataClay-3.0.0a2/src/dataClay.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)      107 2023-02-23 12:17:20.000000 dataClay-3.0.0a2/src/dataClay.egg-info/requires.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)       17 2023-02-23 12:17:20.000000 dataClay-3.0.0a2/src/dataClay.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.391231 dataClay-3.0.0a2/src/dataclay/
--rw-rw-r--   0 marc      (1000) marc      (1000)      260 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.391231 dataClay-3.0.0a2/src/dataclay/backend/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/backend/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      186 2023-01-16 16:24:49.000000 dataClay-3.0.0a2/src/dataclay/backend/__main__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    42257 2023-02-09 16:44:44.000000 dataClay-3.0.0a2/src/dataclay/backend/api.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    18683 2023-02-01 17:07:16.000000 dataClay-3.0.0a2/src/dataclay/backend/client.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     7436 2023-01-17 14:49:03.000000 dataClay-3.0.0a2/src/dataclay/backend/heapmanager.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    14319 2023-01-31 14:05:38.000000 dataClay-3.0.0a2/src/dataclay/backend/runtime.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    17417 2023-02-17 10:36:39.000000 dataClay-3.0.0a2/src/dataclay/backend/servicer.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.395231 dataClay-3.0.0a2/src/dataclay/client/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/client/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5790 2023-01-31 15:34:21.000000 dataClay-3.0.0a2/src/dataclay/client/api.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     7536 2023-01-31 14:07:01.000000 dataClay-3.0.0a2/src/dataclay/client/runtime.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.395231 dataClay-3.0.0a2/src/dataclay/conf/
--rw-rw-r--   0 marc      (1000) marc      (1000)     5568 2023-02-17 10:36:38.000000 dataClay-3.0.0a2/src/dataclay/conf/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.395231 dataClay-3.0.0a2/src/dataclay/contrib/
--rw-rw-r--   0 marc      (1000) marc      (1000)       89 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     7335 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/collections.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.395231 dataClay-3.0.0a2/src/dataclay/contrib/dataclay_dummy/
--rw-rw-r--   0 marc      (1000) marc      (1000)      997 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/dataclay_dummy/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      947 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/dummy_pycompss.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1340 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/kafka.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1520 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/mqtt.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    11787 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/splitting.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      551 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/contrib/synchronization.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    18433 2023-02-01 17:01:29.000000 dataClay-3.0.0a2/src/dataclay/dataclay_object.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.395231 dataClay-3.0.0a2/src/dataclay/exceptions/
--rw-rw-r--   0 marc      (1000) marc      (1000)      756 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/exceptions/ErrorDefs.py
--rw-rw-r--   0 marc      (1000) marc      (1000)       45 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/exceptions/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     6205 2023-02-01 17:07:47.000000 dataClay-3.0.0a2/src/dataclay/exceptions/exceptions.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.395231 dataClay-3.0.0a2/src/dataclay/metadata/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/metadata/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1974 2023-02-17 10:36:39.000000 dataClay-3.0.0a2/src/dataclay/metadata/__main__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    10546 2023-01-31 14:27:40.000000 dataClay-3.0.0a2/src/dataclay/metadata/api.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3259 2022-12-29 12:23:20.000000 dataClay-3.0.0a2/src/dataclay/metadata/cli.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4798 2023-02-15 14:14:44.000000 dataClay-3.0.0a2/src/dataclay/metadata/client.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5272 2023-02-23 11:18:12.000000 dataClay-3.0.0a2/src/dataclay/metadata/kvdata.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2357 2023-01-16 13:59:40.000000 dataClay-3.0.0a2/src/dataclay/metadata/redismanager.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5895 2023-01-31 14:17:42.000000 dataClay-3.0.0a2/src/dataclay/metadata/servicer.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.395231 dataClay-3.0.0a2/src/dataclay/paraver/
--rw-rw-r--   0 marc      (1000) marc      (1000)    14952 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/paraver/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2585 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/paraver/__main__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.399231 dataClay-3.0.0a2/src/dataclay/protos/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:33:45.000000 dataClay-3.0.0a2/src/dataclay/protos/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    11086 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/common_messages_pb2.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    18537 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/dataservice_messages_pb2.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     9295 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/dataservice_pb2.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    87821 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/dataservice_pb2_grpc.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    50423 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/logicmodule_messages_pb2.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    15299 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/logicmodule_pb2.py
--rw-rw-r--   0 marc      (1000) marc      (1000)   182431 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/logicmodule_pb2_grpc.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5800 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/metadata_service_pb2.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    21056 2023-02-01 16:42:01.000000 dataClay-3.0.0a2/src/dataclay/protos/metadata_service_pb2_grpc.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    21780 2023-02-01 17:05:05.000000 dataClay-3.0.0a2/src/dataclay/runtime.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.399231 dataClay-3.0.0a2/src/dataclay/util/
--rw-rw-r--   0 marc      (1000) marc      (1000)      546 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/ConfigurationFlags.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      830 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/Constants.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1836 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/DataClayObjectMetaData.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4482 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/FileUtils.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      833 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/IdentityDict.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5283 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/Initializer.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1318 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/MemoryUtils.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    19808 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/MgrObject.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2487 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/PropertiesFilesLoader.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3351 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/ReferenceCounting.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4435 2022-12-23 15:51:12.000000 dataClay-3.0.0a2/src/dataclay/util/StubUtils.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      263 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/YamlIgnores.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5869 2022-12-23 15:51:12.000000 dataClay-3.0.0a2/src/dataclay/util/YamlParser.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5035 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.399231 dataClay-3.0.0a2/src/dataclay/util/classloaders/
--rw-rw-r--   0 marc      (1000) marc      (1000)     3155 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/classloaders/ClassLoader.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/classloaders/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.399231 dataClay-3.0.0a2/src/dataclay/util/ids/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/ids/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      771 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/ids/_uuid.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.399231 dataClay-3.0.0a2/src/dataclay/util/info/
--rw-rw-r--   0 marc      (1000) marc      (1000)      240 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/info/VersionInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/info/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      807 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/logs.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.399231 dataClay-3.0.0a2/src/dataclay/util/management/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.403231 dataClay-3.0.0a2/src/dataclay/util/management/accountmgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      206 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/accountmgr/Account.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      179 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/accountmgr/PasswordCredential.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/accountmgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.403231 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      347 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/AccessedImplementation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      304 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/AccessedProperty.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      628 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Implementation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      162 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/LanguageDependantClassInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      166 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/LanguageDependantOperationInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      165 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/LanguageDependantPropertyInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      161 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/LanguageDependantTypeInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5420 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/MetaClass.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      601 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Operation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      761 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Property.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      668 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/PythonTypeSignatures.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4089 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Type.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      206 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/UserType.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2219 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Utils.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.403231 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/java/
--rw-rw-r--   0 marc      (1000) marc      (1000)      795 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/java/JavaImplementation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/java/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.403231 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/python/
--rw-rw-r--   0 marc      (1000) marc      (1000)      214 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/python/PythonClassInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      166 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/python/PythonImplementation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/classmgr/python/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.403231 dataClay-3.0.0a2/src/dataclay/util/management/contractmgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      444 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/contractmgr/Contract.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      326 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/contractmgr/InterfaceInContract.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      350 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/contractmgr/OpImplementations.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/contractmgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.403231 dataClay-3.0.0a2/src/dataclay/util/management/datacontractmgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      392 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/datacontractmgr/DataContract.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/datacontractmgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.407231 dataClay-3.0.0a2/src/dataclay/util/management/datasetmgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      224 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/datasetmgr/DataSet.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/datasetmgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.407231 dataClay-3.0.0a2/src/dataclay/util/management/interfacemgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      523 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/interfacemgr/Interface.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/interfacemgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.407231 dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/
--rw-rw-r--   0 marc      (1000) marc      (1000)      203 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/DataClayInstance.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      434 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/ExecutionEnvironment.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      654 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/MetaDataInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      301 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/RegistrationInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      185 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/StorageLocation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.407231 dataClay-3.0.0a2/src/dataclay/util/management/namespacemgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      324 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/namespacemgr/Namespace.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/namespacemgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.407231 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/
--rw-rw-r--   0 marc      (1000) marc      (1000)      248 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/SessionContract.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      256 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/SessionDataContract.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      279 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/SessionImplementation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      439 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/SessionInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      336 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/SessionInterface.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      298 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/SessionOperation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      219 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/SessionProperty.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/sessionmgr/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.407231 dataClay-3.0.0a2/src/dataclay/util/management/stubs/
--rw-rw-r--   0 marc      (1000) marc      (1000)      639 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/stubs/ImplementationStubInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      527 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/stubs/PropertyStubInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      555 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/stubs/StubInfo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/management/stubs/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/src/dataclay/util/properties/
--rw-rw-r--   0 marc      (1000) marc      (1000)      391 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)       87 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/checkedtype.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)    10628 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/errorcodes.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)       77 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/event_condition.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)       35 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/event_state.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)       58 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/event_type.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)     4509 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/installedclasses.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/langcodes.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)     5618 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/method_ids.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)      561 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/python_type_signatures.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)       96 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/testflags.properties
--rw-rw-r--   0 marc      (1000) marc      (1000)      359 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/properties/typemodifiers.properties
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/src/dataclay/util/tools/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/tools/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/src/dataclay/util/tools/python/
--rw-rw-r--   0 marc      (1000) marc      (1000)     3723 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/tools/python/PythonMetaClassFactory.py
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/util/tools/python/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/src/dataclay/utils/
--rw-rw-r--   0 marc      (1000) marc      (1000)      401 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/utils/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      364 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/utils/decorators.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      782 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/utils/json.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1953 2023-01-31 13:32:26.000000 dataClay-3.0.0a2/src/dataclay/utils/pickle.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      438 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/dataclay/utils/tracing.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/src/storage/
--rw-rw-r--   0 marc      (1000) marc      (1000)      289 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/storage/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     6481 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/storage/api.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-02-23 12:17:20.411231 dataClay-3.0.0a2/src/storage/models/
--rw-rw-r--   0 marc      (1000) marc      (1000)      396 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/storage/models/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2474 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/storage/models/storagedict.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1638 2022-12-23 15:24:36.000000 dataClay-3.0.0a2/src/storage/models/storagelist.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1529 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/LICENSE.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)       25 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/MANIFEST.in
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2522 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1495 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1000)      263 2022-12-23 16:56:00.000000 dataClay-3.0.0a3/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1236 2023-03-06 12:54:35.015586 dataClay-3.0.0a3/setup.cfg
+-rw-rw-r--   0 marc      (1000) marc      (1000)       69 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/setup.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.983586 dataClay-3.0.0a3/src/
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.987587 dataClay-3.0.0a3/src/dataClay.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2522 2023-03-06 12:54:34.000000 dataClay-3.0.0a3/src/dataClay.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6739 2023-03-06 12:54:34.000000 dataClay-3.0.0a3/src/dataClay.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        1 2023-03-06 12:54:34.000000 dataClay-3.0.0a3/src/dataClay.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)      124 2023-03-06 12:54:34.000000 dataClay-3.0.0a3/src/dataClay.egg-info/requires.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)       17 2023-03-06 12:54:34.000000 dataClay-3.0.0a3/src/dataClay.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.987587 dataClay-3.0.0a3/src/dataclay/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      260 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.987587 dataClay-3.0.0a3/src/dataclay/backend/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/backend/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      186 2023-01-16 16:24:49.000000 dataClay-3.0.0a3/src/dataclay/backend/__main__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    42257 2023-03-01 16:49:51.000000 dataClay-3.0.0a3/src/dataclay/backend/api.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    18683 2023-02-01 17:07:16.000000 dataClay-3.0.0a3/src/dataclay/backend/client.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7436 2023-01-17 14:49:03.000000 dataClay-3.0.0a3/src/dataclay/backend/heapmanager.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    14319 2023-01-31 14:05:38.000000 dataClay-3.0.0a3/src/dataclay/backend/runtime.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    17417 2023-02-17 10:36:39.000000 dataClay-3.0.0a3/src/dataclay/backend/servicer.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.987587 dataClay-3.0.0a3/src/dataclay/client/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/client/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5798 2023-02-27 15:43:08.000000 dataClay-3.0.0a3/src/dataclay/client/api.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7544 2023-02-27 15:43:08.000000 dataClay-3.0.0a3/src/dataclay/client/runtime.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.987587 dataClay-3.0.0a3/src/dataclay/conf/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5568 2023-02-17 10:36:38.000000 dataClay-3.0.0a3/src/dataclay/conf/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.991587 dataClay-3.0.0a3/src/dataclay/contrib/
+-rw-rw-r--   0 marc      (1000) marc      (1000)       89 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7335 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/collections.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.991587 dataClay-3.0.0a3/src/dataclay/contrib/dataclay_dummy/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      997 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/dataclay_dummy/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      947 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/dummy_pycompss.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1340 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/kafka.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1520 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/mqtt.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    11787 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/splitting.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      551 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/contrib/synchronization.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    18262 2023-02-27 18:32:57.000000 dataClay-3.0.0a3/src/dataclay/dataclay_object.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.991587 dataClay-3.0.0a3/src/dataclay/exceptions/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      756 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/exceptions/ErrorDefs.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)       45 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/exceptions/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6205 2023-02-01 17:07:47.000000 dataClay-3.0.0a3/src/dataclay/exceptions/exceptions.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.991587 dataClay-3.0.0a3/src/dataclay/metadata/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/metadata/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1974 2023-02-17 10:36:39.000000 dataClay-3.0.0a3/src/dataclay/metadata/__main__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    10484 2023-02-27 18:19:09.000000 dataClay-3.0.0a3/src/dataclay/metadata/api.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3259 2022-12-29 12:23:20.000000 dataClay-3.0.0a3/src/dataclay/metadata/cli.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4798 2023-02-15 14:14:44.000000 dataClay-3.0.0a3/src/dataclay/metadata/client.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5272 2023-02-23 11:18:12.000000 dataClay-3.0.0a3/src/dataclay/metadata/kvdata.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2357 2023-01-16 13:59:40.000000 dataClay-3.0.0a3/src/dataclay/metadata/redismanager.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5895 2023-01-31 14:17:42.000000 dataClay-3.0.0a3/src/dataclay/metadata/servicer.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.991587 dataClay-3.0.0a3/src/dataclay/paraver/
+-rw-rw-r--   0 marc      (1000) marc      (1000)    14952 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/paraver/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2585 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/paraver/__main__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.995586 dataClay-3.0.0a3/src/dataclay/protos/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:33:45.000000 dataClay-3.0.0a3/src/dataclay/protos/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    11086 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/common_messages_pb2.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    18537 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/dataservice_messages_pb2.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     9295 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/dataservice_pb2.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    87821 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/dataservice_pb2_grpc.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    50423 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/logicmodule_messages_pb2.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    15299 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/logicmodule_pb2.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)   182431 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/logicmodule_pb2_grpc.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5800 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/metadata_service_pb2.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    21056 2023-02-01 16:42:01.000000 dataClay-3.0.0a3/src/dataclay/protos/metadata_service_pb2_grpc.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    21780 2023-02-01 17:05:05.000000 dataClay-3.0.0a3/src/dataclay/runtime.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.995586 dataClay-3.0.0a3/src/dataclay/util/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      546 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/ConfigurationFlags.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      830 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/Constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1836 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/DataClayObjectMetaData.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4482 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/FileUtils.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      833 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/IdentityDict.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5283 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/Initializer.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1318 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/MemoryUtils.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    19808 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/MgrObject.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2487 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/PropertiesFilesLoader.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3351 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/ReferenceCounting.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4435 2022-12-23 15:51:12.000000 dataClay-3.0.0a3/src/dataclay/util/StubUtils.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      263 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/YamlIgnores.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5869 2022-12-23 15:51:12.000000 dataClay-3.0.0a3/src/dataclay/util/YamlParser.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5035 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.995586 dataClay-3.0.0a3/src/dataclay/util/classloaders/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3155 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/classloaders/ClassLoader.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/classloaders/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.995586 dataClay-3.0.0a3/src/dataclay/util/ids/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/ids/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      771 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/ids/_uuid.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.995586 dataClay-3.0.0a3/src/dataclay/util/info/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      240 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/info/VersionInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/info/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      807 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/logs.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.995586 dataClay-3.0.0a3/src/dataclay/util/management/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.995586 dataClay-3.0.0a3/src/dataclay/util/management/accountmgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      206 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/accountmgr/Account.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      179 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/accountmgr/PasswordCredential.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/accountmgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      347 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/AccessedImplementation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      304 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/AccessedProperty.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      628 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Implementation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      162 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/LanguageDependantClassInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      166 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/LanguageDependantOperationInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      165 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/LanguageDependantPropertyInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      161 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/LanguageDependantTypeInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5420 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/MetaClass.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      601 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Operation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      761 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Property.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      668 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/PythonTypeSignatures.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4089 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Type.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      206 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/UserType.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2219 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Utils.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/java/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      795 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/java/JavaImplementation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/java/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/python/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      214 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/python/PythonClassInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      166 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/python/PythonImplementation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/classmgr/python/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/contractmgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      444 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/contractmgr/Contract.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      326 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/contractmgr/InterfaceInContract.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      350 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/contractmgr/OpImplementations.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/contractmgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/datacontractmgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      392 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/datacontractmgr/DataContract.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/datacontractmgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/datasetmgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      224 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/datasetmgr/DataSet.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/datasetmgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/interfacemgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      523 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/interfacemgr/Interface.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/interfacemgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      203 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/DataClayInstance.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      434 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/ExecutionEnvironment.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      654 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/MetaDataInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      301 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/RegistrationInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      185 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/StorageLocation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:34.999586 dataClay-3.0.0a3/src/dataclay/util/management/namespacemgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      324 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/namespacemgr/Namespace.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/namespacemgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.003586 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      248 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/SessionContract.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      256 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/SessionDataContract.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      279 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/SessionImplementation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      439 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/SessionInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      336 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/SessionInterface.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      298 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/SessionOperation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      219 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/SessionProperty.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/sessionmgr/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.003586 dataClay-3.0.0a3/src/dataclay/util/management/stubs/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      639 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/stubs/ImplementationStubInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      527 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/stubs/PropertyStubInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      555 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/stubs/StubInfo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/management/stubs/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/src/dataclay/util/properties/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      391 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)       87 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/checkedtype.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)    10628 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/errorcodes.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)       77 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/event_condition.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)       35 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/event_state.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)       58 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/event_type.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4509 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/installedclasses.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/langcodes.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5618 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/method_ids.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)      561 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/python_type_signatures.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)       96 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/testflags.properties
+-rw-rw-r--   0 marc      (1000) marc      (1000)      359 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/properties/typemodifiers.properties
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/src/dataclay/util/tools/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/tools/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/src/dataclay/util/tools/python/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3723 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/tools/python/PythonMetaClassFactory.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/util/tools/python/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/src/dataclay/utils/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      401 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/utils/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      364 2023-02-28 17:07:11.000000 dataClay-3.0.0a3/src/dataclay/utils/decorators.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      782 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/dataclay/utils/json.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1953 2023-01-31 13:32:26.000000 dataClay-3.0.0a3/src/dataclay/utils/pickle.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      897 2023-02-28 17:08:24.000000 dataClay-3.0.0a3/src/dataclay/utils/tracing.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/src/storage/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      289 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/storage/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6481 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/storage/api.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-03-06 12:54:35.011587 dataClay-3.0.0a3/src/storage/models/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      396 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/storage/models/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2474 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/storage/models/storagedict.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1638 2022-12-23 15:24:36.000000 dataClay-3.0.0a3/src/storage/models/storagelist.py
```

### Comparing `dataClay-3.0.0a2/LICENSE.txt` & `dataClay-3.0.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/PKG-INFO` & `dataClay-3.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataClay
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: Python library for dataClay
 Home-page: https://www.bsc.es/dataclay
 License: BSD License
 Project-URL: Documentation, https://pyclay.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/bsc-dom/pyclay
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mn4
+Provides-Extra: opentelemetry
 License-File: LICENSE.txt
 
 [![Tests](https://github.com/bsc-dom/pyclay/actions/workflows/tests.yml/badge.svg)](https://github.com/bsc-dom/pyclay/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyclay/badge/?version=latest)](https://pyclay.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Status](https://img.shields.io/pypi/status/dataclay)
 ![PyPI - Format](https://img.shields.io/pypi/format/dataclay)
 [![License](https://img.shields.io/github/license/bsc-dom/pyclay)](https://github.com/bsc-dom/pyclay/blob/main/LICENSE.txt)
```

### Comparing `dataClay-3.0.0a2/README.md` & `dataClay-3.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/setup.cfg` & `dataClay-3.0.0a3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dataClay
-version = 3.0.0-alpha.2
+version = 3.0.0-alpha.3
 description = Python library for dataClay
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.bsc.es/dataclay
 project_urls = 
 	Documentation = https://pyclay.readthedocs.io/en/latest/
 	Source = https://github.com/bsc-dom/pyclay
@@ -31,24 +31,25 @@
 install_requires = 
 	grpcio
 	numpy
 	psutil
 	protobuf
 	redis
 	bcrypt
-	opentelemetry-api
 include_package_data = True
 
 [options.extras_require]
 dev = 
 	grpcio-tools
 	black
 	isort
 mn4 = 
 	ansible
+opentelemetry = 
+	opentelemetry-api
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.properties
```

### Comparing `dataClay-3.0.0a2/src/dataClay.egg-info/PKG-INFO` & `dataClay-3.0.0a3/src/dataClay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataClay
-Version: 3.0.0a2
+Version: 3.0.0a3
 Summary: Python library for dataClay
 Home-page: https://www.bsc.es/dataclay
 License: BSD License
 Project-URL: Documentation, https://pyclay.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/bsc-dom/pyclay
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mn4
+Provides-Extra: opentelemetry
 License-File: LICENSE.txt
 
 [![Tests](https://github.com/bsc-dom/pyclay/actions/workflows/tests.yml/badge.svg)](https://github.com/bsc-dom/pyclay/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/pyclay/badge/?version=latest)](https://pyclay.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Status](https://img.shields.io/pypi/status/dataclay)
 ![PyPI - Format](https://img.shields.io/pypi/format/dataclay)
 [![License](https://img.shields.io/github/license/bsc-dom/pyclay)](https://github.com/bsc-dom/pyclay/blob/main/LICENSE.txt)
```

### Comparing `dataClay-3.0.0a2/src/dataClay.egg-info/SOURCES.txt` & `dataClay-3.0.0a3/src/dataClay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/backend/api.py` & `dataClay-3.0.0a3/src/dataclay/backend/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,37 +6,34 @@
 import logging
 import pickle
 import time
 import traceback
 import uuid
 from typing import TYPE_CHECKING
 
-from opentelemetry import trace
-
 from dataclay import utils
 from dataclay.backend.client import BackendClient
 from dataclay.backend.runtime import BackendRuntime
 from dataclay.conf import settings
 from dataclay.exceptions import *
 from dataclay.runtime import UUIDLock, set_runtime
 from dataclay.utils.pickle import RecursiveLocalPickler, RecursiveLocalUnpickler
+from dataclay.utils.tracing import trace
 
 if TYPE_CHECKING:
-
     from dataclay.dataclay_object import DataClayObject
 
 
 logging.basicConfig(level=logging.DEBUG)
 tracer = trace.get_tracer(__name__)
 logger = utils.LoggerEvent(logging.getLogger(__name__))
 
 
 class BackendAPI:
     def __init__(self, name, port, kv_host, kv_port):
-
         # NOTE: the port is (atm) exclusively for unique identification of an EE
         # (given that the name is shared between all EE that share a SL, which happens in HPC deployments)
         self.name = name
         self.port = port
 
         # Initialize runtime
         self.runtime = BackendRuntime(kv_host, kv_port)
@@ -46,15 +43,14 @@
         self.backend_id = settings.DATACLAY_BACKEND_ID
         logger.info(f"Initialized Backend with ID: {self.backend_id}")
 
     def is_ready(self, timeout=None, pause=0.5):
         ref = time.time()
         now = ref
         if self.runtime.metadata_service.is_ready(timeout):
-
             # Check that dataclay_id is defined. If it is not defined, it could break things
             while timeout is None or (now - ref) < timeout:
                 try:
                     dataclay_id = self.runtime.metadata_service.get_dataclay("this").id
                     settings.DATACLAY_ID = dataclay_id
                     return True
                 except DoesNotExistError:
@@ -505,15 +501,14 @@
                 try:
                     instance.when_unfederated()
                 except:
                     # ignore if method is not implemented
                     pass
                 instance.set_origin_location(None)
                 try:
-
                     if instance._dc_alias is not None and instance._dc_alias != "":
                         logger.debug(f"Removing alias {instance._dc_alias}")
                         self.self.runtime.delete_alias(instance)
 
                 except Exception as ex:
                     traceback.print_exc()
                     logger.debug(
@@ -731,17 +726,15 @@
             except KeyError:
                 objects_in_backend = set()
                 objects_per_backend[hint] = objects_in_backend
             objects_in_backend.add(object_id)
 
         # Now Call
         for backend_id, objects_to_get in objects_per_backend.items():
-
             if dest_replica_backend_id is None or dest_replica_backend_id != backend_id:
-
                 logger.debug(
                     "[==GetObjectsInOtherBackend==] Get from other location, objects: %s",
                     objects_to_get,
                 )
                 backend = self.runtime.ee_infos[backend_id]
                 try:
                     client_backend = self.runtime.backend_clients[backend_id]
@@ -943,29 +936,27 @@
         Returns:
             ID of objects and for each object, its bytes.
         """
         raise Exception("To refactor")
         # Prepare to unify calls (only one call for DS)
         objects_per_backend = dict()
         for curr_obj_with_ids in objects_in_other_backends:
-
             object_id = curr_obj_with_ids[0]
             object_md = self.get_object_metadata(object_id)
             location = object_md.backend_id
             # Update object at first location (NOT UPDATING REPLICAS!!!)
             try:
                 objects_in_backend = objects_per_backend[location]
             except KeyError:
                 objects_in_backend = list()
                 objects_per_backend[location] = objects_in_backend
 
             objects_in_backend.append(curr_obj_with_ids)
         # Now Call
         for backend_id, objects_to_update in objects_per_backend.items():
-
             backend = self.runtime.get_execution_environment_info(backend_id)
 
             try:
                 client_backend = self.runtime.backend_clients[backend_id]
             except KeyError:
                 logger.debug(
                     "[==GetObjectsInOtherBackend==] Not found Client to ExecutionEnvironment {%s}!"
```

### Comparing `dataClay-3.0.0a2/src/dataclay/backend/client.py` & `dataClay-3.0.0a3/src/dataclay/backend/client.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/backend/heapmanager.py` & `dataClay-3.0.0a3/src/dataclay/backend/heapmanager.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/backend/runtime.py` & `dataClay-3.0.0a3/src/dataclay/backend/runtime.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/backend/servicer.py` & `dataClay-3.0.0a3/src/dataclay/backend/servicer.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/client/api.py` & `dataClay-3.0.0a3/src/dataclay/client/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 """
 
 __all__ = ["init", "finish", "DataClayObject"]
 
 import logging
 import logging.config
 
-from opentelemetry import trace
-
 from dataclay.client.runtime import UNDEFINED_LOCAL as _UNDEFINED_LOCAL
 from dataclay.client.runtime import ClientRuntime
 from dataclay.conf import settings
 from dataclay.dataclay_object import DataClayObject
 from dataclay.runtime import get_runtime, set_runtime
+from dataclay.utils.tracing import trace
 
 # This will be populated during initialization
 LOCAL = _UNDEFINED_LOCAL
 
 tracer = trace.get_tracer(__name__)
 logger = logging.getLogger(__name__)
```

### Comparing `dataClay-3.0.0a2/src/dataclay/client/runtime.py` & `dataClay-3.0.0a3/src/dataclay/client/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """ ClientRuntime """
 
 import io
 import logging
 import random
 import traceback
 
-from opentelemetry import trace
-
 from dataclay.dataclay_object import DataClayObject
 from dataclay.metadata.client import MetadataClient
 from dataclay.runtime import DataClayRuntime
 from dataclay.utils.pickle import RecursiveLocalPickler
+from dataclay.utils.tracing import trace
 
 UNDEFINED_LOCAL = object()
 
 tracer = trace.get_tracer(__name__)
 logger = logging.getLogger(__name__)
```

### Comparing `dataClay-3.0.0a2/src/dataclay/conf/__init__.py` & `dataClay-3.0.0a3/src/dataclay/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/contrib/collections.py` & `dataClay-3.0.0a3/src/dataclay/contrib/collections.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/contrib/dataclay_dummy/__init__.py` & `dataClay-3.0.0a3/src/dataclay/contrib/dataclay_dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/contrib/dummy_pycompss.py` & `dataClay-3.0.0a3/src/dataclay/contrib/dummy_pycompss.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/contrib/kafka.py` & `dataClay-3.0.0a3/src/dataclay/contrib/kafka.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/contrib/mqtt.py` & `dataClay-3.0.0a3/src/dataclay/contrib/mqtt.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/contrib/splitting.py` & `dataClay-3.0.0a3/src/dataclay/contrib/splitting.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/contrib/synchronization.py` & `dataClay-3.0.0a3/src/dataclay/contrib/synchronization.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/dataclay_object.py` & `dataClay-3.0.0a3/src/dataclay/dataclay_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 import threading
 import traceback
 import uuid
 from collections import ChainMap
 from inspect import get_annotations
 from uuid import UUID
 
-from opentelemetry import trace
-
 from dataclay.exceptions import *
 from dataclay.metadata.kvdata import ObjectMetadata
 from dataclay.protos.common_messages_pb2 import LANG_PYTHON
 from dataclay.runtime import get_runtime
+from dataclay.utils.tracing import trace
 
 DC_PROPERTY_PREFIX = "_dc_property_"
 
 
 tracer = trace.get_tracer(__name__)
 logger = logging.getLogger(__name__)
 
@@ -93,15 +92,14 @@
             raise
 
     # wrapper_activemethod.is_activemethod = True
     return wrapper_activemethod
 
 
 class DataClayProperty:
-
     __slots__ = "property_name", "dc_property_name"
 
     def __init__(self, property_name):
         self.property_name = property_name
         self.dc_property_name = DC_PROPERTY_PREFIX + property_name
 
     def __get__(self, instance: DataClayObject, owner):
@@ -264,25 +262,19 @@
             k: v for k, v in vars(self).items() if not k.startswith(DC_PROPERTY_PREFIX)
         }
 
     ###########################
     # Object Oriented Methods #
     ###########################
 
+    @tracer.start_as_current_span("make_persistent")
     def make_persistent(self, alias=None, backend_id=None, recursive=True):
-
-        with tracer.start_as_current_span(
-            "make_persistent",
-            attributes={"alias": str(alias), "backend_id": str(backend_id), "recursive": recursive},
-        ):
-            if alias == "":
-                raise AttributeError("Alias cannot be empty")
-            get_runtime().make_persistent(
-                self, alias=alias, backend_id=backend_id, recursive=recursive
-            )
+        if alias == "":
+            raise AttributeError("Alias cannot be empty")
+        get_runtime().make_persistent(self, alias=alias, backend_id=backend_id, recursive=recursive)
 
     @classmethod
     def get_by_id(cls, object_id: UUID):
         return get_runtime().get_object_by_id(object_id)
 
     @classmethod
     def get_by_alias(cls, alias, dataset_name=None):
@@ -352,15 +344,14 @@
             <objectID>:<backendID|empty>:<classID>
 
         In which all ID are UUID and the "hint" (backendID) can be empty.
 
         If the object is NOT persistent, then this method returns None.
         """
         if self._dc_is_registered:
-
             return "%s:%s:%s" % (
                 self._dc_id,
                 self._dc_backend_id,
                 self._dc_class_name,
             )
         else:
             return None
@@ -497,15 +488,14 @@
         if not self._dc_is_registered:
             logger.debug("Pickling of object is causing a make_persistent")
             self.make_persistent()
 
         return self.get_by_id, (self._dc_id,)
 
     def __repr__(self):
-
         if self._dc_is_registered:
             return "<%s instance with ObjectID=%s>" % (
                 self._dc_class_name,
                 self._dc_id,
             )
         else:
             return "<%s volatile instance with ObjectID=%s>" % (
```

### Comparing `dataClay-3.0.0a2/src/dataclay/exceptions/ErrorDefs.py` & `dataClay-3.0.0a3/src/dataclay/exceptions/ErrorDefs.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/exceptions/exceptions.py` & `dataClay-3.0.0a3/src/dataclay/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/metadata/__main__.py` & `dataClay-3.0.0a3/src/dataclay/metadata/__main__.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/metadata/api.py` & `dataClay-3.0.0a3/src/dataclay/metadata/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import logging
 import uuid
 from uuid import UUID
 
-from opentelemetry import trace
-
 from dataclay.exceptions.exceptions import *
 from dataclay.metadata.kvdata import (
     Account,
     Alias,
     Backend,
     Dataclay,
     Dataset,
     ObjectMetadata,
     Session,
 )
 from dataclay.metadata.redismanager import RedisManager
+from dataclay.utils.tracing import trace
 
 FEDERATOR_ACCOUNT_USERNAME = "Federator"
 EXTERNAL_OBJECTS_DATASET_NAME = "ExternalObjects"
 
 
 # Acquire a tracer and logger
 tracer = trace.get_tracer(__name__)
 logger = logging.getLogger(__name__)
 
 
 class MetadataAPI:
     def __init__(self, kv_host, kv_port):
-
         self.kv_manager = RedisManager(kv_host, kv_port)
 
         logger.info("Initialized MetadataService")
 
     def is_ready(self, timeout=None, pause=0.5):
         return self.kv_manager.is_ready(timeout=timeout, pause=pause)
 
@@ -110,32 +108,31 @@
         # Put new dataset and account to etcd
         # Order matters to check that dataset name is not registered
         self.kv_manager.set_new(dataset)
         self.kv_manager.set_new(account)
 
         logger.info(f"Created new account for {username} with dataset {dataset.name}")
 
+    @tracer.start_as_current_span("new_account")
     def new_account(self, username: str, password: str):
         """Registers a new account
 
         Creates a new account. Checks that the username is not registered.
 
         Args:
             username : Accounts username
             password : Accounts password
         """
-        with tracer.start_as_current_span("new_account", attributes={"username": username}):
+        # TODO: Ask for admin credentials for creating the account.
 
-            # TODO: Ask for admin credentials for creating the account.
-
-            # Creates new account and put it to etcd
-            account = Account.new(username, password)
-            self.kv_manager.set_new(account)
+        # Creates new account and put it to etcd
+        account = Account.new(username, password)
+        self.kv_manager.set_new(account)
 
-            logger.info(f"Created new account for {username}")
+        logger.info(f"Created new account for {username}")
 
     ###########
     # Dataset #
     ###########
 
     @tracer.start_as_current_span("new_dataset")
     def new_dataset(self, username: str, password: str, dataset_name: str):
@@ -153,15 +150,14 @@
 
         Raises:
             Exception('Account is not valid!'): If wrong credentials
         """
 
         # Lock to update account.datasets without race condition
         with self.kv_manager.lock(Account.path + username):
-
             # Validates account credentials
             account = self.kv_manager.get_kv(Account, username)
             if not account.verify(password):
                 raise AccountInvalidCredentialsError(username)
 
             # Creates new dataset and updates account's list of datasets
             dataset = Dataset(dataset_name, username)
@@ -218,15 +214,15 @@
 
         # NOTE: If a session can just access one dataset, then this
         # dataset will always be the session's default dataset.
         # object_md.dataset_name = session.dataset_name
 
         self.kv_manager.set(object_md)
 
-    @tracer.start_as_current_span("start_as_current_span")
+    @tracer.start_as_current_span("get_object_md_by_id")
     def get_object_md_by_id(self, object_id: UUID, session_id=None, check_session=False):
         if check_session:
             session = self.kv_manager.get_kv(Session, session_id)
             if not session.is_active:
                 raise SessionIsNotActiveError(session_id)
 
         object_md = self.kv_manager.get_kv(ObjectMetadata, object_id)
@@ -266,15 +262,14 @@
         alias = Alias(alias_name, dataset_name, object_id)
         self.kv_manager.set_new(alias)
 
     @tracer.start_as_current_span("delete_alias")
     def delete_alias(
         self, alias_name: str, dataset_name: str, session_id: UUID, check_session=False
     ):
-
         # NOTE: If the session is not checked, we supose the dataset_name is correct
         #       since only the EE is able to set check_session to False
         if check_session:
             # Checks that session exist and is active
             session = self.kv_manager.get_kv(Session, session_id)
             if not session.is_active:
                 raise SessionIsNotActiveError(session_id)
```

### Comparing `dataClay-3.0.0a2/src/dataclay/metadata/cli.py` & `dataClay-3.0.0a3/src/dataclay/metadata/cli.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/metadata/client.py` & `dataClay-3.0.0a3/src/dataclay/metadata/client.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/metadata/kvdata.py` & `dataClay-3.0.0a3/src/dataclay/metadata/kvdata.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/metadata/redismanager.py` & `dataClay-3.0.0a3/src/dataclay/metadata/redismanager.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/metadata/servicer.py` & `dataClay-3.0.0a3/src/dataclay/metadata/servicer.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/paraver/__init__.py` & `dataClay-3.0.0a3/src/dataclay/paraver/__init__.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/paraver/__main__.py` & `dataClay-3.0.0a3/src/dataclay/paraver/__main__.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/common_messages_pb2.py` & `dataClay-3.0.0a3/src/dataclay/protos/common_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/dataservice_messages_pb2.py` & `dataClay-3.0.0a3/src/dataclay/protos/dataservice_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/dataservice_pb2.py` & `dataClay-3.0.0a3/src/dataclay/protos/dataservice_pb2.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/dataservice_pb2_grpc.py` & `dataClay-3.0.0a3/src/dataclay/protos/dataservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/logicmodule_messages_pb2.py` & `dataClay-3.0.0a3/src/dataclay/protos/logicmodule_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/logicmodule_pb2.py` & `dataClay-3.0.0a3/src/dataclay/protos/logicmodule_pb2.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/logicmodule_pb2_grpc.py` & `dataClay-3.0.0a3/src/dataclay/protos/logicmodule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/metadata_service_pb2.py` & `dataClay-3.0.0a3/src/dataclay/protos/metadata_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/protos/metadata_service_pb2_grpc.py` & `dataClay-3.0.0a3/src/dataclay/protos/metadata_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/runtime.py` & `dataClay-3.0.0a3/src/dataclay/runtime.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/ConfigurationFlags.py` & `dataClay-3.0.0a3/src/dataclay/util/ConfigurationFlags.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/Constants.py` & `dataClay-3.0.0a3/src/dataclay/util/Constants.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/DataClayObjectMetaData.py` & `dataClay-3.0.0a3/src/dataclay/util/DataClayObjectMetaData.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/FileUtils.py` & `dataClay-3.0.0a3/src/dataclay/util/FileUtils.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/IdentityDict.py` & `dataClay-3.0.0a3/src/dataclay/util/IdentityDict.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/Initializer.py` & `dataClay-3.0.0a3/src/dataclay/util/Initializer.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/MemoryUtils.py` & `dataClay-3.0.0a3/src/dataclay/util/MemoryUtils.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/MgrObject.py` & `dataClay-3.0.0a3/src/dataclay/util/MgrObject.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/PropertiesFilesLoader.py` & `dataClay-3.0.0a3/src/dataclay/util/PropertiesFilesLoader.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/ReferenceCounting.py` & `dataClay-3.0.0a3/src/dataclay/util/ReferenceCounting.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/StubUtils.py` & `dataClay-3.0.0a3/src/dataclay/util/StubUtils.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/YamlParser.py` & `dataClay-3.0.0a3/src/dataclay/util/YamlParser.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/__init__.py` & `dataClay-3.0.0a3/src/dataclay/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/classloaders/ClassLoader.py` & `dataClay-3.0.0a3/src/dataclay/util/classloaders/ClassLoader.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/ids/_uuid.py` & `dataClay-3.0.0a3/src/dataclay/util/ids/_uuid.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/logs.py` & `dataClay-3.0.0a3/src/dataclay/util/logs.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Implementation.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Implementation.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/MetaClass.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/MetaClass.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Operation.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Operation.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Property.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Property.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/PythonTypeSignatures.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/PythonTypeSignatures.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Type.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Type.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/Utils.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/Utils.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/classmgr/java/JavaImplementation.py` & `dataClay-3.0.0a3/src/dataclay/util/management/classmgr/java/JavaImplementation.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/interfacemgr/Interface.py` & `dataClay-3.0.0a3/src/dataclay/util/management/interfacemgr/Interface.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/metadataservice/MetaDataInfo.py` & `dataClay-3.0.0a3/src/dataclay/util/management/metadataservice/MetaDataInfo.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/stubs/ImplementationStubInfo.py` & `dataClay-3.0.0a3/src/dataclay/util/management/stubs/ImplementationStubInfo.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/stubs/PropertyStubInfo.py` & `dataClay-3.0.0a3/src/dataclay/util/management/stubs/PropertyStubInfo.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/management/stubs/StubInfo.py` & `dataClay-3.0.0a3/src/dataclay/util/management/stubs/StubInfo.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/properties/errorcodes.properties` & `dataClay-3.0.0a3/src/dataclay/util/properties/errorcodes.properties`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/properties/installedclasses.properties` & `dataClay-3.0.0a3/src/dataclay/util/properties/installedclasses.properties`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/properties/method_ids.properties` & `dataClay-3.0.0a3/src/dataclay/util/properties/method_ids.properties`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/properties/python_type_signatures.properties` & `dataClay-3.0.0a3/src/dataclay/util/properties/python_type_signatures.properties`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/util/tools/python/PythonMetaClassFactory.py` & `dataClay-3.0.0a3/src/dataclay/util/tools/python/PythonMetaClassFactory.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/utils/json.py` & `dataClay-3.0.0a3/src/dataclay/utils/json.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/dataclay/utils/pickle.py` & `dataClay-3.0.0a3/src/dataclay/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/storage/api.py` & `dataClay-3.0.0a3/src/storage/api.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/storage/models/storagedict.py` & `dataClay-3.0.0a3/src/storage/models/storagedict.py`

 * *Files identical despite different names*

### Comparing `dataClay-3.0.0a2/src/storage/models/storagelist.py` & `dataClay-3.0.0a3/src/storage/models/storagelist.py`

 * *Files identical despite different names*

