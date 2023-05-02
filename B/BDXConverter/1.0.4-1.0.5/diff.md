# Comparing `tmp/BDXConverter-1.0.4.tar.gz` & `tmp/BDXConverter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.4.tar", last modified: Tue May  2 03:48:20 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.5.tar", last modified: Tue May  2 05:13:25 2023, max compression
```

## Comparing `BDXConverter-1.0.4.tar` & `BDXConverter-1.0.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 03:48:20.615148 BDXConverter-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-02 03:48:20.176651 BDXConverter-1.0.4/BDXConverter/
-drwxrwxrwx   0        0        0        0 2023-05-02 03:48:20.215647 BDXConverter-1.0.4/BDXConverter/Converter/
--rw-rw-rw-   0        0        0      808 2023-05-02 01:50:46.000000 BDXConverter-1.0.4/BDXConverter/Converter/ConvertErrorDefine.py
--rw-rw-rw-   0        0        0     4722 2023-05-02 01:53:27.000000 BDXConverter-1.0.4/BDXConverter/Converter/Converter.py
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.4/BDXConverter/Converter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:48:20.229648 BDXConverter-1.0.4/BDXConverter/General/
--rw-rw-rw-   0        0        0      792 2023-05-02 01:50:46.000000 BDXConverter-1.0.4/BDXConverter/General/GeneralClass.py
--rw-rw-rw-   0        0        0     4167 2023-05-02 01:53:47.000000 BDXConverter-1.0.4/BDXConverter/General/Pool.py
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.4/BDXConverter/General/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:48:20.593147 BDXConverter-1.0.4/BDXConverter/Operation/
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:19.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt16XValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:24.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt16YValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:27.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt16ZValue.py
--rw-rw-rw-   0        0        0      665 2023-05-02 01:56:31.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt16ZValue0.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:38.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt32XValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:44.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt32YValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:49.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt32ZValue.py
--rw-rw-rw-   0        0        0      666 2023-05-02 01:56:53.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt32ZValue0.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:56:01.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt8XValue.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:56:09.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt8YValue.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:56:13.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddInt8ZValue.py
--rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddXValue.py
--rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddYValue.py
--rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddZValue.py
--rw-rw-rw-   0        0        0      206 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/AddZValue0.py
--rw-rw-rw-   0        0        0     1273 2023-05-02 01:57:01.000000 BDXConverter-1.0.4/BDXConverter/Operation/AssignDebugData.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:57:14.000000 BDXConverter-1.0.4/BDXConverter/Operation/CreateConstantString.py
--rw-rw-rw-   0        0        0      192 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/NOP.py
--rw-rw-rw-   0        0        0      979 2023-05-02 01:57:21.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlock.py
--rw-rw-rw-   0        0        0     1131 2023-05-02 01:57:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-rw-rw-   0        0        0     1098 2023-05-02 01:57:36.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-rw-rw-   0        0        0     2082 2023-05-02 02:00:06.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-rw-rw-   0        0        0     3132 2023-05-02 01:58:03.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-rw-rw-   0        0        0     2163 2023-05-02 01:58:14.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-rw-rw-   0        0        0      706 2023-05-02 01:58:19.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-rw-rw-   0        0        0     2830 2023-05-02 01:58:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-rw-rw-   0        0        0      694 2023-05-02 01:58:29.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-rw-rw-   0        0        0     1689 2023-05-02 01:58:56.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-rw-rw-   0        0        0     1725 2023-05-02 01:59:13.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-rw-rw-   0        0        0     2868 2023-05-02 01:59:21.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-rw-rw-   0        0        0     2904 2023-05-02 01:59:28.000000 BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-rw-rw-   0        0        0     2618 2023-05-02 01:59:35.000000 BDXConverter-1.0.4/BDXConverter/Operation/SetCommandBlockData.py
--rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/SubtractXValue.py
--rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/SubtractYValue.py
--rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/SubtractZValue.py
--rw-rw-rw-   0        0        0      495 2023-05-02 01:55:26.000000 BDXConverter-1.0.4/BDXConverter/Operation/Terminate.py
--rw-rw-rw-   0        0        0      679 2023-05-02 01:55:44.000000 BDXConverter-1.0.4/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.4/BDXConverter/Operation/__init__.py
--rw-rw-rw-   0        0        0     2322 2023-05-02 01:59:44.000000 BDXConverter-1.0.4/BDXConverter/Operation/structOfChest.py
--rw-rw-rw-   0        0        0       48 2023-05-02 03:10:12.000000 BDXConverter-1.0.4/BDXConverter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:48:20.610146 BDXConverter-1.0.4/BDXConverter/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.4/BDXConverter/utils/__init__.py
--rw-rw-rw-   0        0        0      194 2023-05-02 01:50:46.000000 BDXConverter-1.0.4/BDXConverter/utils/getByte.py
--rw-rw-rw-   0        0        0      337 2023-05-02 01:54:14.000000 BDXConverter-1.0.4/BDXConverter/utils/getString.py
--rw-rw-rw-   0        0        0     3310 2023-05-02 01:50:46.000000 BDXConverter-1.0.4/BDXConverter/utils/marshalNBT.py
--rw-rw-rw-   0        0        0     3676 2023-05-02 01:54:31.000000 BDXConverter-1.0.4/BDXConverter/utils/unmarshalNBT.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:48:20.200647 BDXConverter-1.0.4/BDXConverter.egg-info/
--rw-rw-rw-   0        0        0     3789 2023-05-02 03:48:19.000000 BDXConverter-1.0.4/BDXConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2385 2023-05-02 03:48:20.000000 BDXConverter-1.0.4/BDXConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 03:48:19.000000 BDXConverter-1.0.4/BDXConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-02 03:48:19.000000 BDXConverter-1.0.4/BDXConverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 03:48:19.000000 BDXConverter-1.0.4/BDXConverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2023-05-01 15:39:04.000000 BDXConverter-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3789 2023-05-02 03:48:20.614146 BDXConverter-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3246 2023-05-02 03:48:07.000000 BDXConverter-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 03:48:20.615148 BDXConverter-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-05-02 03:48:15.000000 BDXConverter-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.127890 BDXConverter-1.0.5/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.131890 BDXConverter-1.0.5/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.131890 BDXConverter-1.0.5/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.143890 BDXConverter-1.0.5/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/Terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/BDXConverter/utils/unmarshalNBT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:13:25.127890 BDXConverter-1.0.5/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 05:13:25.000000 BDXConverter-1.0.5/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:13:25.147890 BDXConverter-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-02 05:13:00.000000 BDXConverter-1.0.5/setup.py
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.5/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-class notAcorrectBDXFileError(Exception):
-    """
-    Not a correct BDX file error
-    """
-
-    def __init__(self, path: str):
-        Exception.__init__(self, f'"{path}" is not a correct BDX file')
-
-
-class readError(Exception):
-    """
-    BDX file read error
-    """
-
-    def __init__(self, errorOccurredPosition: int):
-        Exception.__init__(
-            self, f'failed to convert this BDX file, and the error occurred at position {errorOccurredPosition}')
-
-
-class unknownOperationError(Exception):
-    """
-    Find unknown operation error
-    """
-
-    def __init__(self, operationId: int, errorOccurredPosition: int):
-        Exception.__init__(
-            self, f'an unknown operation {operationId} was found, and the error occurred at position {errorOccurredPosition}')
+class notAcorrectBDXFileError(Exception):
+    """
+    Not a correct BDX file error
+    """
+
+    def __init__(self, path: str):
+        Exception.__init__(self, f'"{path}" is not a correct BDX file')
+
+
+class readError(Exception):
+    """
+    BDX file read error
+    """
+
+    def __init__(self, errorOccurredPosition: int):
+        Exception.__init__(
+            self, f'failed to convert this BDX file, and the error occurred at position {errorOccurredPosition}')
+
+
+class unknownOperationError(Exception):
+    """
+    Find unknown operation error
+    """
+
+    def __init__(self, operationId: int, errorOccurredPosition: int):
+        Exception.__init__(
+            self, f'an unknown operation {operationId} was found, and the error occurred at position {errorOccurredPosition}')
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.5/BDXConverter/Converter/Converter.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-from ..General.GeneralClass import GeneralClass
-from ..General.Pool import GetBDXCommandPool
-from ..utils.getString import getByte, getString
-from .ConvertErrorDefine import notAcorrectBDXFileError
-from .ConvertErrorDefine import readError, unknownOperationError
-from brotli import compress, decompress
-from io import BytesIO
-from json import loads, dumps
-from copy import deepcopy
-
-
-def ReadBDXFile(path: str) -> tuple[list[GeneralClass], str]:
-    """
-    Convert BDX file into list[GeneralClass] and return the author's name
-    """
-    with open(path, "r+b") as file:
-        fileContext: bytes = file.read()
-    file.close()
-    # get the context of this bdx file
-    if fileContext[0:3] != b'BD@':
-        raise notAcorrectBDXFileError(path)
-    buffer = BytesIO(decompress(fileContext[3:]))
-    if getByte(buffer, 3) != b'BDX':
-        raise notAcorrectBDXFileError(path)
-    # check header and create new buffer
-    result: list[GeneralClass] = []
-    bdxCommandPool: dict[int, GeneralClass] = GetBDXCommandPool()
-    # prepare
-    getByte(buffer, 1)
-    authorName = getString(buffer)
-    # get author's information
-    while True:
-        commandId = getByte(buffer, 1)
-        if commandId[0] in bdxCommandPool:
-            struct: GeneralClass = deepcopy(bdxCommandPool[commandId[0]])
-            # get struct(operation) from the pool
-            try:
-                struct.UnMarshal(buffer)
-            except EOFError:
-                raise EOFError
-            except:
-                raise readError(buffer.seek(0, 1))
-            # unmarshal bytes into python object(GeneralClass)
-            result.append(struct)
-            # submit single datas
-            if struct.operationNumber == 88:
-                break
-            # if meet operation Terminate(88)
-        else:
-            raise unknownOperationError(commandId[0], buffer.seek(0, 1))
-            # if we can not find the operation from the command pool
-    # read bdx file
-    return result, authorName
-    # return
-
-
-def DumpStructs(
-        structs: list[GeneralClass],
-        outputPath: str,
-        authorName: str = 'KazamataNeri/MCConvertExecute-bdx'
-) -> None:
-    """
-    Convert list[GeneralClass] into bytes and write it into a bdx file(outputPath:str).
-
-    Note:
-        - Author's name is no need to write,
-        because this field has been officially deprecated.
-        But we still put the names into this place as symbolically
-    """
-    writer: BytesIO = BytesIO(b'')
-    # request a new writer
-    writer.write(b'BDX\x00'+authorName.encode(encoding='utf-8')+b'\x00')
-    # write inside header(BDX) and author's name
-    for i in structs:
-        writer.write(i.operationNumber.to_bytes(
-            length=1, byteorder='big', signed=False))
-        i.Marshal(writer)
-    # marshal python object into the writer
-    result = b'BD@' + compress(writer.getvalue())
-    # compress writer into bytes and set outside header which named "BD@"
-    with open(outputPath, 'w+b') as file:
-        file.write(result)
-    file.close()
-    # write bytes into a bdx file
-
-
-def VisualStructs(structs: list[GeneralClass], outputPath: str) -> None:
-    """
-    Convert list[GeneralClass] into json data and write it into outputPath:str
-    """
-    new: list = []
-    for i in structs:
-        new.append(i.Dumps())
-    # convert bdx file in to basic datas
-    result: str = dumps(
-        new,
-        sort_keys=True,
-        indent=4,
-        separators=(', ', ': '),
-        ensure_ascii=False
-    )
-    # get string
-    with open(outputPath, 'w+', encoding='utf-8') as file:
-        file.write(result)
-    file.close()
-    # write json datas
-
-
-def ConvertJSONFileIntoStructs(path: str) -> list[GeneralClass]:
-    """
-    Read json datas from path:str and convert it into list[GeneralClass]
-    """
-    with open(path, 'r+', encoding='utf-8') as file:
-        fileContext: str = file.read()
-    jsonDatas: list[dict] = loads(fileContext)
-    # load json datas from file
-    result: list[GeneralClass] = []
-    bdxCommandPool: dict[int, GeneralClass] = GetBDXCommandPool()
-    # prepare
-    for i in jsonDatas:
-        if not 'operationNumber' in i:
-            continue
-        operationNumber: int = i['operationNumber']
-        if not operationNumber in bdxCommandPool:
-            continue
-        # get operation number
-        struct: GeneralClass = deepcopy(bdxCommandPool[operationNumber])
-        # request a new struct
-        struct.Loads(i)
-        # load datas
-        result.append(struct)
-        # submit single struct
-    # load datas from json dict
-    return result
-    # return
+from ..General.GeneralClass import GeneralClass
+from ..General.Pool import GetBDXCommandPool
+from ..utils.getString import getByte, getString
+from .ConvertErrorDefine import notAcorrectBDXFileError
+from .ConvertErrorDefine import readError, unknownOperationError
+from brotli import compress, decompress
+from io import BytesIO
+from json import loads, dumps
+from copy import deepcopy
+
+
+def ReadBDXFile(path: str) -> tuple[list[GeneralClass], str]:
+    """
+    Convert BDX file into list[GeneralClass] and return the author's name
+    """
+    with open(path, "r+b") as file:
+        fileContext: bytes = file.read()
+    file.close()
+    # get the context of this bdx file
+    if fileContext[0:3] != b'BD@':
+        raise notAcorrectBDXFileError(path)
+    buffer = BytesIO(decompress(fileContext[3:]))
+    if getByte(buffer, 3) != b'BDX':
+        raise notAcorrectBDXFileError(path)
+    # check header and create new buffer
+    result: list[GeneralClass] = []
+    bdxCommandPool: dict[int, GeneralClass] = GetBDXCommandPool()
+    # prepare
+    getByte(buffer, 1)
+    authorName = getString(buffer)
+    # get author's information
+    while True:
+        commandId = getByte(buffer, 1)
+        if commandId[0] in bdxCommandPool:
+            struct: GeneralClass = deepcopy(bdxCommandPool[commandId[0]])
+            # get struct(operation) from the pool
+            try:
+                struct.UnMarshal(buffer)
+            except EOFError:
+                raise EOFError
+            except:
+                raise readError(buffer.seek(0, 1))
+            # unmarshal bytes into python object(GeneralClass)
+            result.append(struct)
+            # submit single datas
+            if struct.operationNumber == 88:
+                break
+            # if meet operation Terminate(88)
+        else:
+            raise unknownOperationError(commandId[0], buffer.seek(0, 1))
+            # if we can not find the operation from the command pool
+    # read bdx file
+    return result, authorName
+    # return
+
+
+def DumpStructs(
+        structs: list[GeneralClass],
+        outputPath: str,
+        authorName: str = 'KazamataNeri/MCConvertExecute-bdx'
+) -> None:
+    """
+    Convert list[GeneralClass] into bytes and write it into a bdx file(outputPath:str).
+
+    Note:
+        - Author's name is no need to write,
+        because this field has been officially deprecated.
+        But we still put the names into this place as symbolically
+    """
+    writer: BytesIO = BytesIO(b'')
+    # request a new writer
+    writer.write(b'BDX\x00'+authorName.encode(encoding='utf-8')+b'\x00')
+    # write inside header(BDX) and author's name
+    for i in structs:
+        writer.write(i.operationNumber.to_bytes(
+            length=1, byteorder='big', signed=False))
+        i.Marshal(writer)
+    # marshal python object into the writer
+    result = b'BD@' + compress(writer.getvalue())
+    # compress writer into bytes and set outside header which named "BD@"
+    with open(outputPath, 'w+b') as file:
+        file.write(result)
+    file.close()
+    # write bytes into a bdx file
+
+
+def VisualStructs(structs: list[GeneralClass], outputPath: str) -> None:
+    """
+    Convert list[GeneralClass] into json data and write it into outputPath:str
+    """
+    new: list = []
+    for i in structs:
+        new.append(i.Dumps())
+    # convert bdx file in to basic datas
+    result: str = dumps(
+        new,
+        sort_keys=True,
+        indent=4,
+        separators=(', ', ': '),
+        ensure_ascii=False
+    )
+    # get string
+    with open(outputPath, 'w+', encoding='utf-8') as file:
+        file.write(result)
+    file.close()
+    # write json datas
+
+
+def ConvertJSONFileIntoStructs(path: str) -> list[GeneralClass]:
+    """
+    Read json datas from path:str and convert it into list[GeneralClass]
+    """
+    with open(path, 'r+', encoding='utf-8') as file:
+        fileContext: str = file.read()
+    jsonDatas: list[dict] = loads(fileContext)
+    # load json datas from file
+    result: list[GeneralClass] = []
+    bdxCommandPool: dict[int, GeneralClass] = GetBDXCommandPool()
+    # prepare
+    for i in jsonDatas:
+        if not 'operationNumber' in i:
+            continue
+        operationNumber: int = i['operationNumber']
+        if not operationNumber in bdxCommandPool:
+            continue
+        # get operation number
+        struct: GeneralClass = deepcopy(bdxCommandPool[operationNumber])
+        # request a new struct
+        struct.Loads(i)
+        # load datas
+        result.append(struct)
+        # submit single struct
+    # load datas from json dict
+    return result
+    # return
```

### Comparing `BDXConverter-1.0.4/BDXConverter/General/Pool.py` & `BDXConverter-1.0.5/BDXConverter/General/Pool.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from .GeneralClass import GeneralClass
-
-from ..Operation.CreateConstantString import CreateConstantString
-from ..Operation.PlaceBlockWithBlockStates import PlaceBlockWithBlockStates
-from ..Operation.AddInt16ZValue0 import AddInt16ZValue0
-from ..Operation.PlaceBlock import PlaceBlock
-from ..Operation.AddZValue0 import AddZValue0
-from ..Operation.NOP import NOP
-from ..Operation.AddInt32ZValue0 import AddInt32ZValue0
-from ..Operation.PlaceBlockWithBlockStatesDeprecated import PlaceBlockWithBlockStatesDeprecated
-from ..Operation.AddXValue import AddXValue
-from ..Operation.SubtractXValue import SubtractXValue
-from ..Operation.AddYValue import AddYValue
-from ..Operation.SubtractYValue import SubtractYValue
-from ..Operation.AddZValue import AddZValue
-from ..Operation.SubtractZValue import SubtractZValue
-from ..Operation.AddInt16XValue import AddInt16XValue
-from ..Operation.AddInt32XValue import AddInt32XValue
-from ..Operation.AddInt16YValue import AddInt16YValue
-from ..Operation.AddInt32YValue import AddInt32YValue
-from ..Operation.AddInt16XValue import AddInt16XValue
-from ..Operation.AddInt32XValue import AddInt32XValue
-from ..Operation.AddInt16YValue import AddInt16YValue
-from ..Operation.AddInt32YValue import AddInt32YValue
-from ..Operation.AddInt16ZValue import AddInt16ZValue
-from ..Operation.AddInt32ZValue import AddInt32ZValue
-from ..Operation.SetCommandBlockData import SetCommandBlockData
-from ..Operation.PlaceBlockWithCommandBlockData import PlaceBlockWithCommandBlockData
-from ..Operation.AddInt8XValue import AddInt8XValue
-from ..Operation.AddInt8YValue import AddInt8YValue
-from ..Operation.AddInt8ZValue import AddInt8ZValue
-from ..Operation.UseRuntimeIDPool import UseRuntimeIDPool
-from ..Operation.PlaceRuntimeBlock import PlaceRuntimeBlock
-from ..Operation.PlaceBlockWithRuntimeId import PlaceBlockWithRuntimeId
-from ..Operation.PlaceRuntimeBlockWithCommandBlockData import PlaceRuntimeBlockWithCommandBlockData
-from ..Operation.PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID import PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID
-from ..Operation.PlaceCommandBlockWithCommandBlockData import PlaceCommandBlockWithCommandBlockData
-from ..Operation.PlaceRuntimeBlockWithChestData import PlaceRuntimeBlockWithChestData
-from ..Operation.PlaceRuntimeBlockWithChestDataAndUint32RuntimeID import PlaceRuntimeBlockWithChestDataAndUint32RuntimeID
-from ..Operation.AssignDebugData import AssignDebugData
-from ..Operation.PlaceBlockWithChestData import PlaceBlockWithChestData
-from ..Operation.PlaceBlockWithNBTData import PlaceBlockWithNBTData
-from ..Operation.Terminate import Terminate
-
-
-def GetBDXCommandPool() -> dict[int, GeneralClass]:
-    """
-    Return dict[commandId(..operationId):int, PythonClass:GeneralClass]
-    """
-    return {
-        1: CreateConstantString(),
-        5: PlaceBlockWithBlockStates(),
-        6: AddInt16ZValue0(),
-        7: PlaceBlock(),
-        8: AddZValue0(),
-        9: NOP(),
-        12: AddInt32ZValue0(),
-        13: PlaceBlockWithBlockStatesDeprecated(),
-        14: AddXValue(),
-        15: SubtractXValue(),
-        16: AddYValue(),
-        17: SubtractYValue(),
-        18: AddZValue(),
-        19: SubtractZValue(),
-        20: AddInt16XValue(),
-        21: AddInt32XValue(),
-        22: AddInt16YValue(),
-        23: AddInt32YValue(),
-        24: AddInt16ZValue(),
-        25: AddInt32ZValue(),
-        26: SetCommandBlockData(),
-        27: PlaceBlockWithCommandBlockData(),
-        28: AddInt8XValue(),
-        29: AddInt8YValue(),
-        30: AddInt8ZValue(),
-        31: UseRuntimeIDPool(),
-        32: PlaceRuntimeBlock(),
-        33: PlaceBlockWithRuntimeId(),
-        34: PlaceRuntimeBlockWithCommandBlockData(),
-        35: PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID(),
-        36: PlaceCommandBlockWithCommandBlockData(),
-        37: PlaceRuntimeBlockWithChestData(),
-        38: PlaceRuntimeBlockWithChestDataAndUint32RuntimeID(),
-        39: AssignDebugData(),
-        40: PlaceBlockWithChestData(),
-        41: PlaceBlockWithNBTData(),
-        88: Terminate()
-    }
+from .GeneralClass import GeneralClass
+
+from ..Operation.CreateConstantString import CreateConstantString
+from ..Operation.PlaceBlockWithBlockStates import PlaceBlockWithBlockStates
+from ..Operation.AddInt16ZValue0 import AddInt16ZValue0
+from ..Operation.PlaceBlock import PlaceBlock
+from ..Operation.AddZValue0 import AddZValue0
+from ..Operation.NOP import NOP
+from ..Operation.AddInt32ZValue0 import AddInt32ZValue0
+from ..Operation.PlaceBlockWithBlockStatesDeprecated import PlaceBlockWithBlockStatesDeprecated
+from ..Operation.AddXValue import AddXValue
+from ..Operation.SubtractXValue import SubtractXValue
+from ..Operation.AddYValue import AddYValue
+from ..Operation.SubtractYValue import SubtractYValue
+from ..Operation.AddZValue import AddZValue
+from ..Operation.SubtractZValue import SubtractZValue
+from ..Operation.AddInt16XValue import AddInt16XValue
+from ..Operation.AddInt32XValue import AddInt32XValue
+from ..Operation.AddInt16YValue import AddInt16YValue
+from ..Operation.AddInt32YValue import AddInt32YValue
+from ..Operation.AddInt16XValue import AddInt16XValue
+from ..Operation.AddInt32XValue import AddInt32XValue
+from ..Operation.AddInt16YValue import AddInt16YValue
+from ..Operation.AddInt32YValue import AddInt32YValue
+from ..Operation.AddInt16ZValue import AddInt16ZValue
+from ..Operation.AddInt32ZValue import AddInt32ZValue
+from ..Operation.SetCommandBlockData import SetCommandBlockData
+from ..Operation.PlaceBlockWithCommandBlockData import PlaceBlockWithCommandBlockData
+from ..Operation.AddInt8XValue import AddInt8XValue
+from ..Operation.AddInt8YValue import AddInt8YValue
+from ..Operation.AddInt8ZValue import AddInt8ZValue
+from ..Operation.UseRuntimeIDPool import UseRuntimeIDPool
+from ..Operation.PlaceRuntimeBlock import PlaceRuntimeBlock
+from ..Operation.PlaceBlockWithRuntimeId import PlaceBlockWithRuntimeId
+from ..Operation.PlaceRuntimeBlockWithCommandBlockData import PlaceRuntimeBlockWithCommandBlockData
+from ..Operation.PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID import PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID
+from ..Operation.PlaceCommandBlockWithCommandBlockData import PlaceCommandBlockWithCommandBlockData
+from ..Operation.PlaceRuntimeBlockWithChestData import PlaceRuntimeBlockWithChestData
+from ..Operation.PlaceRuntimeBlockWithChestDataAndUint32RuntimeID import PlaceRuntimeBlockWithChestDataAndUint32RuntimeID
+from ..Operation.AssignDebugData import AssignDebugData
+from ..Operation.PlaceBlockWithChestData import PlaceBlockWithChestData
+from ..Operation.PlaceBlockWithNBTData import PlaceBlockWithNBTData
+from ..Operation.Terminate import Terminate
+
+
+def GetBDXCommandPool() -> dict[int, GeneralClass]:
+    """
+    Return dict[commandId(..operationId):int, PythonClass:GeneralClass]
+    """
+    return {
+        1: CreateConstantString(),
+        5: PlaceBlockWithBlockStates(),
+        6: AddInt16ZValue0(),
+        7: PlaceBlock(),
+        8: AddZValue0(),
+        9: NOP(),
+        12: AddInt32ZValue0(),
+        13: PlaceBlockWithBlockStatesDeprecated(),
+        14: AddXValue(),
+        15: SubtractXValue(),
+        16: AddYValue(),
+        17: SubtractYValue(),
+        18: AddZValue(),
+        19: SubtractZValue(),
+        20: AddInt16XValue(),
+        21: AddInt32XValue(),
+        22: AddInt16YValue(),
+        23: AddInt32YValue(),
+        24: AddInt16ZValue(),
+        25: AddInt32ZValue(),
+        26: SetCommandBlockData(),
+        27: PlaceBlockWithCommandBlockData(),
+        28: AddInt8XValue(),
+        29: AddInt8YValue(),
+        30: AddInt8ZValue(),
+        31: UseRuntimeIDPool(),
+        32: PlaceRuntimeBlock(),
+        33: PlaceBlockWithRuntimeId(),
+        34: PlaceRuntimeBlockWithCommandBlockData(),
+        35: PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID(),
+        36: PlaceCommandBlockWithCommandBlockData(),
+        37: PlaceRuntimeBlockWithChestData(),
+        38: PlaceRuntimeBlockWithChestDataAndUint32RuntimeID(),
+        39: AssignDebugData(),
+        40: PlaceBlockWithChestData(),
+        41: PlaceBlockWithNBTData(),
+        88: Terminate()
+    }
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt8YValue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt16XValue(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt16XValue'
-        self.operationNumber: int = 20
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>h', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>h', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt8YValue(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt8YValue'
+        self.operationNumber: int = 29
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(self.value.to_bytes(
+            length=1, byteorder='big', signed=True))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>b', getByte(buffer, 1))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16YValue.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt16YValue(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt16YValue'
-        self.operationNumber: int = 22
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>h', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>h', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt16YValue(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt16YValue'
+        self.operationNumber: int = 22
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>h', self.value))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>h', getByte(buffer, 2))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt16ZValue(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt16ZValue'
-        self.operationNumber: int = 24
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>h', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>h', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt16ZValue(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt16ZValue'
+        self.operationNumber: int = 24
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>h', self.value))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>h', getByte(buffer, 2))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt16ZValue0(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt16ZValue0'
-        self.operationNumber: int = 6
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>H', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt16ZValue0(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt16ZValue0'
+        self.operationNumber: int = 6
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.value))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>H', getByte(buffer, 2))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt16XValue.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt32XValue(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt32XValue'
-        self.operationNumber: int = 21
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>i', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>i', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt16XValue(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt16XValue'
+        self.operationNumber: int = 20
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>h', self.value))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>h', getByte(buffer, 2))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt32YValue(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt32YValue'
-        self.operationNumber: int = 23
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>i', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>i', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt8ZValue(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt8ZValue'
+        self.operationNumber: int = 30
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(self.value.to_bytes(
+            length=1, byteorder='big', signed=True))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>b', getByte(buffer, 1))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt8XValue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt32ZValue(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt32ZValue'
-        self.operationNumber: int = 25
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>i', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>i', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt8XValue(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt8XValue'
+        self.operationNumber: int = 28
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(self.value.to_bytes(
+            length=1, byteorder='big', signed=True))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>b', getByte(buffer, 1))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AddInt32ZValue0(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AddInt32ZValue0'
-        self.operationNumber: int = 12
-        self.value: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>I', self.value))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.value = unpack('>I', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.value = jsonDict['value'] if 'value' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AddInt32ZValue0(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AddInt32ZValue0'
+        self.operationNumber: int = 12
+        self.value: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>I', self.value))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.value = unpack('>I', getByte(buffer, 4))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.value = jsonDict['value'] if 'value' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.5/BDXConverter/Operation/AssignDebugData.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class AssignDebugData(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'AssignDebugData'
-        self.operationNumber: int = 39
-        self.length: int = 0
-        self.buffer: bytes = b''
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>I', self.length) + self.buffer)
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.length = unpack('>I', getByte(buffer, 4))[0]
-        self.buffer = getByte(buffer, self.length)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.length = jsonDict['length'] if 'length' in jsonDict else 0
-        self.buffer = b''.join(
-            [
-                i.to_bytes(length=1, byteorder='big', signed=False)
-                for i in jsonDict['buffer']
-            ]
-        ) if 'buffer' in jsonDict else b''
-
-    def Dumps(self) -> dict:
-        result: dict = {
-            'operationName': self.operationName,
-            'operationNumber': self.operationNumber,
-            'length': self.length,
-            'buffer': [i for i in self.buffer]
-        }
-        return result
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class AssignDebugData(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'AssignDebugData'
+        self.operationNumber: int = 39
+        self.length: int = 0
+        self.buffer: bytes = b''
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>I', self.length) + self.buffer)
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.length = unpack('>I', getByte(buffer, 4))[0]
+        self.buffer = getByte(buffer, self.length)
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.length = jsonDict['length'] if 'length' in jsonDict else 0
+        self.buffer = b''.join(
+            [
+                i.to_bytes(length=1, byteorder='big', signed=False)
+                for i in jsonDict['buffer']
+            ]
+        ) if 'buffer' in jsonDict else b''
+
+    def Dumps(self) -> dict:
+        result: dict = {
+            'operationName': self.operationName,
+            'operationNumber': self.operationNumber,
+            'length': self.length,
+            'buffer': [i for i in self.buffer]
+        }
+        return result
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.5/BDXConverter/Operation/CreateConstantString.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from io import BytesIO
-from ..General.GeneralClass import GeneralClass
-from ..utils.getString import getString
-
-
-class CreateConstantString(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'CreateConstantString'
-        self.operationNumber: int = 1
-        self.constantString: str = ''
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(self.constantString.encode(encoding='utf-8') + b'\x00')
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.constantString = getString(buffer)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.constantString = jsonDict['constantString'] if 'constantString' in jsonDict else ''
+from io import BytesIO
+from ..General.GeneralClass import GeneralClass
+from ..utils.getString import getString
+
+
+class CreateConstantString(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'CreateConstantString'
+        self.operationNumber: int = 1
+        self.constantString: str = ''
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(self.constantString.encode(encoding='utf-8') + b'\x00')
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.constantString = getString(buffer)
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.constantString = jsonDict['constantString'] if 'constantString' in jsonDict else ''
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlock.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class PlaceBlock(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlock'
-        self.operationNumber: int = 7
-        self.blockConstantStringID: int = 0
-        self.blockData: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) +
-                     pack('>H', self.blockData))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockData = unpack('>H', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class PlaceBlock(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceBlock'
+        self.operationNumber: int = 7
+        self.blockConstantStringID: int = 0
+        self.blockData: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.blockConstantStringID) +
+                     pack('>H', self.blockData))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
+        self.blockData = unpack('>H', getByte(buffer, 2))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
+        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class PlaceBlockWithBlockStates(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlockWithBlockStates'
-        self.operationNumber: int = 5
-        self.blockConstantStringID: int = 0
-        self.blockStatesConstantStringID: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) +
-                     pack('>H', self.blockStatesConstantStringID))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockStatesConstantStringID = jsonDict[
-            'blockStatesConstantStringID'] if 'blockStatesConstantStringID' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class PlaceBlockWithBlockStates(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceBlockWithBlockStates'
+        self.operationNumber: int = 5
+        self.blockConstantStringID: int = 0
+        self.blockStatesConstantStringID: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.blockConstantStringID) +
+                     pack('>H', self.blockStatesConstantStringID))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
+        self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
+        self.blockStatesConstantStringID = jsonDict[
+            'blockStatesConstantStringID'] if 'blockStatesConstantStringID' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getString import getByte, getString
-
-
-class PlaceBlockWithBlockStatesDeprecated(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlockWithBlockStatesDeprecated'
-        self.operationNumber: int = 13
-        self.blockConstantStringID: int = 0
-        self.blockStatesString: str = ''
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) +
-                     self.blockStatesString.encode(encoding='utf-8') + b'\x00')
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockStatesString = getString(buffer)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockStatesString = jsonDict['blockStatesString'] if 'blockStatesString' in jsonDict else ''
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getString import getByte, getString
+
+
+class PlaceBlockWithBlockStatesDeprecated(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceBlockWithBlockStatesDeprecated'
+        self.operationNumber: int = 13
+        self.blockConstantStringID: int = 0
+        self.blockStatesString: str = ''
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.blockConstantStringID) +
+                     self.blockStatesString.encode(encoding='utf-8') + b'\x00')
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
+        self.blockStatesString = getString(buffer)
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
+        self.blockStatesString = jsonDict['blockStatesString'] if 'blockStatesString' in jsonDict else ''
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from io import BytesIO
-from struct import pack, unpack
-from .structOfChest import ChestData
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class PlaceBlockWithChestData(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlockWithChestData'
-        self.operationNumber: int = 40
-        self.blockConstantStringID: int = 0
-        self.blockData: int = 0
-        self.slotCount: int = 0
-        self.data: ChestData = ChestData()
-
-    def Marshal(self, writer: BytesIO) -> None:
-        self.slotCount = len(self.data.chestData)
-        writer.write(pack('>H', self.blockConstantStringID) + pack('>H', self.blockData) +
-                     self.slotCount.to_bytes(length=1, byteorder='big', signed=False))
-        self.data.Marshal(writer)
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockData = unpack('>H', getByte(buffer, 2))[0]
-        self.slotCount = getByte(buffer, 1)[0]
-        self.data.slotCount = self.slotCount
-        self.data.UnMarshal(buffer)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
-        # self.slotCount = jsonDict['slotCount'] if 'slotCount' in jsonDict else 0
-        newChestData = ChestData()
-        if 'data' in jsonDict:
-            newChestData.Loads(jsonDict['data'])
-        self.slotCount = self.data.slotCount
-        self.data = newChestData
-
-    def Dumps(self) -> dict:
-        result: dict = {
-            'operationName': self.operationName,
-            'operationNumber': self.operationNumber,
-            'blockConstantStringID': self.blockConstantStringID,
-            'blockData': self.blockData,
-            'slotCount': len(self.data.chestData),
-            'data': self.data.Dumps()
-        }
-        return result
+from io import BytesIO
+from struct import pack, unpack
+from .structOfChest import ChestData
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class PlaceBlockWithChestData(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceBlockWithChestData'
+        self.operationNumber: int = 40
+        self.blockConstantStringID: int = 0
+        self.blockData: int = 0
+        self.slotCount: int = 0
+        self.data: ChestData = ChestData()
+
+    def Marshal(self, writer: BytesIO) -> None:
+        self.slotCount = len(self.data.chestData)
+        writer.write(pack('>H', self.blockConstantStringID) + pack('>H', self.blockData) +
+                     self.slotCount.to_bytes(length=1, byteorder='big', signed=False))
+        self.data.Marshal(writer)
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
+        self.blockData = unpack('>H', getByte(buffer, 2))[0]
+        self.slotCount = getByte(buffer, 1)[0]
+        self.data.slotCount = self.slotCount
+        self.data.UnMarshal(buffer)
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
+        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
+        # self.slotCount = jsonDict['slotCount'] if 'slotCount' in jsonDict else 0
+        newChestData = ChestData()
+        if 'data' in jsonDict:
+            newChestData.Loads(jsonDict['data'])
+        self.slotCount = self.data.slotCount
+        self.data = newChestData
+
+    def Dumps(self) -> dict:
+        result: dict = {
+            'operationName': self.operationName,
+            'operationNumber': self.operationNumber,
+            'blockConstantStringID': self.blockConstantStringID,
+            'blockData': self.blockData,
+            'slotCount': len(self.data.chestData),
+            'data': self.data.Dumps()
+        }
+        return result
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getString import getByte, getString
-
-
-class PlaceBlockWithCommandBlockData(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlockWithCommandBlockData'
-        self.operationNumber: int = 27
-        self.blockConstantStringID: int = 0
-        self.blockData: int = 0
-        self.mode: int = 0
-        self.command: str = ''
-        self.customName: str = ''
-        self.lastOutput: str = ''
-        self.tickdelay: int = 0
-        self.executeOnFirstTick: bool = True
-        self.trackOutput: bool = True
-        self.conditional: bool = False
-        self.needsRedstone: bool = False
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) + pack('>H', self.blockData) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
-                     self.executeOnFirstTick.to_bytes(length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockData = unpack('>H', getByte(buffer, 2))[0]
-        self.mode = unpack('>I', getByte(buffer, 4))[0]
-        self.command = getString(buffer)
-        self.customName = getString(buffer)
-        self.lastOutput = getString(buffer)
-        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
-        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
-        self.trackOutput = bool(getByte(buffer, 1)[0])
-        self.conditional = bool(getByte(buffer, 1)[0])
-        self.needsRedstone = bool(getByte(buffer, 1)[0])
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockData = jsonDict['blockData'] if 'blockData' in jsonDict else 0
-        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
-        self.command = jsonDict['command'] if 'command' in jsonDict else ''
-        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
-        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
-        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
-        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
-        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
-        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
-        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getString import getByte, getString
+
+
+class PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID'
+        self.operationNumber: int = 35
+        self.runtimeId: int = 0
+        self.mode: int = 0
+        self.command: str = ''
+        self.customName: str = ''
+        self.lastOutput: str = ''
+        self.tickdelay: int = 0
+        self.executeOnFirstTick: bool = True
+        self.trackOutput: bool = True
+        self.conditional: bool = False
+        self.needsRedstone: bool = False
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>I', self.runtimeId) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
+                     self.executeOnFirstTick.to_bytes(length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
+        self.mode = unpack('>I', getByte(buffer, 4))[0]
+        self.command = getString(buffer)
+        self.customName = getString(buffer)
+        self.lastOutput = getString(buffer)
+        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
+        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
+        self.trackOutput = bool(getByte(buffer, 1)[0])
+        self.conditional = bool(getByte(buffer, 1)[0])
+        self.needsRedstone = bool(getByte(buffer, 1)[0])
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
+        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
+        self.command = jsonDict['command'] if 'command' in jsonDict else ''
+        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
+        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
+        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
+        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
+        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
+        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
+        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import nbtlib
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-from ..utils.marshalNBT import MarshalPythonNBTObjectToWriter
-from ..utils.unmarshalNBT import UnMarshalBufferToPythonNBTObject
-
-
-class PlaceBlockWithNBTData(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceBlockWithNBTData'
-        self.operationNumber: int = 41
-        self.blockConstantStringID: int = 0
-        self.blockStatesConstantStringID: int = 0
-        self.blockNBT: nbtlib.tag.Compound = nbtlib.tag.Compound({})
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) + pack('>H',
-                     self.blockStatesConstantStringID) + pack('>H', self.blockStatesConstantStringID))
-        MarshalPythonNBTObjectToWriter(writer, self.blockNBT, '')
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
-        getByte(buffer, 2)  # do not delete this line because it is correct
-        self.blockNBT, _ = UnMarshalBufferToPythonNBTObject(  # type: ignore
-            buffer)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
-        self.blockStatesConstantStringID = jsonDict[
-            'blockStatesConstantStringID'] if 'blockStatesConstantStringID' in jsonDict else 0
-        self.blockNBT = nbtlib.parse_nbt(
-            jsonDict['blockNBT']) if 'blockNBT' in jsonDict else nbtlib.tag.Compound({})
-
-    def Dumps(self) -> dict:
-        result: dict = {
-            'operationName': self.operationName,
-            'operationNumber': self.operationNumber,
-            'blockConstantStringID': self.blockConstantStringID,
-            'blockStatesConstantStringID': self.blockStatesConstantStringID,
-            'blockNBT': nbtlib.serialize_tag(self.blockNBT)
-        }
-        return result
+import nbtlib
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+from ..utils.marshalNBT import MarshalPythonNBTObjectToWriter
+from ..utils.unmarshalNBT import UnMarshalBufferToPythonNBTObject
+
+
+class PlaceBlockWithNBTData(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceBlockWithNBTData'
+        self.operationNumber: int = 41
+        self.blockConstantStringID: int = 0
+        self.blockStatesConstantStringID: int = 0
+        self.blockNBT: nbtlib.tag.Compound = nbtlib.tag.Compound({})
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.blockConstantStringID) + pack('>H',
+                     self.blockStatesConstantStringID) + pack('>H', self.blockStatesConstantStringID))
+        MarshalPythonNBTObjectToWriter(writer, self.blockNBT, '')
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
+        self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
+        getByte(buffer, 2)  # do not delete this line because it is correct
+        self.blockNBT, _ = UnMarshalBufferToPythonNBTObject(  # type: ignore
+            buffer)
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.blockConstantStringID = jsonDict['blockConstantStringID'] if 'blockConstantStringID' in jsonDict else 0
+        self.blockStatesConstantStringID = jsonDict[
+            'blockStatesConstantStringID'] if 'blockStatesConstantStringID' in jsonDict else 0
+        self.blockNBT = nbtlib.parse_nbt(
+            jsonDict['blockNBT']) if 'blockNBT' in jsonDict else nbtlib.tag.Compound({})
+
+    def Dumps(self) -> dict:
+        result: dict = {
+            'operationName': self.operationName,
+            'operationNumber': self.operationNumber,
+            'blockConstantStringID': self.blockConstantStringID,
+            'blockStatesConstantStringID': self.blockStatesConstantStringID,
+            'blockNBT': nbtlib.serialize_tag(self.blockNBT)
+        }
+        return result
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class PlaceBlockWithRuntimeId(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'placeBlockWithRuntimeId'
-        self.operationNumber: int = 33
-        self.runtimeId: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>I', self.runtimeId))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class PlaceRuntimeBlock(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceRuntimeBlock'
+        self.operationNumber: int = 32
+        self.runtimeId: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.runtimeId))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.5/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getString import getByte, getString
-
-
-class PlaceCommandBlockWithCommandBlockData(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceCommandBlockWithCommandBlockData'
-        self.operationNumber: int = 36
-        self.data: int = 0
-        self.mode: int = 0
-        self.command: str = ''
-        self.customName: str = ''
-        self.lastOutput: str = ''
-        self.tickdelay: int = 0
-        self.executeOnFirstTick: bool = True
-        self.trackOutput: bool = True
-        self.conditional: bool = False
-        self.needsRedstone: bool = False
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.data) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) + self.executeOnFirstTick.to_bytes(
-            length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.data = unpack('>H', getByte(buffer, 2))[0]
-        self.mode = unpack('>I', getByte(buffer, 4))[0]
-        self.command = getString(buffer)
-        self.customName = getString(buffer)
-        self.lastOutput = getString(buffer)
-        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
-        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
-        self.trackOutput = bool(getByte(buffer, 1)[0])
-        self.conditional = bool(getByte(buffer, 1)[0])
-        self.needsRedstone = bool(getByte(buffer, 1)[0])
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.data = jsonDict['data'] if 'data' in jsonDict else 0
-        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
-        self.command = jsonDict['command'] if 'command' in jsonDict else ''
-        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
-        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
-        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
-        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
-        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
-        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
-        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getString import getByte, getString
+
+
+class SetCommandBlockData(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'SetCommandBlockData'
+        self.operationNumber: int = 26
+        self.mode: int = 0
+        self.command: str = ''
+        self.customName: str = ''
+        self.lastOutput: str = ''
+        self.tickdelay: int = 0
+        self.executeOnFirstTick: bool = True
+        self.trackOutput: bool = True
+        self.conditional: bool = False
+        self.needsRedstone: bool = False
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) + self.executeOnFirstTick.to_bytes(
+            length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.mode = unpack('>I', getByte(buffer, 4))[0]
+        self.command = getString(buffer)
+        self.customName = getString(buffer)
+        self.lastOutput = getString(buffer)
+        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
+        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
+        self.trackOutput = bool(getByte(buffer, 1)[0])
+        self.conditional = bool(getByte(buffer, 1)[0])
+        self.needsRedstone = bool(getByte(buffer, 1)[0])
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
+        self.command = jsonDict['command'] if 'command' in jsonDict else ''
+        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
+        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
+        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
+        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
+        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
+        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
+        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from io import BytesIO
-from struct import pack, unpack
-from .structOfChest import ChestData
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class PlaceRuntimeBlockWithChestData(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceRuntimeBlockWithChestData'
-        self.operationNumber: int = 37
-        self.runtimeId: int = 0
-        self.slotCount: int = 0
-        self.data: ChestData = ChestData()
-
-    def Marshal(self, writer: BytesIO) -> None:
-        self.data.slotCount = self.slotCount
-        writer.write(pack('>H', self.runtimeId) +
-                     self.slotCount.to_bytes(length=1, byteorder='big', signed=False))
-        self.data.Marshal(writer)
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
-        self.slotCount = getByte(buffer, 1)[0]
-        self.data.slotCount = self.slotCount
-        self.data.UnMarshal(buffer)
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
-        self.slotCount = jsonDict['slotCount'] if 'slotCount' in jsonDict else 0
-        newChestData = ChestData()
-        if 'data' in jsonDict:
-            newChestData.Loads(jsonDict['data'])
-        self.data = newChestData
-
-    def Dumps(self) -> dict:
-        result: dict = {
-            'operationName': self.operationName,
-            'operationNumber': self.operationNumber,
-            'runtimeId': self.runtimeId,
-            'slotCount': self.slotCount,
-            'data': self.data.Dumps()
-        }
-        return result
+from io import BytesIO
+from struct import pack, unpack
+from .structOfChest import ChestData
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class PlaceRuntimeBlockWithChestDataAndUint32RuntimeID(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceRuntimeBlockWithChestDataAndUint32RuntimeID'
+        self.operationNumber: int = 38
+        self.runtimeId: int = 0
+        self.slotCount: int = 0
+        self.data: ChestData = ChestData()
+
+    def Marshal(self, writer: BytesIO) -> None:
+        self.data.slotCount = self.slotCount
+        writer.write(pack('>I', self.runtimeId) +
+                     self.slotCount.to_bytes(length=1, byteorder='big', signed=False))
+        self.data.Marshal(writer)
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
+        self.slotCount = getByte(buffer, 1)[0]
+        self.data.slotCount = self.slotCount
+        self.data.UnMarshal(buffer)
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
+        self.slotCount = jsonDict['slotCount'] if 'slotCount' in jsonDict else 0
+        newChestData = ChestData()
+        if 'data' in jsonDict:
+            newChestData.Loads(jsonDict['data'])
+        self.data = newChestData
+
+    def Dumps(self) -> dict:
+        result: dict = {
+            'operationName': self.operationName,
+            'operationNumber': self.operationNumber,
+            'runtimeId': self.runtimeId,
+            'slotCount': self.slotCount,
+            'data': self.data.Dumps()
+        }
+        return result
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getString import getByte, getString
-
-
-class PlaceRuntimeBlockWithCommandBlockData(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceRuntimeBlockWithCommandBlockData'
-        self.operationNumber: int = 34
-        self.runtimeId: int = 0
-        self.mode: int = 0
-        self.command: str = ''
-        self.customName: str = ''
-        self.lastOutput: str = ''
-        self.tickdelay: int = 0
-        self.executeOnFirstTick: bool = True
-        self.trackOutput: bool = True
-        self.conditional: bool = False
-        self.needsRedstone: bool = False
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.runtimeId) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
-                     self.executeOnFirstTick.to_bytes(length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
-        self.mode = unpack('>I', getByte(buffer, 4))[0]
-        self.command = getString(buffer)
-        self.customName = getString(buffer)
-        self.lastOutput = getString(buffer)
-        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
-        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
-        self.trackOutput = bool(getByte(buffer, 1)[0])
-        self.conditional = bool(getByte(buffer, 1)[0])
-        self.needsRedstone = bool(getByte(buffer, 1)[0])
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
-        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
-        self.command = jsonDict['command'] if 'command' in jsonDict else ''
-        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
-        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
-        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
-        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
-        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
-        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
-        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getString import getByte, getString
+
+
+class PlaceRuntimeBlockWithCommandBlockData(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceRuntimeBlockWithCommandBlockData'
+        self.operationNumber: int = 34
+        self.runtimeId: int = 0
+        self.mode: int = 0
+        self.command: str = ''
+        self.customName: str = ''
+        self.lastOutput: str = ''
+        self.tickdelay: int = 0
+        self.executeOnFirstTick: bool = True
+        self.trackOutput: bool = True
+        self.conditional: bool = False
+        self.needsRedstone: bool = False
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.runtimeId) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
+                     self.executeOnFirstTick.to_bytes(length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.runtimeId = unpack('>H', getByte(buffer, 2))[0]
+        self.mode = unpack('>I', getByte(buffer, 4))[0]
+        self.command = getString(buffer)
+        self.customName = getString(buffer)
+        self.lastOutput = getString(buffer)
+        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
+        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
+        self.trackOutput = bool(getByte(buffer, 1)[0])
+        self.conditional = bool(getByte(buffer, 1)[0])
+        self.needsRedstone = bool(getByte(buffer, 1)[0])
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
+        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
+        self.command = jsonDict['command'] if 'command' in jsonDict else ''
+        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
+        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
+        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
+        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
+        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
+        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
+        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.0.5/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getString import getByte, getString
-
-
-class PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID'
-        self.operationNumber: int = 35
-        self.runtimeId: int = 0
-        self.mode: int = 0
-        self.command: str = ''
-        self.customName: str = ''
-        self.lastOutput: str = ''
-        self.tickdelay: int = 0
-        self.executeOnFirstTick: bool = True
-        self.trackOutput: bool = True
-        self.conditional: bool = False
-        self.needsRedstone: bool = False
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>I', self.runtimeId) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) +
-                     self.executeOnFirstTick.to_bytes(length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.runtimeId = unpack('>I', getByte(buffer, 4))[0]
-        self.mode = unpack('>I', getByte(buffer, 4))[0]
-        self.command = getString(buffer)
-        self.customName = getString(buffer)
-        self.lastOutput = getString(buffer)
-        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
-        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
-        self.trackOutput = bool(getByte(buffer, 1)[0])
-        self.conditional = bool(getByte(buffer, 1)[0])
-        self.needsRedstone = bool(getByte(buffer, 1)[0])
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.runtimeId = jsonDict['runtimeId'] if 'runtimeId' in jsonDict else 0
-        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
-        self.command = jsonDict['command'] if 'command' in jsonDict else ''
-        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
-        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
-        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
-        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
-        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
-        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
-        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getString import getByte, getString
+
+
+class PlaceCommandBlockWithCommandBlockData(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'PlaceCommandBlockWithCommandBlockData'
+        self.operationNumber: int = 36
+        self.data: int = 0
+        self.mode: int = 0
+        self.command: str = ''
+        self.customName: str = ''
+        self.lastOutput: str = ''
+        self.tickdelay: int = 0
+        self.executeOnFirstTick: bool = True
+        self.trackOutput: bool = True
+        self.conditional: bool = False
+        self.needsRedstone: bool = False
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(pack('>H', self.data) + pack('>I', self.mode) + self.command.encode(encoding='utf-8') + b'\x00' + self.customName.encode(encoding='utf-8') + b'\x00' + self.lastOutput.encode(encoding='utf-8') + b'\x00' + pack('>I', self.tickdelay) + self.executeOnFirstTick.to_bytes(
+            length=1, byteorder='big', signed=False) + self.trackOutput.to_bytes(length=1, byteorder='big', signed=False) + self.conditional.to_bytes(length=1, byteorder='big', signed=False) + self.needsRedstone.to_bytes(length=1, byteorder='big', signed=False))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.data = unpack('>H', getByte(buffer, 2))[0]
+        self.mode = unpack('>I', getByte(buffer, 4))[0]
+        self.command = getString(buffer)
+        self.customName = getString(buffer)
+        self.lastOutput = getString(buffer)
+        self.tickdelay = unpack('>I', getByte(buffer, 4))[0]
+        self.executeOnFirstTick = bool(getByte(buffer, 1)[0])
+        self.trackOutput = bool(getByte(buffer, 1)[0])
+        self.conditional = bool(getByte(buffer, 1)[0])
+        self.needsRedstone = bool(getByte(buffer, 1)[0])
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.data = jsonDict['data'] if 'data' in jsonDict else 0
+        self.mode = jsonDict['mode'] if 'mode' in jsonDict else 0
+        self.command = jsonDict['command'] if 'command' in jsonDict else ''
+        self.customName = jsonDict['customName'] if 'customName' in jsonDict else ''
+        self.lastOutput = jsonDict['lastOutput'] if 'lastOutput' in jsonDict else ''
+        self.tickdelay = jsonDict['tickdelay'] if 'tickdelay' in jsonDict else 0
+        self.executeOnFirstTick = jsonDict['executeOnFirstTick'] if 'executeOnFirstTick' in jsonDict else True
+        self.trackOutput = jsonDict['trackOutput'] if 'trackOutput' in jsonDict else True
+        self.conditional = jsonDict['conditional'] if 'conditional' in jsonDict else False
+        self.needsRedstone = jsonDict['needsRedstone'] if 'needsRedstone' in jsonDict else False
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.0.5/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from io import BytesIO
-from ..General.GeneralClass import GeneralClass
-from ..utils.getByte import getByte
-
-
-class UseRuntimeIDPool(GeneralClass):
-    def __init__(self) -> None:
-        self.operationName: str = 'UseRuntimeIDPool'
-        self.operationNumber: int = 31
-        self.poolId: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(self.poolId.to_bytes(
-            length=1, byteorder='big', signed=False))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.poolId = getByte(buffer, 1)[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.poolId = jsonDict['poolId'] if 'poolId' in jsonDict else 0
+from io import BytesIO
+from ..General.GeneralClass import GeneralClass
+from ..utils.getByte import getByte
+
+
+class UseRuntimeIDPool(GeneralClass):
+    def __init__(self) -> None:
+        self.operationName: str = 'UseRuntimeIDPool'
+        self.operationNumber: int = 31
+        self.poolId: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(self.poolId.to_bytes(
+            length=1, byteorder='big', signed=False))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.poolId = getByte(buffer, 1)[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.poolId = jsonDict['poolId'] if 'poolId' in jsonDict else 0
```

### Comparing `BDXConverter-1.0.4/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.5/BDXConverter/Operation/structOfChest.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from io import BytesIO
-from struct import pack, unpack
-from ..General.GeneralClass import GeneralClass
-from ..utils.getString import getByte, getString
-
-
-class ChestSlot(GeneralClass):
-    """
-    Note: `ChestSlot` is not a operation
-    """
-
-    def __init__(self) -> None:
-        self.itemName: str = ''
-        self.count: int = 0
-        self.data: int = 0
-        self.slotID: int = 0
-
-    def Marshal(self, writer: BytesIO) -> None:
-        writer.write(self.itemName.encode(encoding='utf-8') + b'\x00' + self.count.to_bytes(length=1, byteorder='big',
-                     signed=False) + pack('>H', self.data) + self.slotID.to_bytes(length=1, byteorder='big', signed=False))
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.itemName = getString(buffer)
-        self.count = getByte(buffer, 1)[0]
-        self.data = unpack('>H', getByte(buffer, 2))[0]
-        self.slotID = getByte(buffer, 1)[0]
-
-    def Loads(self, jsonDict: dict) -> None:
-        self.itemName = jsonDict['itemName'] if 'itemName' in jsonDict else ''
-        self.count = jsonDict['count'] if 'count' in jsonDict else 0
-        self.data = jsonDict['data'] if 'data' in jsonDict else 0
-        self.slotID = jsonDict['slotID'] if 'slotID' in jsonDict else 0
-
-
-class ChestData(GeneralClass):
-    """
-    Note: `ChestData` is not a operation
-    """
-
-    def __init__(self) -> None:
-        self.slotCount: int = 0
-        self.chestData: list[ChestSlot] = []
-
-    def Marshal(self, writer: BytesIO) -> None:
-        for i in self.chestData:
-            i.Marshal(writer)
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        self.chestData = []
-        for _ in range(self.slotCount):
-            newSlot = ChestSlot()
-            newSlot.UnMarshal(buffer)
-            self.chestData.append(newSlot)
-
-    def Loads(self, jsonList: list[dict]) -> None:
-        self.slotCount = len(jsonList)
-        self.chestData = []
-        for i in jsonList:
-            newSlot = ChestSlot()
-            newSlot.Loads(i)
-            self.chestData.append(newSlot)
-        self.slotCount = len(self.chestData)
-
-    def Dumps(self) -> list[dict]:
-        result: list[dict] = []
-        for i in self.chestData:
-            result.append(i.Dumps())
-        return result
+from io import BytesIO
+from struct import pack, unpack
+from ..General.GeneralClass import GeneralClass
+from ..utils.getString import getByte, getString
+
+
+class ChestSlot(GeneralClass):
+    """
+    Note: `ChestSlot` is not a operation
+    """
+
+    def __init__(self) -> None:
+        self.itemName: str = ''
+        self.count: int = 0
+        self.data: int = 0
+        self.slotID: int = 0
+
+    def Marshal(self, writer: BytesIO) -> None:
+        writer.write(self.itemName.encode(encoding='utf-8') + b'\x00' + self.count.to_bytes(length=1, byteorder='big',
+                     signed=False) + pack('>H', self.data) + self.slotID.to_bytes(length=1, byteorder='big', signed=False))
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.itemName = getString(buffer)
+        self.count = getByte(buffer, 1)[0]
+        self.data = unpack('>H', getByte(buffer, 2))[0]
+        self.slotID = getByte(buffer, 1)[0]
+
+    def Loads(self, jsonDict: dict) -> None:
+        self.itemName = jsonDict['itemName'] if 'itemName' in jsonDict else ''
+        self.count = jsonDict['count'] if 'count' in jsonDict else 0
+        self.data = jsonDict['data'] if 'data' in jsonDict else 0
+        self.slotID = jsonDict['slotID'] if 'slotID' in jsonDict else 0
+
+
+class ChestData(GeneralClass):
+    """
+    Note: `ChestData` is not a operation
+    """
+
+    def __init__(self) -> None:
+        self.slotCount: int = 0
+        self.chestData: list[ChestSlot] = []
+
+    def Marshal(self, writer: BytesIO) -> None:
+        for i in self.chestData:
+            i.Marshal(writer)
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        self.chestData = []
+        for _ in range(self.slotCount):
+            newSlot = ChestSlot()
+            newSlot.UnMarshal(buffer)
+            self.chestData.append(newSlot)
+
+    def Loads(self, jsonList: list[dict]) -> None:
+        self.slotCount = len(jsonList)
+        self.chestData = []
+        for i in jsonList:
+            newSlot = ChestSlot()
+            newSlot.Loads(i)
+            self.chestData.append(newSlot)
+        self.slotCount = len(self.chestData)
+
+    def Dumps(self) -> list[dict]:
+        result: list[dict] = []
+        for i in self.chestData:
+            result.append(i.Dumps())
+        return result
```

### Comparing `BDXConverter-1.0.4/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.0.5/BDXConverter/utils/marshalNBT.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from io import BytesIO
-from struct import pack
-import nbtlib
-
-endian: str = '<'
-endianWord: str = 'little'
-
-
-def getValueType(value) -> bytes:
-    match type(value):
-        case nbtlib.tag.Byte:
-            return b'\x01'
-        case nbtlib.tag.Short:
-            return b'\x02'
-        case nbtlib.tag.Int:
-            return b'\x03'
-        case nbtlib.tag.Long:
-            return b'\x04'
-        case nbtlib.tag.Float:
-            return b'\x05'
-        case nbtlib.tag.Double:
-            return b'\x06'
-        case nbtlib.tag.ByteArray:
-            return b'\x07'
-        case nbtlib.tag.String:
-            return b'\x08'
-        case nbtlib.tag.Compound:
-            return b'\x0a'
-        case nbtlib.tag.IntArray:
-            return b'\x0b'
-        case nbtlib.tag.LongArray:
-            return b'\x0c'
-        case _:
-            return b'\x09'
-
-
-def marshalToName(writer: BytesIO, name: str) -> None:
-    encodeResult = name.encode(encoding='utf-8')
-    writer.write(pack(f'{endian}H', len(encodeResult)) + encodeResult)
-
-
-def marshalToValue(writer: BytesIO, value, valueType: int) -> None:
-    match valueType:
-        case 1:
-            writer.write(value.to_bytes(length=1, byteorder=endianWord, signed=True))
-        case 2:
-            writer.write(pack(f'{endian}h', value))
-        case 3:
-            writer.write(pack(f'{endian}i', value))
-        case 4:
-            writer.write(pack(f'{endian}q', value))
-        case 5:
-            writer.write(pack(f'{endian}f', value))
-        case 6:
-            writer.write(pack(f'{endian}d', value))
-        case 7 | 11 | 12:
-            marshalToArray(writer, value, valueType)
-        case 8:
-            marshalToName(writer, str(value))
-        case 9:
-            marshalToList(writer, value)
-        case 10:
-            marshalToCompound(writer, value)
-
-
-def marshalToArray(
-        writer: BytesIO,
-        value: nbtlib.tag.ByteArray | nbtlib.tag.IntArray | nbtlib.tag.LongArray,
-        valueType: int
-) -> None:
-    writer.write(pack(f'{endian}i', len(value)))
-    match valueType:
-        case 7:
-            writer.write(b''.join([pack(f'{endian}b', i) for i in value]))
-        case 11:
-            writer.write(b''.join([pack(f'{endian}i', i) for i in value]))
-        case 12:
-            writer.write(b''.join([pack(f'{endian}q', i) for i in value]))
-        case _:
-            raise TypeError
-
-
-def marshalToList(writer: BytesIO, value) -> None:
-    if len(value) > 0:
-        subValueType = getValueType(value[0])
-        writer.write(subValueType+pack(f'{endian}i', len(value)))
-        for i in value:
-            marshalToValue(writer, i, subValueType[0])
-    else:
-        writer.write(b'\x00' * 5)
-
-
-def marshalToCompound(writer: BytesIO, value: nbtlib.tag.Compound) -> None:
-    for i in value:
-        valueType = getValueType(value[i])
-        writer.write(valueType)
-        marshalToName(writer, i)
-        marshalToValue(writer, value[i], valueType[0])
-    writer.write(b'\x00')
-
-
-def MarshalPythonNBTObjectToWriter(writer: BytesIO, value, name: str) -> None:
-    valueType = getValueType(value)
-    writer.write(valueType)
-    marshalToName(writer, name)
-    marshalToValue(writer, value, valueType[0])
+from io import BytesIO
+from struct import pack
+import nbtlib
+
+endian: str = '<'
+endianWord: str = 'little'
+
+
+def getValueType(value) -> bytes:
+    match type(value):
+        case nbtlib.tag.Byte:
+            return b'\x01'
+        case nbtlib.tag.Short:
+            return b'\x02'
+        case nbtlib.tag.Int:
+            return b'\x03'
+        case nbtlib.tag.Long:
+            return b'\x04'
+        case nbtlib.tag.Float:
+            return b'\x05'
+        case nbtlib.tag.Double:
+            return b'\x06'
+        case nbtlib.tag.ByteArray:
+            return b'\x07'
+        case nbtlib.tag.String:
+            return b'\x08'
+        case nbtlib.tag.Compound:
+            return b'\x0a'
+        case nbtlib.tag.IntArray:
+            return b'\x0b'
+        case nbtlib.tag.LongArray:
+            return b'\x0c'
+        case _:
+            return b'\x09'
+
+
+def marshalToName(writer: BytesIO, name: str) -> None:
+    encodeResult = name.encode(encoding='utf-8')
+    writer.write(pack(f'{endian}H', len(encodeResult)) + encodeResult)
+
+
+def marshalToValue(writer: BytesIO, value, valueType: int) -> None:
+    match valueType:
+        case 1:
+            writer.write(value.to_bytes(length=1, byteorder=endianWord, signed=True))
+        case 2:
+            writer.write(pack(f'{endian}h', value))
+        case 3:
+            writer.write(pack(f'{endian}i', value))
+        case 4:
+            writer.write(pack(f'{endian}q', value))
+        case 5:
+            writer.write(pack(f'{endian}f', value))
+        case 6:
+            writer.write(pack(f'{endian}d', value))
+        case 7 | 11 | 12:
+            marshalToArray(writer, value, valueType)
+        case 8:
+            marshalToName(writer, str(value))
+        case 9:
+            marshalToList(writer, value)
+        case 10:
+            marshalToCompound(writer, value)
+
+
+def marshalToArray(
+        writer: BytesIO,
+        value: nbtlib.tag.ByteArray | nbtlib.tag.IntArray | nbtlib.tag.LongArray,
+        valueType: int
+) -> None:
+    writer.write(pack(f'{endian}i', len(value)))
+    match valueType:
+        case 7:
+            writer.write(b''.join([pack(f'{endian}b', i) for i in value]))
+        case 11:
+            writer.write(b''.join([pack(f'{endian}i', i) for i in value]))
+        case 12:
+            writer.write(b''.join([pack(f'{endian}q', i) for i in value]))
+        case _:
+            raise TypeError
+
+
+def marshalToList(writer: BytesIO, value) -> None:
+    if len(value) > 0:
+        subValueType = getValueType(value[0])
+        writer.write(subValueType+pack(f'{endian}i', len(value)))
+        for i in value:
+            marshalToValue(writer, i, subValueType[0])
+    else:
+        writer.write(b'\x00' * 5)
+
+
+def marshalToCompound(writer: BytesIO, value: nbtlib.tag.Compound) -> None:
+    for i in value:
+        valueType = getValueType(value[i])
+        writer.write(valueType)
+        marshalToName(writer, i)
+        marshalToValue(writer, value[i], valueType[0])
+    writer.write(b'\x00')
+
+
+def MarshalPythonNBTObjectToWriter(writer: BytesIO, value, name: str) -> None:
+    valueType = getValueType(value)
+    writer.write(valueType)
+    marshalToName(writer, name)
+    marshalToValue(writer, value, valueType[0])
```

### Comparing `BDXConverter-1.0.4/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.0.5/BDXConverter/utils/unmarshalNBT.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from io import BytesIO
-from struct import unpack
-from .getByte import getByte
-import nbtlib
-
-endian: str = '<'
-
-
-class getValueError(Exception):
-    def __init__(self, errorOccurredPosition: int):
-        Exception.__init__(
-            self, f'failed to parse value, and the error occurred at position {errorOccurredPosition}')
-
-
-class unexpectedError(Exception):
-    def __init__(self, value: int):
-        Exception.__init__(self, f'unexpected number {value}')
-
-
-def getName(buffer: BytesIO) -> str:
-    keyLength = unpack(f'{endian}H', getByte(buffer, 2))[0]
-    return getByte(buffer, keyLength).decode(encoding='utf-8')
-
-
-def getValue(buffer: BytesIO, valueType: int) -> nbtlib.tag.Byte | nbtlib.tag.Short | nbtlib.tag.Int | nbtlib.tag.Long | nbtlib.tag.Float | nbtlib.tag.Double | nbtlib.tag.ByteArray | nbtlib.tag.String | nbtlib.tag.List | nbtlib.tag.Compound | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
-    match valueType:
-        case 1:
-            return nbtlib.tag.Byte(unpack(f'{endian}b', getByte(buffer, 1))[0])
-        case 2:
-            return nbtlib.tag.Short(unpack(f'{endian}h', getByte(buffer, 2))[0])
-        case 3:
-            return nbtlib.tag.Int(unpack(f'{endian}i', getByte(buffer, 4))[0])
-        case 4:
-            return nbtlib.tag.Long(unpack(f'{endian}q', getByte(buffer, 8))[0])
-        case 5:
-            return nbtlib.tag.Float(unpack(f'{endian}f', getByte(buffer, 4))[0])
-        case 6:
-            return nbtlib.tag.Double(unpack(f'{endian}d', getByte(buffer, 8))[0])
-        case 7 | 11 | 12:
-            return getArray(buffer, valueType)
-        case 8:
-            return nbtlib.tag.String(getName(buffer))
-        case 9:
-            return getList(buffer)
-        case 10:
-            return getCompound(buffer)
-        case _:
-            raise getValueError(buffer.seek(0, 1))
-
-
-def getArray(buffer: BytesIO, valueType: int) -> nbtlib.tag.ByteArray | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
-    arrayLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
-    match valueType:
-        case 7:
-            return nbtlib.tag.ByteArray([unpack(f'{endian}b', getByte(buffer, 1))[0] for _ in range(arrayLength)])
-        case 11:
-            return nbtlib.tag.IntArray([unpack(f'{endian}i', getByte(buffer, 4))[0] for _ in range(arrayLength)])
-        case 12:
-            return nbtlib.tag.LongArray([unpack(f'{endian}q', getByte(buffer, 8))[0] for _ in range(arrayLength)])
-        case _:
-            raise unexpectedError(valueType)
-
-
-def getList(buffer: BytesIO) -> nbtlib.tag.List:
-    valueType = getByte(buffer, 1)[0]
-    listLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
-    return nbtlib.tag.List([getValue(buffer, valueType) for _ in range(listLength)])
-
-
-def getCompound(buffer: BytesIO) -> nbtlib.tag.Compound:
-    result: dict = {}
-    while True:
-        nextBuffer = getByte(buffer, 1)
-        if nextBuffer == b'\x00':
-            return nbtlib.tag.Compound(result)
-        # if meet TAG_End
-        buffer.seek(-1, 1)
-        # correct the pointer
-        valueType = getByte(buffer, 1)[0]
-        name = getName(buffer)
-        result[name] = getValue(buffer, valueType)
-        # set values
-
-
-def UnMarshalBufferToPythonNBTObject(buffer: BytesIO) -> tuple[nbtlib.tag.Byte | nbtlib.tag.Short | nbtlib.tag.Int | nbtlib.tag.Long | nbtlib.tag.Float | nbtlib.tag.Double | nbtlib.tag.ByteArray | nbtlib.tag.String | nbtlib.tag.List | nbtlib.tag.Compound | nbtlib.tag.IntArray | nbtlib.tag.LongArray, str]:
-    valueType = getByte(buffer, 1)[0]
-    name = getName(buffer)
-    return getValue(buffer, valueType), name
+from io import BytesIO
+from struct import unpack
+from .getByte import getByte
+import nbtlib
+
+endian: str = '<'
+
+
+class getValueError(Exception):
+    def __init__(self, errorOccurredPosition: int):
+        Exception.__init__(
+            self, f'failed to parse value, and the error occurred at position {errorOccurredPosition}')
+
+
+class unexpectedError(Exception):
+    def __init__(self, value: int):
+        Exception.__init__(self, f'unexpected number {value}')
+
+
+def getName(buffer: BytesIO) -> str:
+    keyLength = unpack(f'{endian}H', getByte(buffer, 2))[0]
+    return getByte(buffer, keyLength).decode(encoding='utf-8')
+
+
+def getValue(buffer: BytesIO, valueType: int) -> nbtlib.tag.Byte | nbtlib.tag.Short | nbtlib.tag.Int | nbtlib.tag.Long | nbtlib.tag.Float | nbtlib.tag.Double | nbtlib.tag.ByteArray | nbtlib.tag.String | nbtlib.tag.List | nbtlib.tag.Compound | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
+    match valueType:
+        case 1:
+            return nbtlib.tag.Byte(unpack(f'{endian}b', getByte(buffer, 1))[0])
+        case 2:
+            return nbtlib.tag.Short(unpack(f'{endian}h', getByte(buffer, 2))[0])
+        case 3:
+            return nbtlib.tag.Int(unpack(f'{endian}i', getByte(buffer, 4))[0])
+        case 4:
+            return nbtlib.tag.Long(unpack(f'{endian}q', getByte(buffer, 8))[0])
+        case 5:
+            return nbtlib.tag.Float(unpack(f'{endian}f', getByte(buffer, 4))[0])
+        case 6:
+            return nbtlib.tag.Double(unpack(f'{endian}d', getByte(buffer, 8))[0])
+        case 7 | 11 | 12:
+            return getArray(buffer, valueType)
+        case 8:
+            return nbtlib.tag.String(getName(buffer))
+        case 9:
+            return getList(buffer)
+        case 10:
+            return getCompound(buffer)
+        case _:
+            raise getValueError(buffer.seek(0, 1))
+
+
+def getArray(buffer: BytesIO, valueType: int) -> nbtlib.tag.ByteArray | nbtlib.tag.IntArray | nbtlib.tag.LongArray:
+    arrayLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
+    match valueType:
+        case 7:
+            return nbtlib.tag.ByteArray([unpack(f'{endian}b', getByte(buffer, 1))[0] for _ in range(arrayLength)])
+        case 11:
+            return nbtlib.tag.IntArray([unpack(f'{endian}i', getByte(buffer, 4))[0] for _ in range(arrayLength)])
+        case 12:
+            return nbtlib.tag.LongArray([unpack(f'{endian}q', getByte(buffer, 8))[0] for _ in range(arrayLength)])
+        case _:
+            raise unexpectedError(valueType)
+
+
+def getList(buffer: BytesIO) -> nbtlib.tag.List:
+    valueType = getByte(buffer, 1)[0]
+    listLength = unpack(f'{endian}i', getByte(buffer, 4))[0]
+    return nbtlib.tag.List([getValue(buffer, valueType) for _ in range(listLength)])
+
+
+def getCompound(buffer: BytesIO) -> nbtlib.tag.Compound:
+    result: dict = {}
+    while True:
+        nextBuffer = getByte(buffer, 1)
+        if nextBuffer == b'\x00':
+            return nbtlib.tag.Compound(result)
+        # if meet TAG_End
+        buffer.seek(-1, 1)
+        # correct the pointer
+        valueType = getByte(buffer, 1)[0]
+        name = getName(buffer)
+        result[name] = getValue(buffer, valueType)
+        # set values
+
+
+def UnMarshalBufferToPythonNBTObject(buffer: BytesIO) -> tuple[nbtlib.tag.Byte | nbtlib.tag.Short | nbtlib.tag.Int | nbtlib.tag.Long | nbtlib.tag.Float | nbtlib.tag.Double | nbtlib.tag.ByteArray | nbtlib.tag.String | nbtlib.tag.List | nbtlib.tag.Compound | nbtlib.tag.IntArray | nbtlib.tag.LongArray, str]:
+    valueType = getByte(buffer, 1)[0]
+    name = getName(buffer)
+    return getValue(buffer, valueType), name
```

### Comparing `BDXConverter-1.0.4/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.5/BDXConverter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-Metadata-Version: 2.1
-Name: BDXConverter
-Version: 1.0.4
-Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
-Home-page: https://github.com/TriM-Organization/BDXConverter
-Author: Minecraft Muti-Media Organization
-Author-email: TriM-Organization@hotmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">BDX Converter</h1>
-<h3 align="center">一个免费开源的 BDX 文件解析器</h3>
-<br/>
-<p align="center">
-<img src="https://forthebadge.com/images/badges/built-with-love.svg">
-<p>
-
-[GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
-[python]: https://img.shields.io/badge/python-3.11-AB70FF?style=for-the-badge
-[release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
-[license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
-
-[![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
-[![][python]](https://www.python.org/)<br/>
-[![][license]](LICENSE)<br/>
-
-
-
-
-
-# `BDX Converter`
-`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
-
-# 快速上手
-您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
-
-# 项目依赖
-本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
-
-```
-pip install brotli
-pip install nbtlib
-```
-
-# 项目特性
-您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
-
-实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
-
-```python
-class GeneralClass:
-    """
-    Any Operation eration of the BDX file will inherit this class
-    """
-
-    def __init__(self) -> None:
-        self.operationNumber: int
-        self.operationName: str
-
-    def Marshal(self, writer: BytesIO) -> None:
-        """
-        Marshal GeneralClass into the writer
-        """
-        ...
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        """
-        Unmarshal the buffer(io object) into GeneralClass
-        """
-        ...
-
-    def Loads(self, jsonDict: dict) -> None:
-        """
-        Convert jsonDict:dict into GeneralClass
-        """
-        ...
-
-    def Dumps(self) -> dict:
-        """
-        Convert GeneralClass into basic dictionary
-        """
-        return self.__dict__
-```
-
-因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
-而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
-
-目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
-
-# 待办列表
-- [ ] `API` 文档
-- [ ] 支持与 `签名` 有关的功能
-- [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
-- [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
-
-# 其他
-本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
+Metadata-Version: 2.1
+Name: BDXConverter
+Version: 1.0.5
+Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
+Home-page: https://github.com/TriM-Organization/BDXConverter
+Author: Minecraft Muti-Media Organization
+Author-email: TriM-Organization@hotmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">BDX Converter</h1>
+<h3 align="center">一个免费开源的 BDX 文件解析器</h3>
+<br/>
+<p align="center">
+<img src="https://forthebadge.com/images/badges/built-with-love.svg">
+<p>
+
+[GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
+[python]: https://img.shields.io/badge/python-3.11-AB70FF?style=for-the-badge
+[release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
+[license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
+
+[![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
+[![][python]](https://www.python.org/)<br/>
+[![][license]](LICENSE)<br/>
+
+
+
+
+
+# `BDX Converter`
+`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+
+# 快速上手
+您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+
+# 项目依赖
+本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
+
+```
+pip install brotli
+pip install nbtlib
+```
+
+# 项目特性
+您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
+
+实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
+
+```python
+class GeneralClass:
+    """
+    Any Operation eration of the BDX file will inherit this class
+    """
+
+    def __init__(self) -> None:
+        self.operationNumber: int
+        self.operationName: str
+
+    def Marshal(self, writer: BytesIO) -> None:
+        """
+        Marshal GeneralClass into the writer
+        """
+        ...
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        """
+        Unmarshal the buffer(io object) into GeneralClass
+        """
+        ...
+
+    def Loads(self, jsonDict: dict) -> None:
+        """
+        Convert jsonDict:dict into GeneralClass
+        """
+        ...
+
+    def Dumps(self) -> dict:
+        """
+        Convert GeneralClass into basic dictionary
+        """
+        return self.__dict__
+```
+
+因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
+而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
+
+目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
+
+# 待办列表
+- [ ] `API` 文档
+- [ ] 支持与 `签名` 有关的功能
+- [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
+- [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
+
+# 其他
+本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
```

### Comparing `BDXConverter-1.0.4/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.5/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.4/LICENSE` & `BDXConverter-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Minecraft Muti-Media Organization
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Minecraft Muti-Media Organization
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `BDXConverter-1.0.4/PKG-INFO` & `BDXConverter-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-Metadata-Version: 2.1
-Name: BDXConverter
-Version: 1.0.4
-Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
-Home-page: https://github.com/TriM-Organization/BDXConverter
-Author: Minecraft Muti-Media Organization
-Author-email: TriM-Organization@hotmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">BDX Converter</h1>
-<h3 align="center">一个免费开源的 BDX 文件解析器</h3>
-<br/>
-<p align="center">
-<img src="https://forthebadge.com/images/badges/built-with-love.svg">
-<p>
-
-[GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
-[python]: https://img.shields.io/badge/python-3.11-AB70FF?style=for-the-badge
-[release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
-[license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
-
-[![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
-[![][python]](https://www.python.org/)<br/>
-[![][license]](LICENSE)<br/>
-
-
-
-
-
-# `BDX Converter`
-`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
-
-# 快速上手
-您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
-
-# 项目依赖
-本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
-
-```
-pip install brotli
-pip install nbtlib
-```
-
-# 项目特性
-您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
-
-实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
-
-```python
-class GeneralClass:
-    """
-    Any Operation eration of the BDX file will inherit this class
-    """
-
-    def __init__(self) -> None:
-        self.operationNumber: int
-        self.operationName: str
-
-    def Marshal(self, writer: BytesIO) -> None:
-        """
-        Marshal GeneralClass into the writer
-        """
-        ...
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        """
-        Unmarshal the buffer(io object) into GeneralClass
-        """
-        ...
-
-    def Loads(self, jsonDict: dict) -> None:
-        """
-        Convert jsonDict:dict into GeneralClass
-        """
-        ...
-
-    def Dumps(self) -> dict:
-        """
-        Convert GeneralClass into basic dictionary
-        """
-        return self.__dict__
-```
-
-因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
-而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
-
-目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
-
-# 待办列表
-- [ ] `API` 文档
-- [ ] 支持与 `签名` 有关的功能
-- [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
-- [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
-
-# 其他
-本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
+Metadata-Version: 2.1
+Name: BDXConverter
+Version: 1.0.5
+Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
+Home-page: https://github.com/TriM-Organization/BDXConverter
+Author: Minecraft Muti-Media Organization
+Author-email: TriM-Organization@hotmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">BDX Converter</h1>
+<h3 align="center">一个免费开源的 BDX 文件解析器</h3>
+<br/>
+<p align="center">
+<img src="https://forthebadge.com/images/badges/built-with-love.svg">
+<p>
+
+[GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
+[python]: https://img.shields.io/badge/python-3.11-AB70FF?style=for-the-badge
+[release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
+[license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
+
+[![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
+[![][python]](https://www.python.org/)<br/>
+[![][license]](LICENSE)<br/>
+
+
+
+
+
+# `BDX Converter`
+`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+
+# 快速上手
+您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+
+# 项目依赖
+本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
+
+```
+pip install brotli
+pip install nbtlib
+```
+
+# 项目特性
+您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
+
+实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
+
+```python
+class GeneralClass:
+    """
+    Any Operation eration of the BDX file will inherit this class
+    """
+
+    def __init__(self) -> None:
+        self.operationNumber: int
+        self.operationName: str
+
+    def Marshal(self, writer: BytesIO) -> None:
+        """
+        Marshal GeneralClass into the writer
+        """
+        ...
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        """
+        Unmarshal the buffer(io object) into GeneralClass
+        """
+        ...
+
+    def Loads(self, jsonDict: dict) -> None:
+        """
+        Convert jsonDict:dict into GeneralClass
+        """
+        ...
+
+    def Dumps(self) -> dict:
+        """
+        Convert GeneralClass into basic dictionary
+        """
+        return self.__dict__
+```
+
+因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
+而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
+
+目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
+
+# 待办列表
+- [ ] `API` 文档
+- [ ] 支持与 `签名` 有关的功能
+- [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
+- [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
+
+# 其他
+本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
```

### Comparing `BDXConverter-1.0.4/README.md` & `BDXConverter-1.0.5/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-<h1 align="center">BDX Converter</h1>
-<h3 align="center">一个免费开源的 BDX 文件解析器</h3>
-<br/>
-<p align="center">
-<img src="https://forthebadge.com/images/badges/built-with-love.svg">
-<p>
-
-[GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
-[python]: https://img.shields.io/badge/python-3.11-AB70FF?style=for-the-badge
-[release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
-[license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
-
-[![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
-[![][python]](https://www.python.org/)<br/>
-[![][license]](LICENSE)<br/>
-
-
-
-
-
-# `BDX Converter`
-`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
-
-# 快速上手
-您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
-
-# 项目依赖
-本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
-
-```
-pip install brotli
-pip install nbtlib
-```
-
-# 项目特性
-您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
-
-实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
-
-```python
-class GeneralClass:
-    """
-    Any Operation eration of the BDX file will inherit this class
-    """
-
-    def __init__(self) -> None:
-        self.operationNumber: int
-        self.operationName: str
-
-    def Marshal(self, writer: BytesIO) -> None:
-        """
-        Marshal GeneralClass into the writer
-        """
-        ...
-
-    def UnMarshal(self, buffer: BytesIO) -> None:
-        """
-        Unmarshal the buffer(io object) into GeneralClass
-        """
-        ...
-
-    def Loads(self, jsonDict: dict) -> None:
-        """
-        Convert jsonDict:dict into GeneralClass
-        """
-        ...
-
-    def Dumps(self) -> dict:
-        """
-        Convert GeneralClass into basic dictionary
-        """
-        return self.__dict__
-```
-
-因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
-而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
-
-目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
-
-# 待办列表
-- [ ] `API` 文档
-- [ ] 支持与 `签名` 有关的功能
-- [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
-- [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
-
-# 其他
-本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
+<h1 align="center">BDX Converter</h1>
+<h3 align="center">一个免费开源的 BDX 文件解析器</h3>
+<br/>
+<p align="center">
+<img src="https://forthebadge.com/images/badges/built-with-love.svg">
+<p>
+
+[GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
+[python]: https://img.shields.io/badge/python-3.11-AB70FF?style=for-the-badge
+[release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
+[license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
+
+[![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
+[![][python]](https://www.python.org/)<br/>
+[![][license]](LICENSE)<br/>
+
+
+
+
+
+# `BDX Converter`
+`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+
+# 快速上手
+您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+
+# 项目依赖
+本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
+
+```
+pip install brotli
+pip install nbtlib
+```
+
+# 项目特性
+您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
+
+实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
+
+```python
+class GeneralClass:
+    """
+    Any Operation eration of the BDX file will inherit this class
+    """
+
+    def __init__(self) -> None:
+        self.operationNumber: int
+        self.operationName: str
+
+    def Marshal(self, writer: BytesIO) -> None:
+        """
+        Marshal GeneralClass into the writer
+        """
+        ...
+
+    def UnMarshal(self, buffer: BytesIO) -> None:
+        """
+        Unmarshal the buffer(io object) into GeneralClass
+        """
+        ...
+
+    def Loads(self, jsonDict: dict) -> None:
+        """
+        Convert jsonDict:dict into GeneralClass
+        """
+        ...
+
+    def Dumps(self) -> dict:
+        """
+        Convert GeneralClass into basic dictionary
+        """
+        return self.__dict__
+```
+
+因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
+而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
+
+目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
+
+# 待办列表
+- [ ] `API` 文档
+- [ ] 支持与 `签名` 有关的功能
+- [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
+- [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
+
+# 其他
+本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
```

### Comparing `BDXConverter-1.0.4/setup.py` & `BDXConverter-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import setuptools
-
-with open("requirements.txt", "r+", encoding="utf-8") as file:
-    dependences = file.read().strip().split("\n")
-file.close()
-
-with open("README.md", "r+", encoding='utf-8') as file:
-    long_description = file.read()
-file.close()
-
-setuptools.setup(
-    name="BDXConverter",
-    version="1.0.4",
-    author="Minecraft Muti-Media Organization",
-    author_email="TriM-Organization@hotmail.com",
-    description="A code library to marshal, unmarshal, visual and reverse visualization of BDX files",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/TriM-Organization/BDXConverter",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=dependences,
-    python_requires='>=3.11',
-)
+import setuptools
+
+with open("requirements.txt", "r+", encoding="utf-8") as file:
+    dependences = file.read().strip().split("\n")
+file.close()
+
+with open("README.md", "r+", encoding='utf-8') as file:
+    long_description = file.read()
+file.close()
+
+setuptools.setup(
+    name="BDXConverter",
+    version="1.0.5",
+    author="Minecraft Muti-Media Organization",
+    author_email="TriM-Organization@hotmail.com",
+    description="A code library to marshal, unmarshal, visual and reverse visualization of BDX files",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/TriM-Organization/BDXConverter",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=dependences,
+    python_requires='>=3.11',
+)
```

