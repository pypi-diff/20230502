# Comparing `tmp/BDXConverter-1.0.10.tar.gz` & `tmp/BDXConverter-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.10.tar", last modified: Tue May  2 10:26:42 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.11.tar", last modified: Tue May  2 21:02:07 2023, max compression
```

## Comparing `BDXConverter-1.0.10.tar` & `BDXConverter-1.0.11.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:42.542192 BDXConverter-1.0.10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:42.534191 BDXConverter-1.0.10/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:42.538192 BDXConverter-1.0.10/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Converter/ConvertErrorDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:42.538192 BDXConverter-1.0.10/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:42.542192 BDXConverter-1.0.10/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/Terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:42.542192 BDXConverter-1.0.10/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/BDXConverter/utils/unmarshalNBT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:26:42.534191 BDXConverter-1.0.10/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-02 10:26:42.000000 BDXConverter-1.0.10/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-02 10:26:42.000000 BDXConverter-1.0.10/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:26:42.000000 BDXConverter-1.0.10/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 10:26:42.000000 BDXConverter-1.0.10/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 10:26:42.000000 BDXConverter-1.0.10/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-02 10:26:42.542192 BDXConverter-1.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:26:42.542192 BDXConverter-1.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-02 10:26:28.000000 BDXConverter-1.0.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.484086 BDXConverter-1.0.11/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.484086 BDXConverter-1.0.11/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.488086 BDXConverter-1.0.11/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.496086 BDXConverter-1.0.11/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/Terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/unmarshalNBT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.484086 BDXConverter-1.0.11/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/setup.py
```

### Comparing `BDXConverter-1.0.10/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.11/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.11/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.0.11/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/General/Pool.py` & `BDXConverter-1.0.11/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.11/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.0.11/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.0.11/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.11/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.0.11/BDXConverter/utils/unmarshalNBT.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import BytesIO
 from struct import unpack
 from .getByte import getByte
 import nbtlib
-
+import sys
 endian: str = '<'
 
 
 class getValueError(Exception):
     def __init__(self, errorOccurredPosition: int):
         Exception.__init__(
             self, f'failed to parse value, and the error occurred at position {errorOccurredPosition}')
@@ -17,51 +17,90 @@
         Exception.__init__(self, f'unexpected number {value}')
 
 
 def getName(buffer: BytesIO) -> str:
     keyLength = unpack(f'{endian}H', getByte(buffer, 2))[0]
     return getByte(buffer, keyLength).decode(encoding='utf-8')
 
