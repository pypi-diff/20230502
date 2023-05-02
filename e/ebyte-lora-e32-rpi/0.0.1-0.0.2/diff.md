# Comparing `tmp/ebyte-lora-e32-rpi-0.0.1.tar.gz` & `tmp/ebyte-lora-e32-rpi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebyte-lora-e32-rpi-0.0.1.tar", last modified: Sat Apr 22 20:50:08 2023, max compression
+gzip compressed data, was "ebyte-lora-e32-rpi-0.0.2.tar", last modified: Tue May  2 07:07:14 2023, max compression
```

## Comparing `ebyte-lora-e32-rpi-0.0.1.tar` & `ebyte-lora-e32-rpi-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 20:50:08.719153 ebyte-lora-e32-rpi-0.0.1/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e32-rpi-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0    20950 2023-04-22 20:50:08.720152 ebyte-lora-e32-rpi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    18029 2023-04-21 13:15:41.000000 ebyte-lora-e32-rpi-0.0.1/README.md
--rw-rw-rw-   0        0        0     1521 2023-04-22 20:49:39.000000 ebyte-lora-e32-rpi-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      871 2023-04-22 20:50:08.722159 ebyte-lora-e32-rpi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1920 2023-04-22 20:31:11.000000 ebyte-lora-e32-rpi-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 20:50:08.698157 ebyte-lora-e32-rpi-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-22 20:50:08.718154 ebyte-lora-e32-rpi-0.0.1/src/ebyte_lora_e32_rpi.egg-info/
--rw-rw-rw-   0        0        0    20950 2023-04-22 20:50:08.000000 ebyte-lora-e32-rpi-0.0.1/src/ebyte_lora_e32_rpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-22 20:50:08.000000 ebyte-lora-e32-rpi-0.0.1/src/ebyte_lora_e32_rpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 20:50:08.000000 ebyte-lora-e32-rpi-0.0.1/src/ebyte_lora_e32_rpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-22 20:50:08.000000 ebyte-lora-e32-rpi-0.0.1/src/ebyte_lora_e32_rpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-04-22 20:50:08.000000 ebyte-lora-e32-rpi-0.0.1/src/ebyte_lora_e32_rpi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25651 2023-04-21 10:59:11.000000 ebyte-lora-e32-rpi-0.0.1/src/lora_e32.py
--rw-rw-rw-   0        0        0    13039 2023-04-18 14:05:09.000000 ebyte-lora-e32-rpi-0.0.1/src/lora_e32_constants.py
--rw-rw-rw-   0        0        0     2914 2023-03-21 16:15:50.000000 ebyte-lora-e32-rpi-0.0.1/src/lora_e32_operation_constant.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:07:14.054812 ebyte-lora-e32-rpi-0.0.2/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e32-rpi-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0    21000 2023-05-02 07:07:14.054812 ebyte-lora-e32-rpi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18079 2023-05-02 07:02:32.000000 ebyte-lora-e32-rpi-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1521 2023-05-02 07:03:00.000000 ebyte-lora-e32-rpi-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      871 2023-05-02 07:07:14.056813 ebyte-lora-e32-rpi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1920 2023-05-02 07:03:00.000000 ebyte-lora-e32-rpi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:07:14.028814 ebyte-lora-e32-rpi-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 07:07:14.052814 ebyte-lora-e32-rpi-0.0.2/src/ebyte_lora_e32_rpi.egg-info/
+-rw-rw-rw-   0        0        0    21000 2023-05-02 07:07:13.000000 ebyte-lora-e32-rpi-0.0.2/src/ebyte_lora_e32_rpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-02 07:07:14.000000 ebyte-lora-e32-rpi-0.0.2/src/ebyte_lora_e32_rpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 07:07:13.000000 ebyte-lora-e32-rpi-0.0.2/src/ebyte_lora_e32_rpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-02 07:07:13.000000 ebyte-lora-e32-rpi-0.0.2/src/ebyte_lora_e32_rpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-05-02 07:07:13.000000 ebyte-lora-e32-rpi-0.0.2/src/ebyte_lora_e32_rpi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25651 2023-05-02 07:03:00.000000 ebyte-lora-e32-rpi-0.0.2/src/lora_e32.py
+-rw-rw-rw-   0        0        0    13039 2023-05-02 07:01:37.000000 ebyte-lora-e32-rpi-0.0.2/src/lora_e32_constants.py
+-rw-rw-rw-   0        0        0     2914 2023-03-21 16:15:50.000000 ebyte-lora-e32-rpi-0.0.2/src/lora_e32_operation_constant.py
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/LICENSE.md` & `ebyte-lora-e32-rpi-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ebyte-lora-e32-rpi-0.0.1/PKG-INFO` & `ebyte-lora-e32-rpi-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e32-rpi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ebyte E32 LoRa raspberrypi library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.
 Home-page: https://github.com/xreef/EByte_LoRa_E32_raspberrypi_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -71,14 +71,15 @@
 3.  [LoRa E32 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2019/10/29/lora-e32-device-for-arduino-esp32-or-esp8266-configuration-part-3/)
 4.  [LoRa E32 device for Arduino, esp32 or esp8266: fixed transmission](https://www.mischianti.org/2019/11/10/lora-e32-device-for-arduino-esp32-or-esp8266-fixed-transmission-part-4/)
 5.  [LoRa E32 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2019/12/03/lora-e32-device-for-arduino-esp32-or-esp8266-power-saving-and-sending-structured-data-part-5/)
 6.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) the microcontroller and Arduino shield](https://www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/)
 7.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-wemos-d1-mini-shield-part-7/)
 
 ### Changelog
