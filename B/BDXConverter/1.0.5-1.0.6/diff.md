# Comparing `tmp/BDXConverter-1.0.5.tar.gz` & `tmp/BDXConverter-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.5.tar", last modified: Tue May  2 05:13:25 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.6.tar", last modified: Tue May  2 05:17:20 2023, max compression
```

## Comparing `BDXConverter-1.0.5.tar` & `BDXConverter-1.0.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.127890 BDXConverter-1.0.5/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.131890 BDXConverter-1.0.5/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Converter/ConvertErrorDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.131890 BDXConverter-1.0.5/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.143890 BDXConverter-1.0.5/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/Terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/unmarshalNBT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.127890 BDXConverter-1.0.5/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:17:20.042656 BDXConverter-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:17:20.034655 BDXConverter-1.0.6/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:17:20.034655 BDXConverter-1.0.6/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:17:20.034655 BDXConverter-1.0.6/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:17:20.042656 BDXConverter-1.0.6/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/Terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:17:20.042656 BDXConverter-1.0.6/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/BDXConverter/utils/unmarshalNBT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:17:20.034655 BDXConverter-1.0.6/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-02 05:17:20.000000 BDXConverter-1.0.6/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-02 05:17:20.000000 BDXConverter-1.0.6/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:17:20.000000 BDXConverter-1.0.6/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 05:17:20.000000 BDXConverter-1.0.6/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 05:17:20.000000 BDXConverter-1.0.6/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-02 05:17:20.042656 BDXConverter-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:17:20.042656 BDXConverter-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-02 05:16:56.000000 BDXConverter-1.0.6/setup.py
```

### Comparing `BDXConverter-1.0.5/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.6/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.6/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.0.6/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/General/Pool.py` & `BDXConverter-1.0.6/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.6/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.0.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.0.6/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.0.6/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.6/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.0.6/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.0.6/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.6/BDXConverter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.5
+Version: 1.0.6
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `BDXConverter-1.0.5/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.6/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/LICENSE` & `BDXConverter-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/PKG-INFO` & `BDXConverter-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.5
+Version: 1.0.6
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `BDXConverter-1.0.5/README.md` & `BDXConverter-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.5/setup.py` & `BDXConverter-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r+", encoding='utf-8') as file:
     long_description = file.read()
 file.close()
 
 setuptools.setup(
     name="BDXConverter",
-    version="1.0.5",
+    version="1.0.6",
     author="Minecraft Muti-Media Organization",
     author_email="TriM-Organization@hotmail.com",
     description="A code library to marshal, unmarshal, visual and reverse visualization of BDX files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TriM-Organization/BDXConverter",
     packages=setuptools.find_packages(),
```