-
-def getValue(buffer: BytesIO, valueType: int) -> nbtlib.tag.Byte | nbtlib.tag.Short | nbtlib.tag.Int | nbtlib.tag.Long | nbtlib.tag.Float | nbtlib.tag.Double | nbtlib.tag.ByteArray | nbtlib.tag.String | nbtlib.tag.List | nbtlib.tag.Compound | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
-    if valueType == 1:
-        return nbtlib.tag.Byte(unpack(f'{endian}b', getByte(buffer, 1))[0])
-    elif valueType == 2:
-        return nbtlib.tag.Short(unpack(f'{endian}h', getByte(buffer, 2))[0])
-    elif valueType == 3:
-        return nbtlib.tag.Int(unpack(f'{endian}i', getByte(buffer, 4))[0])
-    elif valueType == 4:
-        return nbtlib.tag.Long(unpack(f'{endian}q', getByte(buffer, 8))[0])
-    elif valueType == 5:
-        return nbtlib.tag.Float(unpack(f'{endian}f', getByte(buffer, 4))[0])
-    elif valueType == 6:
-        return nbtlib.tag.Double(unpack(f'{endian}d', getByte(buffer, 8))[0])
-    elif valueType == 7 or valueType == 11 or valueType == 12:
-        return getArray(buffer, valueType)
-    elif valueType == 8:
-        return nbtlib.tag.String(getName(buffer))
-    elif valueType == 9:
-        return getList(buffer)
-    elif valueType == 10:
-        return getCompound(buffer)
-    else:
-        raise getValueError(buffer.seek(0, 1))
-
-
-def getArray(buffer: BytesIO, valueType: int) -> nbtlib.tag.ByteArray | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
-    arrayLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
-    if valueType == 7:
-        return nbtlib.tag.ByteArray([unpack(f'{endian}b', getByte(buffer, 1))[0] for _ in range(arrayLength)])
-    elif valueType == 11:
-        return nbtlib.tag.IntArray([unpack(f'{endian}i', getByte(buffer, 4))[0] for _ in range(arrayLength)])
-    elif valueType == 12:
-        return nbtlib.tag.LongArray([unpack(f'{endian}q', getByte(buffer, 8))[0] for _ in range(arrayLength)])
-    else:
-        raise unexpectedError(valueType)
-
+if sys.version_info.major>=3 and sys.version_info.minor>=10:
+    def getValue(buffer: BytesIO, valueType: int) -> nbtlib.tag.Byte | nbtlib.tag.Short | nbtlib.tag.Int | nbtlib.tag.Long | nbtlib.tag.Float | nbtlib.tag.Double | nbtlib.tag.ByteArray | nbtlib.tag.String | nbtlib.tag.List | nbtlib.tag.Compound | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
+        match valueType:
+            case 1:
+                return nbtlib.tag.Byte(unpack(f'{endian}b', getByte(buffer, 1))[0])
+            case 2:
+                return nbtlib.tag.Short(unpack(f'{endian}h', getByte(buffer, 2))[0])
+            case 3:
+                return nbtlib.tag.Int(unpack(f'{endian}i', getByte(buffer, 4))[0])
+            case 4:
+                return nbtlib.tag.Long(unpack(f'{endian}q', getByte(buffer, 8))[0])
+            case 5:
+                return nbtlib.tag.Float(unpack(f'{endian}f', getByte(buffer, 4))[0])
+            case 6:
+                return nbtlib.tag.Double(unpack(f'{endian}d', getByte(buffer, 8))[0])
+            case 7:
+                return getArray(buffer, valueType)
+            case 11:
+                return getArray(buffer, valueType)
+            case 12:
+                return getArray(buffer, valueType)
+            case 8:
+                return nbtlib.tag.String(getName(buffer))
+            case 9:
+                return getList(buffer)
+            case 10:
+                return getCompound(buffer)
+            case _:
+                raise getValueError(buffer.seek(0, 1))
+else:
+    def getValue(buffer: BytesIO, valueType: int) -> nbtlib.tag.Byte | nbtlib.tag.Short | nbtlib.tag.Int | nbtlib.tag.Long | nbtlib.tag.Float | nbtlib.tag.Double | nbtlib.tag.ByteArray | nbtlib.tag.String | nbtlib.tag.List | nbtlib.tag.Compound | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
+        if valueType == 1:
+            return nbtlib.tag.Byte(unpack(f'{endian}b', getByte(buffer, 1))[0])
+        elif valueType == 2:
+            return nbtlib.tag.Short(unpack(f'{endian}h', getByte(buffer, 2))[0])
+        elif valueType == 3:
+            return nbtlib.tag.Int(unpack(f'{endian}i', getByte(buffer, 4))[0])
+        elif valueType == 4:
+            return nbtlib.tag.Long(unpack(f'{endian}q', getByte(buffer, 8))[0])
+        elif valueType == 5:
+            return nbtlib.tag.Float(unpack(f'{endian}f', getByte(buffer, 4))[0])
+        elif valueType == 6:
+            return nbtlib.tag.Double(unpack(f'{endian}d', getByte(buffer, 8))[0])
+        elif valueType == 7 or valueType == 11 or valueType == 12:
+            return getArray(buffer, valueType)
+        elif valueType == 8:
+            return nbtlib.tag.String(getName(buffer))
+        elif valueType == 9:
+            return getList(buffer)
+        elif valueType == 10:
+            return getCompound(buffer)
+        else:
+            raise getValueError(buffer.seek(0, 1))
+if sys.version_info.major>=3 and sys.version_info.minor>=10:
+    def getArray(buffer: BytesIO, valueType: int) -> nbtlib.tag.ByteArray | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
+        arrayLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
+        match valueType:
+            case 7:
+                return nbtlib.tag.ByteArray([unpack(f'{endian}b', getByte(buffer, 1))[0] for _ in range(arrayLength)])
+            case 11:
+                return nbtlib.tag.IntArray([unpack(f'{endian}i', getByte(buffer, 4))[0] for _ in range(arrayLength)])
+            case 12:
+                return nbtlib.tag.LongArray([unpack(f'{endian}q', getByte(buffer, 8))[0] for _ in range(arrayLength)])
+            case _:
+                raise unexpectedError(valueType)
+else:
+    def getArray(buffer: BytesIO, valueType: int) -> nbtlib.tag.ByteArray | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
+        arrayLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
+        if valueType == 7:
+            return nbtlib.tag.ByteArray([unpack(f'{endian}b', getByte(buffer, 1))[0] for _ in range(arrayLength)])
+        elif valueType ==11:
+            return nbtlib.tag.IntArray([unpack(f'{endian}i', getByte(buffer, 4))[0] for _ in range(arrayLength)])
+        elif valueType ==12:
+            return nbtlib.tag.LongArray([unpack(f'{endian}q', getByte(buffer, 8))[0] for _ in range(arrayLength)])
+        else:
+            raise unexpectedError(valueType)
 
 def getList(buffer: BytesIO) -> nbtlib.tag.List:
     valueType = getByte(buffer, 1)[0]
     listLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
     return nbtlib.tag.List([getValue(buffer, valueType) for _ in range(listLength)])