+ - 2023-05-02 0.0.2 Fix 900MHz devices frequency
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e32-rpi Version: 0.0.1 Summary: Ebyte
+Metadata-Version: 2.1 Name: ebyte-lora-e32-rpi Version: 0.0.2 Summary: Ebyte
 E32 LoRa raspberrypi library device very cheap and very long range (from 3Km to
 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino,
 esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276. Home-page: https://
 github.com/xreef/EByte_LoRa_E32_raspberrypi_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -53,21 +53,22 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-03-21 0.0.1 Fully functional
-library ### Library usage Here an example of constructor, you must pass the
-UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
-### Installation To install the library execute the following command: ```bash
-pip install ebyte-lora-e32-rpi ``` #### Initialization ```python from lora_e32
-import LoRaE32 import serial loraSerial = serial.Serial('/dev/serial0') #,
-baudrate=9600, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE,
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-05-02 0.0.2 Fix 900MHz
+devices frequency - 2023-03-21 0.0.1 Fully functional library ### Library usage
+Here an example of constructor, you must pass the UART interface and (if you
+want, but It's reccomended) the AUX pin, M0 and M1. ### Installation To install
+the library execute the following command: ```bash pip install ebyte-lora-e32-
+rpi ``` #### Initialization ```python from lora_e32 import LoRaE32 import
+serial loraSerial = serial.Serial('/dev/serial0') #, baudrate=9600,
+parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE,
 bytesize=serial.EIGHTBITS) lora = LoRaE32('433T20D', loraSerial, aux_pin=18,
 m0_pin=23, m1_pin=24) ``` #### Start the module transmission ```python code =
 lora.begin() print(ResponseStatusCode.get_description(code)) ``` #### Get
 Configuration ```python from lora_e32 import LoRaE32, print_configuration,
 Configuration from lora_e32_operation_constant import ResponseStatusCode code,
 configuration = lora.get_configuration() print
 (ResponseStatusCode.get_description(code)) print_configuration(configuration)
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/README.md` & `ebyte-lora-e32-rpi-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 3.  [LoRa E32 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2019/10/29/lora-e32-device-for-arduino-esp32-or-esp8266-configuration-part-3/)
 4.  [LoRa E32 device for Arduino, esp32 or esp8266: fixed transmission](https://www.mischianti.org/2019/11/10/lora-e32-device-for-arduino-esp32-or-esp8266-fixed-transmission-part-4/)
 5.  [LoRa E32 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2019/12/03/lora-e32-device-for-arduino-esp32-or-esp8266-power-saving-and-sending-structured-data-part-5/)
 6.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) the microcontroller and Arduino shield](https://www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/)
 7.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-wemos-d1-mini-shield-part-7/)
 
 ### Changelog
+ - 2023-05-02 0.0.2 Fix 900MHz devices frequency
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
 ### Installation
