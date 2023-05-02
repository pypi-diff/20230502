# Comparing `tmp/sw_mc_lib-0.2.1.tar.gz` & `tmp/sw_mc_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_mc_lib-0.2.1.tar", last modified: Tue May  2 19:37:10 2023, max compression
+gzip compressed data, was "sw_mc_lib-0.3.0.tar", last modified: Tue May  2 21:42:27 2023, max compression
```

## Comparing `sw_mc_lib-0.2.1.tar` & `sw_mc_lib-0.3.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 19:37:10.566519 sw_mc_lib-0.2.1/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1073 2023-04-21 16:19:23.000000 sw_mc_lib-0.2.1/LICENSE
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      967 2023-05-02 19:37:10.566519 sw_mc_lib-0.2.1/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       49 2023-05-01 20:30:36.000000 sw_mc_lib-0.2.1/README.md
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1200 2023-05-02 19:34:46.000000 sw_mc_lib-0.2.1/pyproject.toml
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      163 2023-05-02 19:37:10.567519 sw_mc_lib-0.2.1/setup.cfg
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 19:37:10.544517 sw_mc_lib-0.2.1/sw_mc_lib/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     9879 2023-05-01 19:50:53.000000 sw_mc_lib-0.2.1/sw_mc_lib/Component.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 19:37:10.564519 sw_mc_lib-0.2.1/sw_mc_lib/Components/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/AND.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1246 2023-05-01 15:24:25.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Abs.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Add.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1753 2023-05-01 15:25:02.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/ArithmeticFunction1In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2046 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/ArithmeticFunction3In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2792 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/ArithmeticFunction8In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1789 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/AudioSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2080 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Blinker.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2127 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/BooleanFunction4In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2741 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/BooleanFunction8In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1997 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Capacitor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1752 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Clamp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1507 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeBinaryToNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1920 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeReadBoolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1912 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeReadNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1825 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3339 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeWriteBoolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3324 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeWriteNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1528 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/ConstantNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1013 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/ConstantOn.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1230 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Delta.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1351 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Divide.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1350 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Equal.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1397 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/GreaterThan.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1412 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/JKFlipFlop.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1370 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/LessThan.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2329 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/LuaScript.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2268 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/MemoryRegister.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1331 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Modulo.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1361 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Multiply.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/NAND.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/NOR.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1164 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/NOT.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1500 2023-05-01 15:24:44.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/NumberToCompositeBinary.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1777 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/NumericalJunction.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1821 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/NumericalSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1306 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/OR.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2969 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PIDController.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2454 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PIDControllerAdvanced.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3112 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyDropdown.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1696 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2444 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertySlider.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1648 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyText.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2009 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyToggle.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1657 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Pulse.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1273 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/PushToToggle.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1384 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/SRLatch.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 19:37:10.565519 sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1339 2023-05-01 12:54:18.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/MinMaxComponent.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1105 2023-05-01 12:54:18.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/ResetComponent.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1106 2023-05-01 12:54:18.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/ValueComponent.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-04-21 11:51:32.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1371 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Subtract.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1870 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/Threshold.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1929 2023-05-01 15:23:45.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerRTF.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1924 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerRTO.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1733 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerTOF.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1724 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerTON.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2542 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/TooltipBoolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2212 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/TooltipNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2928 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/UpDownCounter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1789 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/VideoSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/XOR.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2218 2023-04-30 21:48:55.000000 sw_mc_lib-0.2.1/sw_mc_lib/Components/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1173 2023-05-01 15:20:10.000000 sw_mc_lib-0.2.1/sw_mc_lib/Input.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     4058 2023-05-01 19:13:34.000000 sw_mc_lib-0.2.1/sw_mc_lib/Microcontroller.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3231 2023-05-01 15:37:20.000000 sw_mc_lib-0.2.1/sw_mc_lib/Node.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1478 2023-05-01 19:13:58.000000 sw_mc_lib-0.2.1/sw_mc_lib/NumberProperty.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      874 2023-05-01 15:39:10.000000 sw_mc_lib-0.2.1/sw_mc_lib/Position.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2586 2023-05-01 12:32:04.000000 sw_mc_lib-0.2.1/sw_mc_lib/Types.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1159 2023-05-01 19:14:23.000000 sw_mc_lib-0.2.1/sw_mc_lib/XMLElement.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2795 2023-05-01 19:48:50.000000 sw_mc_lib-0.2.1/sw_mc_lib/XMLFormatter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     5953 2023-05-01 19:43:01.000000 sw_mc_lib-0.2.1/sw_mc_lib/XMLParser.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      424 2023-05-02 19:31:42.000000 sw_mc_lib-0.2.1/sw_mc_lib/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1576 2023-05-01 19:14:13.000000 sw_mc_lib-0.2.1/sw_mc_lib/util.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 19:37:10.545518 sw_mc_lib-0.2.1/sw_mc_lib.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      967 2023-05-02 19:37:10.000000 sw_mc_lib-0.2.1/sw_mc_lib.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2965 2023-05-02 19:37:10.000000 sw_mc_lib-0.2.1/sw_mc_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-02 19:37:10.000000 sw_mc_lib-0.2.1/sw_mc_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       69 2023-05-02 19:37:10.000000 sw_mc_lib-0.2.1/sw_mc_lib.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       10 2023-05-02 19:37:10.000000 sw_mc_lib-0.2.1/sw_mc_lib.egg-info/top_level.txt
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 19:37:10.566519 sw_mc_lib-0.2.1/test/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     4924 2023-05-01 15:40:04.000000 sw_mc_lib-0.2.1/test/test_component.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1148 2023-04-30 06:28:11.000000 sw_mc_lib-0.2.1/test/test_input.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2028 2023-04-30 15:23:37.000000 sw_mc_lib-0.2.1/test/test_number_property.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1071 2023-05-01 15:40:04.000000 sw_mc_lib-0.2.1/test/test_position.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2968 2023-04-30 15:17:44.000000 sw_mc_lib-0.2.1/test/test_xml_formatter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1851 2023-05-01 15:31:58.000000 sw_mc_lib-0.2.1/test/test_xml_parser.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 21:42:27.874149 sw_mc_lib-0.3.0/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1073 2023-04-21 16:19:23.000000 sw_mc_lib-0.3.0/LICENSE
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1863 2023-05-02 21:42:27.875149 sw_mc_lib-0.3.0/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      945 2023-05-02 20:04:04.000000 sw_mc_lib-0.3.0/README.md
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1200 2023-05-02 21:39:09.000000 sw_mc_lib-0.3.0/pyproject.toml
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      163 2023-05-02 21:42:27.875149 sw_mc_lib-0.3.0/setup.cfg
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 21:42:27.856148 sw_mc_lib-0.3.0/sw_mc_lib/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     9879 2023-05-01 19:50:53.000000 sw_mc_lib-0.3.0/sw_mc_lib/Component.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 21:42:27.868149 sw_mc_lib-0.3.0/sw_mc_lib/Components/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/AND.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1246 2023-05-01 15:24:25.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Abs.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Add.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1753 2023-05-01 15:25:02.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/ArithmeticFunction1In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2046 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/ArithmeticFunction3In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2792 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/ArithmeticFunction8In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1789 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/AudioSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2080 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Blinker.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2127 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/BooleanFunction4In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2741 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/BooleanFunction8In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1997 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Capacitor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1752 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Clamp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1507 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeBinaryToNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1920 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeReadBoolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1912 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeReadNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1825 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3339 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeWriteBoolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3324 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeWriteNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1528 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/ConstantNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1013 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/ConstantOn.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1230 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Delta.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1351 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Divide.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1350 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Equal.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1397 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/GreaterThan.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1412 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/JKFlipFlop.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1370 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/LessThan.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2329 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/LuaScript.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2268 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/MemoryRegister.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1331 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Modulo.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1361 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Multiply.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/NAND.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/NOR.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1164 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/NOT.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1500 2023-05-01 15:24:44.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/NumberToCompositeBinary.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1777 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/NumericalJunction.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1821 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/NumericalSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1306 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/OR.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2969 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PIDController.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2454 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PIDControllerAdvanced.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3112 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyDropdown.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1696 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2444 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertySlider.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1648 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyText.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2009 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyToggle.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1657 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Pulse.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1273 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/PushToToggle.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1384 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/SRLatch.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 21:42:27.869149 sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1339 2023-05-01 12:54:18.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/MinMaxComponent.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1105 2023-05-01 12:54:18.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/ResetComponent.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1106 2023-05-01 12:54:18.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/ValueComponent.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-04-21 11:51:32.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1371 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Subtract.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1870 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/Threshold.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1929 2023-05-01 15:23:45.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerRTF.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1924 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerRTO.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1733 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerTOF.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1724 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerTON.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2542 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/TooltipBoolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2212 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/TooltipNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2928 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/UpDownCounter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1789 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/VideoSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/XOR.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2218 2023-04-30 21:48:55.000000 sw_mc_lib-0.3.0/sw_mc_lib/Components/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1173 2023-05-01 15:20:10.000000 sw_mc_lib-0.3.0/sw_mc_lib/Input.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4805 2023-05-02 21:00:36.000000 sw_mc_lib-0.3.0/sw_mc_lib/Microcontroller.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3231 2023-05-01 15:37:20.000000 sw_mc_lib-0.3.0/sw_mc_lib/Node.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1478 2023-05-01 19:13:58.000000 sw_mc_lib-0.3.0/sw_mc_lib/NumberProperty.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      874 2023-05-01 15:39:10.000000 sw_mc_lib-0.3.0/sw_mc_lib/Position.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2586 2023-05-01 12:32:04.000000 sw_mc_lib-0.3.0/sw_mc_lib/Types.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1159 2023-05-01 19:14:23.000000 sw_mc_lib-0.3.0/sw_mc_lib/XMLElement.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2795 2023-05-01 19:48:50.000000 sw_mc_lib-0.3.0/sw_mc_lib/XMLFormatter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     5953 2023-05-01 19:43:01.000000 sw_mc_lib-0.3.0/sw_mc_lib/XMLParser.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      346 2023-05-02 21:38:15.000000 sw_mc_lib-0.3.0/sw_mc_lib/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1576 2023-05-01 19:14:13.000000 sw_mc_lib-0.3.0/sw_mc_lib/util.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 21:42:27.856148 sw_mc_lib-0.3.0/sw_mc_lib.egg-info/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1863 2023-05-02 21:42:27.000000 sw_mc_lib-0.3.0/sw_mc_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2965 2023-05-02 21:42:27.000000 sw_mc_lib-0.3.0/sw_mc_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-02 21:42:27.000000 sw_mc_lib-0.3.0/sw_mc_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       69 2023-05-02 21:42:27.000000 sw_mc_lib-0.3.0/sw_mc_lib.egg-info/requires.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       10 2023-05-02 21:42:27.000000 sw_mc_lib-0.3.0/sw_mc_lib.egg-info/top_level.txt
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-02 21:42:27.874149 sw_mc_lib-0.3.0/test/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4924 2023-05-01 15:40:04.000000 sw_mc_lib-0.3.0/test/test_component.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1148 2023-04-30 06:28:11.000000 sw_mc_lib-0.3.0/test/test_input.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2028 2023-04-30 15:23:37.000000 sw_mc_lib-0.3.0/test/test_number_property.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1071 2023-05-01 15:40:04.000000 sw_mc_lib-0.3.0/test/test_position.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2968 2023-04-30 15:17:44.000000 sw_mc_lib-0.3.0/test/test_xml_formatter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1851 2023-05-01 15:31:58.000000 sw_mc_lib-0.3.0/test/test_xml_parser.py
```

### Comparing `sw_mc_lib-0.2.1/LICENSE` & `sw_mc_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/pyproject.toml` & `sw_mc_lib-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sw_mc_lib"
-version = "0.2.1"
+version = "0.3.0"
 description = "Library for interaction with Stormworks Microcontrollers"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["stormworks", "lib", "microcontroller"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
```

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Component.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Component.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/AND.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/AND.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Abs.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Abs.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Add.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Add.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/ArithmeticFunction1In.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/ArithmeticFunction1In.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/ArithmeticFunction3In.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/ArithmeticFunction3In.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/ArithmeticFunction8In.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/ArithmeticFunction8In.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/AudioSwitchbox.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/AudioSwitchbox.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Blinker.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Blinker.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/BooleanFunction4In.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/BooleanFunction4In.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/BooleanFunction8In.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/BooleanFunction8In.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Capacitor.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Capacitor.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Clamp.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Clamp.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeBinaryToNumber.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeBinaryToNumber.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeReadBoolean.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeReadBoolean.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeReadNumber.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeReadNumber.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeSwitchbox.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeSwitchbox.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeWriteBoolean.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeWriteBoolean.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/CompositeWriteNumber.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/CompositeWriteNumber.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/ConstantNumber.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/ConstantNumber.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/ConstantOn.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/ConstantOn.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Delta.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Delta.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Divide.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Divide.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Equal.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Equal.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/GreaterThan.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/JKFlipFlop.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/JKFlipFlop.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/LessThan.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/LessThan.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/LuaScript.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/LuaScript.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/MemoryRegister.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/MemoryRegister.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Modulo.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Modulo.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Multiply.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Multiply.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/NAND.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/NAND.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/NOR.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/NOR.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/NOT.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/NOT.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/NumberToCompositeBinary.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/NumberToCompositeBinary.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/NumericalJunction.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/NumericalJunction.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/NumericalSwitchbox.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/NumericalSwitchbox.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/OR.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/OR.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PIDController.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PIDController.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PIDControllerAdvanced.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PIDControllerAdvanced.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyDropdown.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyDropdown.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyNumber.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyNumber.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertySlider.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertySlider.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyText.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyText.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PropertyToggle.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PropertyToggle.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Pulse.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Pulse.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/PushToToggle.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/PushToToggle.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/SRLatch.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/SRLatch.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/MinMaxComponent.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/MinMaxComponent.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/ResetComponent.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/ResetComponent.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/SubTypes/ValueComponent.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/SubTypes/ValueComponent.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Subtract.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Subtract.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/Threshold.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/Threshold.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerRTF.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerRTF.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerRTO.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerRTO.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerTOF.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerTOF.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/TimerTON.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/TimerTON.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/TooltipBoolean.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/TooltipBoolean.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/TooltipNumber.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/TooltipNumber.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/UpDownCounter.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/UpDownCounter.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/VideoSwitchbox.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/VideoSwitchbox.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/XOR.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/XOR.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Components/__init__.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Components/__init__.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Input.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Input.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Microcontroller.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Microcontroller.py`

 * *Files 15% similar despite different names*

```diff
@@ -77,14 +77,35 @@
             "width": str(self.width),
             "length": str(self.length),
             "id_counter": str(self.id_counter),
             "id_counter_node": str(self.node_counter),
         }
         return XMLParserElement("microprocessor", attributes, [nodes_elem, group_elem])
 
+    def add_new_component(self, component: Component) -> None:
+        """
+        Adds a new :class:`Component <sw_mc_lib.Component.Component>`. Sets the right `component_id`.
+
+        :param component: The component to add, `component_id` may be any value
+        :return: None
+        """
+        component.component_id = self.id_counter + 1
+        self.components.append(component)
+
+    def add_new_node(self, node: Node) -> None:
+        """
+        Adds a new :class:`Node <sw_mc_lib.Node.Node>`. Sets the right `component_id` and `node_id`.
+
+        :param node: The Node to add
+        :return: None
+        """
+        node.component_id = self.id_counter + 1
+        node.node_id = self.node_counter + 1
+        self.nodes.append(node)
+
     @property
     def id_counter(self) -> int:
         """
         Stormworks internal counter of what the largest component_id is.
 
         :return: The currently largest component_id
         """
```

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Node.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Node.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/NumberProperty.py` & `sw_mc_lib-0.3.0/sw_mc_lib/NumberProperty.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Position.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Position.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/Types.py` & `sw_mc_lib-0.3.0/sw_mc_lib/Types.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/XMLElement.py` & `sw_mc_lib-0.3.0/sw_mc_lib/XMLElement.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/XMLFormatter.py` & `sw_mc_lib-0.3.0/sw_mc_lib/XMLFormatter.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/XMLParser.py` & `sw_mc_lib-0.3.0/sw_mc_lib/XMLParser.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib/util.py` & `sw_mc_lib-0.3.0/sw_mc_lib/util.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/sw_mc_lib.egg-info/SOURCES.txt` & `sw_mc_lib-0.3.0/sw_mc_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/test/test_component.py` & `sw_mc_lib-0.3.0/test/test_component.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/test/test_input.py` & `sw_mc_lib-0.3.0/test/test_input.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/test/test_number_property.py` & `sw_mc_lib-0.3.0/test/test_number_property.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/test/test_position.py` & `sw_mc_lib-0.3.0/test/test_position.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/test/test_xml_formatter.py` & `sw_mc_lib-0.3.0/test/test_xml_formatter.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.2.1/test/test_xml_parser.py` & `sw_mc_lib-0.3.0/test/test_xml_parser.py`

 * *Files identical despite different names*

