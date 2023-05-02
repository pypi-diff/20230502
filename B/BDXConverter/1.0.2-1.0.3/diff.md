# Comparing `tmp/BDXConverter-1.0.2.tar.gz` & `tmp/BDXConverter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.2.tar", last modified: Tue May  2 03:12:45 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.3.tar", last modified: Tue May  2 03:46:48 2023, max compression
```

## Comparing `BDXConverter-1.0.2.tar` & `BDXConverter-1.0.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 03:12:45.783554 BDXConverter-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-02 03:12:45.405914 BDXConverter-1.0.2/BDXConverter/
-drwxrwxrwx   0        0        0        0 2023-05-02 03:12:45.447915 BDXConverter-1.0.2/BDXConverter/Converter/
--rw-rw-rw-   0        0        0      808 2023-05-02 01:50:46.000000 BDXConverter-1.0.2/BDXConverter/Converter/ConvertErrorDefine.py
--rw-rw-rw-   0        0        0     4722 2023-05-02 01:53:27.000000 BDXConverter-1.0.2/BDXConverter/Converter/Converter.py
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.2/BDXConverter/Converter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:12:45.470562 BDXConverter-1.0.2/BDXConverter/General/
--rw-rw-rw-   0        0        0      792 2023-05-02 01:50:46.000000 BDXConverter-1.0.2/BDXConverter/General/GeneralClass.py
--rw-rw-rw-   0        0        0     4167 2023-05-02 01:53:47.000000 BDXConverter-1.0.2/BDXConverter/General/Pool.py
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.2/BDXConverter/General/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:12:45.738770 BDXConverter-1.0.2/BDXConverter/Operation/
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:19.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt16XValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:24.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt16YValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:27.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt16ZValue.py
--rw-rw-rw-   0        0        0      665 2023-05-02 01:56:31.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt16ZValue0.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:38.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt32XValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:44.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt32YValue.py
--rw-rw-rw-   0        0        0      664 2023-05-02 01:56:49.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt32ZValue.py
--rw-rw-rw-   0        0        0      666 2023-05-02 01:56:53.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt32ZValue0.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:56:01.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt8XValue.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:56:09.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt8YValue.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:56:13.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddInt8ZValue.py
--rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddXValue.py
--rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddYValue.py
--rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddZValue.py
--rw-rw-rw-   0        0        0      206 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/AddZValue0.py
--rw-rw-rw-   0        0        0     1273 2023-05-02 01:57:01.000000 BDXConverter-1.0.2/BDXConverter/Operation/AssignDebugData.py
--rw-rw-rw-   0        0        0      707 2023-05-02 01:57:14.000000 BDXConverter-1.0.2/BDXConverter/Operation/CreateConstantString.py
--rw-rw-rw-   0        0        0      192 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/NOP.py
--rw-rw-rw-   0        0        0      979 2023-05-02 01:57:21.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlock.py
--rw-rw-rw-   0        0        0     1131 2023-05-02 01:57:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-rw-rw-   0        0        0     1098 2023-05-02 01:57:36.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-rw-rw-   0        0        0     2082 2023-05-02 02:00:06.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-rw-rw-   0        0        0     3132 2023-05-02 01:58:03.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-rw-rw-   0        0        0     2163 2023-05-02 01:58:14.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-rw-rw-   0        0        0      706 2023-05-02 01:58:19.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-rw-rw-   0        0        0     2830 2023-05-02 01:58:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-rw-rw-   0        0        0      694 2023-05-02 01:58:29.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-rw-rw-   0        0        0     1689 2023-05-02 01:58:56.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-rw-rw-   0        0        0     1725 2023-05-02 01:59:13.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-rw-rw-   0        0        0     2868 2023-05-02 01:59:21.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-rw-rw-   0        0        0     2904 2023-05-02 01:59:28.000000 BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-rw-rw-   0        0        0     2618 2023-05-02 01:59:35.000000 BDXConverter-1.0.2/BDXConverter/Operation/SetCommandBlockData.py
--rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/SubtractXValue.py
--rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/SubtractYValue.py
--rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/SubtractZValue.py
--rw-rw-rw-   0        0        0      495 2023-05-02 01:55:26.000000 BDXConverter-1.0.2/BDXConverter/Operation/Terminate.py
--rw-rw-rw-   0        0        0      679 2023-05-02 01:55:44.000000 BDXConverter-1.0.2/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.2/BDXConverter/Operation/__init__.py
--rw-rw-rw-   0        0        0     2322 2023-05-02 01:59:44.000000 BDXConverter-1.0.2/BDXConverter/Operation/structOfChest.py
--rw-rw-rw-   0        0        0       48 2023-05-02 03:10:12.000000 BDXConverter-1.0.2/BDXConverter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:12:45.770547 BDXConverter-1.0.2/BDXConverter/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.2/BDXConverter/utils/__init__.py
--rw-rw-rw-   0        0        0      194 2023-05-02 01:50:46.000000 BDXConverter-1.0.2/BDXConverter/utils/getByte.py
--rw-rw-rw-   0        0        0      337 2023-05-02 01:54:14.000000 BDXConverter-1.0.2/BDXConverter/utils/getString.py
--rw-rw-rw-   0        0        0     3310 2023-05-02 01:50:46.000000 BDXConverter-1.0.2/BDXConverter/utils/marshalNBT.py
--rw-rw-rw-   0        0        0     3676 2023-05-02 01:54:31.000000 BDXConverter-1.0.2/BDXConverter/utils/unmarshalNBT.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:12:45.432916 BDXConverter-1.0.2/BDXConverter.egg-info/
--rw-rw-rw-   0        0        0     3621 2023-05-02 03:12:45.000000 BDXConverter-1.0.2/BDXConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2385 2023-05-02 03:12:45.000000 BDXConverter-1.0.2/BDXConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 03:12:45.000000 BDXConverter-1.0.2/BDXConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-02 03:12:45.000000 BDXConverter-1.0.2/BDXConverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 03:12:45.000000 BDXConverter-1.0.2/BDXConverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2023-05-01 15:39:04.000000 BDXConverter-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3621 2023-05-02 03:12:45.773543 BDXConverter-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2023-05-02 02:16:54.000000 BDXConverter-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 03:12:45.783554 BDXConverter-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-05-02 03:12:15.000000 BDXConverter-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:46:48.943096 BDXConverter-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-02 03:46:48.635901 BDXConverter-1.0.3/BDXConverter/
+drwxrwxrwx   0        0        0        0 2023-05-02 03:46:48.675382 BDXConverter-1.0.3/BDXConverter/Converter/
+-rw-rw-rw-   0        0        0      808 2023-05-02 01:50:46.000000 BDXConverter-1.0.3/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-rw-rw-   0        0        0     4722 2023-05-02 01:53:27.000000 BDXConverter-1.0.3/BDXConverter/Converter/Converter.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.3/BDXConverter/Converter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:46:48.686356 BDXConverter-1.0.3/BDXConverter/General/
+-rw-rw-rw-   0        0        0      792 2023-05-02 01:50:46.000000 BDXConverter-1.0.3/BDXConverter/General/GeneralClass.py
+-rw-rw-rw-   0        0        0     4167 2023-05-02 01:53:47.000000 BDXConverter-1.0.3/BDXConverter/General/Pool.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.3/BDXConverter/General/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:46:48.891555 BDXConverter-1.0.3/BDXConverter/Operation/
+-rw-rw-rw-   0        0        0      664 2023-05-02 01:56:19.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt16XValue.py
+-rw-rw-rw-   0        0        0      664 2023-05-02 01:56:24.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt16YValue.py
+-rw-rw-rw-   0        0        0      664 2023-05-02 01:56:27.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt16ZValue.py
+-rw-rw-rw-   0        0        0      665 2023-05-02 01:56:31.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-rw-rw-   0        0        0      664 2023-05-02 01:56:38.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt32XValue.py
+-rw-rw-rw-   0        0        0      664 2023-05-02 01:56:44.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt32YValue.py
+-rw-rw-rw-   0        0        0      664 2023-05-02 01:56:49.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt32ZValue.py
+-rw-rw-rw-   0        0        0      666 2023-05-02 01:56:53.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-rw-rw-   0        0        0      707 2023-05-02 01:56:01.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt8XValue.py
+-rw-rw-rw-   0        0        0      707 2023-05-02 01:56:09.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt8YValue.py
+-rw-rw-rw-   0        0        0      707 2023-05-02 01:56:13.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddInt8ZValue.py
+-rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddXValue.py
+-rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddYValue.py
+-rw-rw-rw-   0        0        0      205 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddZValue.py
+-rw-rw-rw-   0        0        0      206 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/AddZValue0.py
+-rw-rw-rw-   0        0        0     1273 2023-05-02 01:57:01.000000 BDXConverter-1.0.3/BDXConverter/Operation/AssignDebugData.py
+-rw-rw-rw-   0        0        0      707 2023-05-02 01:57:14.000000 BDXConverter-1.0.3/BDXConverter/Operation/CreateConstantString.py
+-rw-rw-rw-   0        0        0      192 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/NOP.py
+-rw-rw-rw-   0        0        0      979 2023-05-02 01:57:21.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlock.py
+-rw-rw-rw-   0        0        0     1131 2023-05-02 01:57:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-rw-rw-   0        0        0     1098 2023-05-02 01:57:36.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-rw-rw-   0        0        0     2082 2023-05-02 02:00:06.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-rw-rw-   0        0        0     3132 2023-05-02 01:58:03.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-rw-rw-   0        0        0     2163 2023-05-02 01:58:14.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-rw-rw-   0        0        0      706 2023-05-02 01:58:19.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-rw-rw-   0        0        0     2830 2023-05-02 01:58:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-rw-rw-   0        0        0      694 2023-05-02 01:58:29.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-rw-rw-   0        0        0     1689 2023-05-02 01:58:56.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-rw-rw-   0        0        0     1725 2023-05-02 01:59:13.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-rw-rw-   0        0        0     2868 2023-05-02 01:59:21.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-rw-rw-   0        0        0     2904 2023-05-02 01:59:28.000000 BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-rw-rw-   0        0        0     2618 2023-05-02 01:59:35.000000 BDXConverter-1.0.3/BDXConverter/Operation/SetCommandBlockData.py
+-rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/SubtractXValue.py
+-rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/SubtractYValue.py
+-rw-rw-rw-   0        0        0      215 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/SubtractZValue.py
+-rw-rw-rw-   0        0        0      495 2023-05-02 01:55:26.000000 BDXConverter-1.0.3/BDXConverter/Operation/Terminate.py
+-rw-rw-rw-   0        0        0      679 2023-05-02 01:55:44.000000 BDXConverter-1.0.3/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.3/BDXConverter/Operation/__init__.py
+-rw-rw-rw-   0        0        0     2322 2023-05-02 01:59:44.000000 BDXConverter-1.0.3/BDXConverter/Operation/structOfChest.py
+-rw-rw-rw-   0        0        0       48 2023-05-02 03:10:12.000000 BDXConverter-1.0.3/BDXConverter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:46:48.914584 BDXConverter-1.0.3/BDXConverter/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 02:02:21.000000 BDXConverter-1.0.3/BDXConverter/utils/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-05-02 01:50:46.000000 BDXConverter-1.0.3/BDXConverter/utils/getByte.py
+-rw-rw-rw-   0        0        0      337 2023-05-02 01:54:14.000000 BDXConverter-1.0.3/BDXConverter/utils/getString.py
+-rw-rw-rw-   0        0        0     3310 2023-05-02 01:50:46.000000 BDXConverter-1.0.3/BDXConverter/utils/marshalNBT.py
+-rw-rw-rw-   0        0        0     3676 2023-05-02 01:54:31.000000 BDXConverter-1.0.3/BDXConverter/utils/unmarshalNBT.py
+drwxrwxrwx   0        0        0        0 2023-05-02 03:46:48.660381 BDXConverter-1.0.3/BDXConverter.egg-info/
+-rw-rw-rw-   0        0        0     3864 2023-05-02 03:46:48.000000 BDXConverter-1.0.3/BDXConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2385 2023-05-02 03:46:48.000000 BDXConverter-1.0.3/BDXConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 03:46:48.000000 BDXConverter-1.0.3/BDXConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-02 03:46:48.000000 BDXConverter-1.0.3/BDXConverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 03:46:48.000000 BDXConverter-1.0.3/BDXConverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2023-05-01 15:39:04.000000 BDXConverter-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3864 2023-05-02 03:46:48.937573 BDXConverter-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3321 2023-05-02 03:27:13.000000 BDXConverter-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 03:46:48.943096 BDXConverter-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-05-02 03:46:42.000000 BDXConverter-1.0.3/setup.py
```

### Comparing `BDXConverter-1.0.2/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.3/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.3/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.0.3/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/General/Pool.py` & `BDXConverter-1.0.3/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.3/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.0.3/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.0.3/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.0.3/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.3/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.0.3/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.0.3/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: BDXConverter
-Version: 1.0.2
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
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -32,26 +18,26 @@
 
 
 
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 # 快速上手
-您可以利用 [`Converter/Converter.py`](./Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+您可以利用 [`BDXConverter/Converter/Converter.py`]([./BDXConverter/Converter/Converter.py](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py)) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 # 项目依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 ```
 
 # 项目特性
-您可以从 [`General/Pool.py`](./General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
+您可以从 [`BDXConverter/General/Pool.py`]([./BDXConverter/General/Pool.py](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py)) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
     Any Operation eration of the BDX file will inherit this class
```

### Comparing `BDXConverter-1.0.2/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.3/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/LICENSE` & `BDXConverter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.2/PKG-INFO` & `BDXConverter-1.0.3/BDXConverter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,26 +32,26 @@
 
 
 
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 # 快速上手
-您可以利用 [`Converter/Converter.py`](./Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+您可以利用 [`BDXConverter/Converter/Converter.py`]([./BDXConverter/Converter/Converter.py](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py)) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 # 项目依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 ```
 
 # 项目特性
-您可以从 [`General/Pool.py`](./General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
+您可以从 [`BDXConverter/General/Pool.py`]([./BDXConverter/General/Pool.py](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py)) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
     Any Operation eration of the BDX file will inherit this class
```

### Comparing `BDXConverter-1.0.2/README.md` & `BDXConverter-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: BDXConverter
+Version: 1.0.3
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
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -18,26 +32,26 @@
 
 
 
 # `BDX Converter`
 `BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 # 快速上手
-您可以利用 [`Converter/Converter.py`](./Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
+您可以利用 [`BDXConverter/Converter/Converter.py`]([./BDXConverter/Converter/Converter.py](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py)) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
 
 # 项目依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 ```
 
 # 项目特性
-您可以从 [`General/Pool.py`](./General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
+您可以从 [`BDXConverter/General/Pool.py`]([./BDXConverter/General/Pool.py](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py)) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
     Any Operation eration of the BDX file will inherit this class
```

### Comparing `BDXConverter-1.0.2/setup.py` & `BDXConverter-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r+", encoding='utf-8') as file:
     long_description = file.read()
 file.close()
 
 setuptools.setup(
     name="BDXConverter",
-    version="1.0.2",
+    version="1.0.3",
     author="Minecraft Muti-Media Organization",
     author_email="TriM-Organization@hotmail.com",
     description="A code library to marshal, unmarshal, visual and reverse visualization of BDX files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TriM-Organization/BDXConverter",
     packages=setuptools.find_packages(),
```