```

#### html2text {}

```diff
@@ -18,21 +18,22 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-03-21 0.0.1 Fully functional
-library ### Library usage Here an example of constructor, you must pass the
-UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
-### Installation To install the library execute the following command: ```bash
-pip install ebyte-lora-e32-rpi ``` #### Initialization ```python from lora_e32
-import LoRaE32 import serial loraSerial = serial.Serial('/dev/serial0') #,
-baudrate=9600, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE,
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-05-02 0.0.2 Fix 900MHz
+devices frequency - 2023-03-21 0.0.1 Fully functional library ### Library usage
+Here an example of constructor, you must pass the UART interface and (if you
+want, but It's reccomended) the AUX pin, M0 and M1. ### Installation To install
+the library execute the following command: ```bash pip install ebyte-lora-e32-
+rpi ``` #### Initialization ```python from lora_e32 import LoRaE32 import
+serial loraSerial = serial.Serial('/dev/serial0') #, baudrate=9600,
+parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE,
 bytesize=serial.EIGHTBITS) lora = LoRaE32('433T20D', loraSerial, aux_pin=18,
 m0_pin=23, m1_pin=24) ``` #### Start the module transmission ```python code =
 lora.begin() print(ResponseStatusCode.get_description(code)) ``` #### Get
 Configuration ```python from lora_e32 import LoRaE32, print_configuration,
 Configuration from lora_e32_operation_constant import ResponseStatusCode code,
 configuration = lora.get_configuration() print
 (ResponseStatusCode.get_description(code)) print_configuration(configuration)
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/pyproject.toml` & `ebyte-lora-e32-rpi-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2265 6279 7465 2d6c 6f72 612d 6533  = "ebyte-lora-e3
 00000020: 322d 7270 6922 0d0a 7665 7273 696f 6e20  2-rpi"..version 