```

### Comparing `BDXConverter-1.0.10/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.11/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: BDXConverter
-Version: 1.0.10
-Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
-Home-page: https://github.com/TriM-Organization/BDXConverter
-Author: Minecraft Muti-Media Organization
-Author-email: TriM-Organization@hotmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -33,14 +19,19 @@
 
 
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+使用下述命令快速安装吧
+```shell
+pip install BDXConverter
+```
+> 我们建议您在 Python 3.10及其以上版本使用他,3.7及其以下版本Python不再维护更新
 
 # 项目依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
```

### Comparing `BDXConverter-1.0.10/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.11/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/LICENSE` & `BDXConverter-1.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.10/PKG-INFO` & `BDXConverter-1.0.11/BDXConverter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.10
+Version: 1.0.11
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,19 @@
 
 
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+使用下述命令快速安装吧
+```shell
+pip install BDXConverter
+```
+> 我们建议您在 Python 3.10及其以上版本使用他,3.7及其以下版本Python不再维护更新
 
 # 项目依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
```

### Comparing `BDXConverter-1.0.10/README.md` & `BDXConverter-1.0.11/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: BDXConverter
+Version: 1.0.11
+Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
+Home-page: https://github.com/TriM-Organization/BDXConverter
+Author: Minecraft Muti-Media Organization
+Author-email: TriM-Organization@hotmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -19,14 +33,19 @@
 
 
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+使用下述命令快速安装吧
+```shell
+pip install BDXConverter
+```
+> 我们建议您在 Python 3.10及其以上版本使用他,3.7及其以下版本Python不再维护更新
 
 # 项目依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
```

### Comparing `BDXConverter-1.0.10/setup.py` & `BDXConverter-1.0.11/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import setuptools
 
 with open("requirements.txt", "r+", encoding="utf-8") as file:
     dependences = file.read().strip().split("\n")
-file.close()
-
 with open("README.md", "r+", encoding='utf-8') as file:
     long_description = file.read()
-file.close()
-
+with open("version", "r+", encoding='utf-8') as file:
+    version = file.read()
 setuptools.setup(
     name="BDXConverter",
-    version="1.0.10",
+    version=version,
     author="Minecraft Muti-Media Organization",
     author_email="TriM-Organization@hotmail.com",
     description="A code library to marshal, unmarshal, visual and reverse visualization of BDX files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TriM-Organization/BDXConverter",
     packages=setuptools.find_packages(),
```