-00000030: 3d20 2230 2e30 2e31 220d 0a61 7574 686f  = "0.0.1"..autho
+00000030: 3d20 2230 2e30 2e32 220d 0a61 7574 686f  = "0.0.2"..autho
 00000040: 7273 203d 205b 0d0a 2020 7b20 6e61 6d65  rs = [..  { name
 00000050: 3d22 5265 6e7a 6f20 4d69 7363 6869 616e  ="Renzo Mischian
 00000060: 7469 222c 2065 6d61 696c 3d22 7265 6e7a  ti", email="renz
 00000070: 6f40 6d69 7363 6869 616e 7469 2e6f 7267  o@mischianti.org
 00000080: 2220 7d2c 0d0a 5d0d 0a6d 6169 6e74 6169  " },..]..maintai
 00000090: 6e65 7273 203d 205b 0d0a 2020 7b20 6e61  ners = [..  { na
 000000a0: 6d65 3d22 5265 6e7a 6f20 4d69 7363 6869  me="Renzo Mischi
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/setup.cfg` & `ebyte-lora-e32-rpi-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6279 7465 2d6c 6f72 612d 6533   = ebyte-lora-e3
 00000020: 322d 7270 690d 0a76 6572 7369 6f6e 203d  2-rpi..version =
-00000030: 2030 2e30 2e31 0d0a 6175 7468 6f72 203d   0.0.1..author =
+00000030: 2030 2e30 2e32 0d0a 6175 7468 6f72 203d   0.0.2..author =
 00000040: 2052 656e 7a6f 204d 6973 6368 6961 6e74   Renzo Mischiant
 00000050: 690d 0a64 6573 6372 6970 7469 6f6e 203d  i..description =
 00000060: 2022 4562 7974 6520 4533 3220 4c6f 5261   "Ebyte E32 LoRa
 00000070: 2072 6173 7062 6572 7279 7069 206c 6962   raspberrypi lib
 00000080: 7261 7279 2064 6576 6963 6520 7665 7279  rary device very
 00000090: 2063 6865 6170 2061 6e64 2076 6572 7920   cheap and very 
 000000a0: 6c6f 6e67 2072 616e 6765 2028 6672 6f6d  long range (from
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/setup.py` & `ebyte-lora-e32-rpi-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="ebyte-lora-e32-rpi",
     package_dir={'': 'src'},
     py_modules=["lora_e32", "lora_e32_constants", "lora_e32_operation_constant"],
-    version="0.0.1",
+    version="0.0.2",
     description="Ebyte E32 LoRa raspberrypi library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.",
     long_description="Ebyte E32 LoRa raspberrypi library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.",
     keywords="LoRa, UART, EByte, e32, RaspberryPi, sx1278, sx1276",
     url="https://github.com/xreef/EByte_LoRa_E32_raspberrypi_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/src/ebyte_lora_e32_rpi.egg-info/PKG-INFO` & `ebyte-lora-e32-rpi-0.0.2/src/ebyte_lora_e32_rpi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e32-rpi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ebyte E32 LoRa raspberrypi library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.
 Home-page: https://github.com/xreef/EByte_LoRa_E32_raspberrypi_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -71,14 +71,15 @@
 3.  [LoRa E32 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2019/10/29/lora-e32-device-for-arduino-esp32-or-esp8266-configuration-part-3/)
 4.  [LoRa E32 device for Arduino, esp32 or esp8266: fixed transmission](https://www.mischianti.org/2019/11/10/lora-e32-device-for-arduino-esp32-or-esp8266-fixed-transmission-part-4/)
 5.  [LoRa E32 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2019/12/03/lora-e32-device-for-arduino-esp32-or-esp8266-power-saving-and-sending-structured-data-part-5/)
 6.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) the microcontroller and Arduino shield](https://www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/)
 7.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-wemos-d1-mini-shield-part-7/)
 
 ### Changelog
+ - 2023-05-02 0.0.2 Fix 900MHz devices frequency
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
 
 ### Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e32-rpi Version: 0.0.1 Summary: Ebyte
+Metadata-Version: 2.1 Name: ebyte-lora-e32-rpi Version: 0.0.2 Summary: Ebyte
 E32 LoRa raspberrypi library device very cheap and very long range (from 3Km to
 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino,
 esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276. Home-page: https://
 github.com/xreef/EByte_LoRa_E32_raspberrypi_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -53,21 +53,22 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-03-21 0.0.1 Fully functional
-library ### Library usage Here an example of constructor, you must pass the
-UART interface and (if you want, but It's reccomended) the AUX pin, M0 and M1.
-### Installation To install the library execute the following command: ```bash
-pip install ebyte-lora-e32-rpi ``` #### Initialization ```python from lora_e32
-import LoRaE32 import serial loraSerial = serial.Serial('/dev/serial0') #,
-baudrate=9600, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE,
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-05-02 0.0.2 Fix 900MHz
+devices frequency - 2023-03-21 0.0.1 Fully functional library ### Library usage
+Here an example of constructor, you must pass the UART interface and (if you
+want, but It's reccomended) the AUX pin, M0 and M1. ### Installation To install
+the library execute the following command: ```bash pip install ebyte-lora-e32-
+rpi ``` #### Initialization ```python from lora_e32 import LoRaE32 import
+serial loraSerial = serial.Serial('/dev/serial0') #, baudrate=9600,
+parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE,
 bytesize=serial.EIGHTBITS) lora = LoRaE32('433T20D', loraSerial, aux_pin=18,
 m0_pin=23, m1_pin=24) ``` #### Start the module transmission ```python code =
 lora.begin() print(ResponseStatusCode.get_description(code)) ``` #### Get
 Configuration ```python from lora_e32 import LoRaE32, print_configuration,
 Configuration from lora_e32_operation_constant import ResponseStatusCode code,
 configuration = lora.get_configuration() print
 (ResponseStatusCode.get_description(code)) print_configuration(configuration)
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/src/lora_e32.py` & `ebyte-lora-e32-rpi-0.0.2/src/lora_e32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #############################################################################################
 # EBYTE LoRa E32 Series for RaspberryPi
 #
 # AUTHOR:  Renzo Mischianti
-# VERSION: 0.0.1
+# VERSION: 0.0.2
 #
 # This library is based on the work of:
 # https://www.mischianti.org/category/my-libraries/lora-e32-devices/
 #
 # This library implements the EBYTE LoRa E32 Series for RaspberryPi.
 #
 #  ____________________________________________
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/src/lora_e32_constants.py` & `ebyte-lora-e32-rpi-0.0.2/src/lora_e32_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 # here a class that contains the starting frequency of the different devices
 # the device 433 start with 410 frequency and so on
 class OperatingFrequency:
     FREQUENCY_433 = 410
     FREQUENCY_170 = 130
     FREQUENCY_470 = 370
     FREQUENCY_868 = 862
-    FREQUENCY_900 = 850
+    FREQUENCY_900 = 862
     FREQUENCY_915 = 900
 
     @staticmethod
     def get_value_from_frequency(frequency):
         if not isinstance(frequency, str):
             frequency = str(frequency)
```

### Comparing `ebyte-lora-e32-rpi-0.0.1/src/lora_e32_operation_constant.py` & `ebyte-lora-e32-rpi-0.0.2/src/lora_e32_operation_constant.py`

 * *Files identical despite different names*

