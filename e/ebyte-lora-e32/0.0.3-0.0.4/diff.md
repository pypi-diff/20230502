# Comparing `tmp/ebyte-lora-e32-0.0.3.tar.gz` & `tmp/ebyte-lora-e32-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebyte-lora-e32-0.0.3.tar", last modified: Tue Apr 18 13:15:22 2023, max compression
+gzip compressed data, was "ebyte-lora-e32-0.0.4.tar", last modified: Tue May  2 07:00:29 2023, max compression
```

## Comparing `ebyte-lora-e32-0.0.3.tar` & `ebyte-lora-e32-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:15:22.256967 ebyte-lora-e32-0.0.3/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e32-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0    22822 2023-04-18 13:15:22.270009 ebyte-lora-e32-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    19867 2023-04-18 13:12:42.000000 ebyte-lora-e32-0.0.3/README.md
--rw-rw-rw-   0        0        0     1571 2023-04-18 13:13:50.000000 ebyte-lora-e32-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      924 2023-04-18 13:15:22.276970 ebyte-lora-e32-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1913 2023-04-18 13:13:50.000000 ebyte-lora-e32-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:15:22.219616 ebyte-lora-e32-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 13:15:22.254968 ebyte-lora-e32-0.0.3/src/ebyte_lora_e32.egg-info/
--rw-rw-rw-   0        0        0    22822 2023-04-18 13:15:22.000000 ebyte-lora-e32-0.0.3/src/ebyte_lora_e32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-18 13:15:22.000000 ebyte-lora-e32-0.0.3/src/ebyte_lora_e32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:15:22.000000 ebyte-lora-e32-0.0.3/src/ebyte_lora_e32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-18 13:15:22.000000 ebyte-lora-e32-0.0.3/src/ebyte_lora_e32.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    24566 2023-04-18 13:13:50.000000 ebyte-lora-e32-0.0.3/src/lora_e32.py
--rw-rw-rw-   0        0        0    12540 2023-04-18 12:00:51.000000 ebyte-lora-e32-0.0.3/src/lora_e32_constants.py
--rw-rw-rw-   0        0        0     2914 2023-03-21 16:15:50.000000 ebyte-lora-e32-0.0.3/src/lora_e32_operation_constant.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:00:29.225367 ebyte-lora-e32-0.0.4/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 ebyte-lora-e32-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0    22872 2023-05-02 07:00:29.226366 ebyte-lora-e32-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    19917 2023-05-02 06:58:54.000000 ebyte-lora-e32-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1571 2023-05-02 06:59:14.000000 ebyte-lora-e32-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      924 2023-05-02 07:00:29.234365 ebyte-lora-e32-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1913 2023-05-02 06:59:14.000000 ebyte-lora-e32-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 07:00:29.198136 ebyte-lora-e32-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 07:00:29.223392 ebyte-lora-e32-0.0.4/src/ebyte_lora_e32.egg-info/
+-rw-rw-rw-   0        0        0    22872 2023-05-02 07:00:29.000000 ebyte-lora-e32-0.0.4/src/ebyte_lora_e32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-02 07:00:29.000000 ebyte-lora-e32-0.0.4/src/ebyte_lora_e32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 07:00:29.000000 ebyte-lora-e32-0.0.4/src/ebyte_lora_e32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-02 07:00:29.000000 ebyte-lora-e32-0.0.4/src/ebyte_lora_e32.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    24566 2023-05-02 06:59:14.000000 ebyte-lora-e32-0.0.4/src/lora_e32.py
+-rw-rw-rw-   0        0        0    13039 2023-05-02 06:58:17.000000 ebyte-lora-e32-0.0.4/src/lora_e32_constants.py
+-rw-rw-rw-   0        0        0     2914 2023-03-21 16:15:50.000000 ebyte-lora-e32-0.0.4/src/lora_e32_operation_constant.py
```

### Comparing `ebyte-lora-e32-0.0.3/LICENSE.md` & `ebyte-lora-e32-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ebyte-lora-e32-0.0.3/PKG-INFO` & `ebyte-lora-e32-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e32
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.
 Home-page: https://github.com/xreef/EByte_LoRa_E32_micropython_library
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
+ - 2023-05-02 0.0.4 Fix 900Mhz devices frequency
  - 2023-04-18 0.0.3 Add power for new kind of devices and fix regex for device name
  - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.3 Summary: Ebyte E32
+Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.4 Summary: Ebyte E32
 LoRa micropython library device very cheap and very long range (from 3Km to
 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino,
 esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276. Home-page: https://
 github.com/xreef/EByte_LoRa_E32_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -54,47 +54,47 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-04-18 0.0.3 Add power for
-new kind of devices and fix regex for device name - 2023-04-18 0.0.2 Distinct
-frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/
-forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21 0.0.1 Fully
-functional library ### Library usage Here an example of constructor, you must
-pass the UART interface and (if you want, but It's reccomended) the AUX pin, M0
-and M1. ### Installation To install the library execute the following command:
-```bash pip install ebyte-lora-e32 ``` #### Initialization ```python from
-lora_e32 import LoRaE32 from machine import UART uart2 = UART(2) lora = LoRaE32
-('433T20D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
-transmission ```python code = lora.begin() print
-(ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e32 import LoRaE32, print_configuration, Configuration from
-lora_e32_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print(ResponseStatusCode.get_description(code))
-print_configuration(configuration) ``` The result ``` -------------------------
---------------- HEAD : 0b11000000 192 AddH : 0 AddL : 2 Chan : 23 -> 433
-SpeedParityBit : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps
-(default) SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionTrans : 0b1 -
-> Fixed transmission (first three bytes can be used a s high/low address and
-channel) OptionPullup : 0b1 -> TXD, RXD, AUX are push-pulls/pull-ups (default)
-OptionWakeup : 0b0 -> 250ms (default) OptionFEC : 0b1 -> Turn on Forward Error
-Correction Switch (Default) OptionPower : 0b0 -> 20dBm (Default) --------------
--------------------------- ``` #### Set Configuration ```python
-configuration_to_set = Configuration('433T20D') configuration_to_set.ADDL =
-0x02 configuration_to_set.OPTION.fixedTransmission =
-FixedTransmission.FIXED_TRANSMISSION code, confSetted = lora.set_configuration
-(configuration_to_set) ``` The configuration object has a lot of parameters.
-```python class Configuration: class Speed: def __init__(self, model):
-self.model = model self.airDataRate = AirDataRate.AIR_DATA_RATE_010_24
-self.uartBaudRate = UARTBaudRate.BPS_9600 self.uartParity =
-UARTParity.MODE_00_8N1 class Option: def __init__(self, model): self.model =
-model self.transmissionPower = TransmissionPower
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-05-02 0.0.4 Fix 900Mhz
+devices frequency - 2023-04-18 0.0.3 Add power for new kind of devices and fix
+regex for device name - 2023-04-18 0.0.2 Distinct frequency from 900MHz and
+915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-
+e32-900t-modules/) - 2023-03-21 0.0.1 Fully functional library ### Library
+usage Here an example of constructor, you must pass the UART interface and (if
+you want, but It's reccomended) the AUX pin, M0 and M1. ### Installation To
+install the library execute the following command: ```bash pip install ebyte-
+lora-e32 ``` #### Initialization ```python from lora_e32 import LoRaE32 from
+machine import UART uart2 = UART(2) lora = LoRaE32('433T20D', uart2,
+aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module transmission
+```python code = lora.begin() print(ResponseStatusCode.get_description(code))
+``` #### Get Configuration ```python from lora_e32 import LoRaE32,
+print_configuration, Configuration from lora_e32_operation_constant import
+ResponseStatusCode code, configuration = lora.get_configuration() print
+(ResponseStatusCode.get_description(code)) print_configuration(configuration)
+``` The result ``` ---------------------------------------- HEAD : 0b11000000
+192 AddH : 0 AddL : 2 Chan : 23 -> 433 SpeedParityBit : 0b0 -> 8N1 (Default)
+SpeedUARTDatte : 0b11 -> 9600bps (default) SpeedAirDataRate : 0b10 -> 2.4kbps
+(default) OptionTrans : 0b1 -> Fixed transmission (first three bytes can be
+used a s high/low address and channel) OptionPullup : 0b1 -> TXD, RXD, AUX are
+push-pulls/pull-ups (default) OptionWakeup : 0b0 -> 250ms (default) OptionFEC :
+0b1 -> Turn on Forward Error Correction Switch (Default) OptionPower : 0b0 -
+> 20dBm (Default) ---------------------------------------- ``` #### Set
+Configuration ```python configuration_to_set = Configuration('433T20D')
+configuration_to_set.ADDL = 0x02 configuration_to_set.OPTION.fixedTransmission
+= FixedTransmission.FIXED_TRANSMISSION code, confSetted =
+lora.set_configuration(configuration_to_set) ``` The configuration object has a
+lot of parameters. ```python class Configuration: class Speed: def __init__
+(self, model): self.model = model self.airDataRate =
+AirDataRate.AIR_DATA_RATE_010_24 self.uartBaudRate = UARTBaudRate.BPS_9600
+self.uartParity = UARTParity.MODE_00_8N1 class Option: def __init__(self,
+model): self.model = model self.transmissionPower = TransmissionPower
 (self.model).get_transmission_power().get_default_value() self.fec =
 ForwardErrorCorrectionSwitch.FEC_1_ON self.wirelessWakeupTime =
 WirelessWakeUpTime.WAKE_UP_250 self.ioDriveMode =
 IODriveMode.PUSH_PULLS_PULL_UPS self.fixedTransmission =
 FixedTransmission.TRANSPARENT_TRANSMISSION class Configuration: def __init__
 (self, model): self.HEAD = 0 self.ADDH = 0 self.ADDL = 0 self.SPED = Speed
 (model) self.CHAN = 23 self.OPTION = Option(model) ``` I create a CONSTANTS
```

### Comparing `ebyte-lora-e32-0.0.3/README.md` & `ebyte-lora-e32-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 3.  [LoRa E32 device for Arduino, esp32 or esp8266: configuration](https://www.mischianti.org/2019/10/29/lora-e32-device-for-arduino-esp32-or-esp8266-configuration-part-3/)
 4.  [LoRa E32 device for Arduino, esp32 or esp8266: fixed transmission](https://www.mischianti.org/2019/11/10/lora-e32-device-for-arduino-esp32-or-esp8266-fixed-transmission-part-4/)
 5.  [LoRa E32 device for Arduino, esp32 or esp8266: power saving and sending structured data](https://www.mischianti.org/2019/12/03/lora-e32-device-for-arduino-esp32-or-esp8266-power-saving-and-sending-structured-data-part-5/)
 6.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) the microcontroller and Arduino shield](https://www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/)
 7.  [LoRa E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-wemos-d1-mini-shield-part-7/)
 
 ### Changelog
+ - 2023-05-02 0.0.4 Fix 900Mhz devices frequency
  - 2023-04-18 0.0.3 Add power for new kind of devices and fix regex for device name
  - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
```

#### html2text {}

```diff
@@ -18,47 +18,47 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-04-18 0.0.3 Add power for
-new kind of devices and fix regex for device name - 2023-04-18 0.0.2 Distinct
-frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/
-forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21 0.0.1 Fully
-functional library ### Library usage Here an example of constructor, you must
-pass the UART interface and (if you want, but It's reccomended) the AUX pin, M0
-and M1. ### Installation To install the library execute the following command:
-```bash pip install ebyte-lora-e32 ``` #### Initialization ```python from
-lora_e32 import LoRaE32 from machine import UART uart2 = UART(2) lora = LoRaE32
-('433T20D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
-transmission ```python code = lora.begin() print
-(ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e32 import LoRaE32, print_configuration, Configuration from
-lora_e32_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print(ResponseStatusCode.get_description(code))
-print_configuration(configuration) ``` The result ``` -------------------------
---------------- HEAD : 0b11000000 192 AddH : 0 AddL : 2 Chan : 23 -> 433
-SpeedParityBit : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps
-(default) SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionTrans : 0b1 -
-> Fixed transmission (first three bytes can be used a s high/low address and
-channel) OptionPullup : 0b1 -> TXD, RXD, AUX are push-pulls/pull-ups (default)
-OptionWakeup : 0b0 -> 250ms (default) OptionFEC : 0b1 -> Turn on Forward Error
-Correction Switch (Default) OptionPower : 0b0 -> 20dBm (Default) --------------
--------------------------- ``` #### Set Configuration ```python
-configuration_to_set = Configuration('433T20D') configuration_to_set.ADDL =
-0x02 configuration_to_set.OPTION.fixedTransmission =
-FixedTransmission.FIXED_TRANSMISSION code, confSetted = lora.set_configuration
-(configuration_to_set) ``` The configuration object has a lot of parameters.
-```python class Configuration: class Speed: def __init__(self, model):
-self.model = model self.airDataRate = AirDataRate.AIR_DATA_RATE_010_24
-self.uartBaudRate = UARTBaudRate.BPS_9600 self.uartParity =
-UARTParity.MODE_00_8N1 class Option: def __init__(self, model): self.model =
-model self.transmissionPower = TransmissionPower
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-05-02 0.0.4 Fix 900Mhz
+devices frequency - 2023-04-18 0.0.3 Add power for new kind of devices and fix
+regex for device name - 2023-04-18 0.0.2 Distinct frequency from 900MHz and
+915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-
+e32-900t-modules/) - 2023-03-21 0.0.1 Fully functional library ### Library
+usage Here an example of constructor, you must pass the UART interface and (if
+you want, but It's reccomended) the AUX pin, M0 and M1. ### Installation To
+install the library execute the following command: ```bash pip install ebyte-
+lora-e32 ``` #### Initialization ```python from lora_e32 import LoRaE32 from
+machine import UART uart2 = UART(2) lora = LoRaE32('433T20D', uart2,
+aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module transmission
+```python code = lora.begin() print(ResponseStatusCode.get_description(code))
+``` #### Get Configuration ```python from lora_e32 import LoRaE32,
+print_configuration, Configuration from lora_e32_operation_constant import
+ResponseStatusCode code, configuration = lora.get_configuration() print
+(ResponseStatusCode.get_description(code)) print_configuration(configuration)
+``` The result ``` ---------------------------------------- HEAD : 0b11000000
+192 AddH : 0 AddL : 2 Chan : 23 -> 433 SpeedParityBit : 0b0 -> 8N1 (Default)
+SpeedUARTDatte : 0b11 -> 9600bps (default) SpeedAirDataRate : 0b10 -> 2.4kbps
+(default) OptionTrans : 0b1 -> Fixed transmission (first three bytes can be
+used a s high/low address and channel) OptionPullup : 0b1 -> TXD, RXD, AUX are
+push-pulls/pull-ups (default) OptionWakeup : 0b0 -> 250ms (default) OptionFEC :
+0b1 -> Turn on Forward Error Correction Switch (Default) OptionPower : 0b0 -
+> 20dBm (Default) ---------------------------------------- ``` #### Set
+Configuration ```python configuration_to_set = Configuration('433T20D')
+configuration_to_set.ADDL = 0x02 configuration_to_set.OPTION.fixedTransmission
+= FixedTransmission.FIXED_TRANSMISSION code, confSetted =
+lora.set_configuration(configuration_to_set) ``` The configuration object has a
+lot of parameters. ```python class Configuration: class Speed: def __init__
+(self, model): self.model = model self.airDataRate =
+AirDataRate.AIR_DATA_RATE_010_24 self.uartBaudRate = UARTBaudRate.BPS_9600
+self.uartParity = UARTParity.MODE_00_8N1 class Option: def __init__(self,
+model): self.model = model self.transmissionPower = TransmissionPower
 (self.model).get_transmission_power().get_default_value() self.fec =
 ForwardErrorCorrectionSwitch.FEC_1_ON self.wirelessWakeupTime =
 WirelessWakeUpTime.WAKE_UP_250 self.ioDriveMode =
 IODriveMode.PUSH_PULLS_PULL_UPS self.fixedTransmission =
 FixedTransmission.TRANSPARENT_TRANSMISSION class Configuration: def __init__
 (self, model): self.HEAD = 0 self.ADDH = 0 self.ADDL = 0 self.SPED = Speed
 (model) self.CHAN = 23 self.OPTION = Option(model) ``` I create a CONSTANTS
```

### Comparing `ebyte-lora-e32-0.0.3/pyproject.toml` & `ebyte-lora-e32-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2265 6279 7465 2d6c 6f72 612d 6533  = "ebyte-lora-e3
 00000020: 3222 0d0a 7665 7273 696f 6e20 3d20 2230  2"..version = "0
-00000030: 2e30 2e33 220d 0a61 7574 686f 7273 203d  .0.3"..authors =
+00000030: 2e30 2e34 220d 0a61 7574 686f 7273 203d  .0.4"..authors =
 00000040: 205b 0d0a 2020 7b20 6e61 6d65 3d22 5265   [..  { name="Re
 00000050: 6e7a 6f20 4d69 7363 6869 616e 7469 222c  nzo Mischianti",
 00000060: 2065 6d61 696c 3d22 7265 6e7a 6f40 6d69   email="renzo@mi
 00000070: 7363 6869 616e 7469 2e6f 7267 2220 7d2c  schianti.org" },
 00000080: 0d0a 5d0d 0a6d 6169 6e74 6169 6e65 7273  ..]..maintainers
 00000090: 203d 205b 0d0a 2020 7b20 6e61 6d65 3d22   = [..  { name="
 000000a0: 5265 6e7a 6f20 4d69 7363 6869 616e 7469  Renzo Mischianti
```

### Comparing `ebyte-lora-e32-0.0.3/setup.cfg` & `ebyte-lora-e32-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6279 7465 2d6c 6f72 612d 6533   = ebyte-lora-e3
 00000020: 320d 0a76 6572 7369 6f6e 203d 2030 2e30  2..version = 0.0
-00000030: 2e33 0d0a 6175 7468 6f72 203d 2052 656e  .3..author = Ren
+00000030: 2e34 0d0a 6175 7468 6f72 203d 2052 656e  .4..author = Ren
 00000040: 7a6f 204d 6973 6368 6961 6e74 690d 0a64  zo Mischianti..d
 00000050: 6573 6372 6970 7469 6f6e 203d 2022 4562  escription = "Eb
 00000060: 7974 6520 4533 3220 4c6f 5261 206d 6963  yte E32 LoRa mic
 00000070: 726f 7079 7468 6f6e 206c 6962 7261 7279  ropython library
 00000080: 2064 6576 6963 6520 7665 7279 2063 6865   device very che
 00000090: 6170 2061 6e64 2076 6572 7920 6c6f 6e67  ap and very long
 000000a0: 2072 616e 6765 2028 6672 6f6d 2033 4b6d   range (from 3Km
```

### Comparing `ebyte-lora-e32-0.0.3/setup.py` & `ebyte-lora-e32-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="ebyte-lora-e32",
     package_dir={'': 'src'},
     py_modules=["lora_e32", "lora_e32_constants", "lora_e32_operation_constant"],
-    version="0.0.3",
+    version="0.0.4",
     description="Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.",
     long_description="Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.",
     keywords="LoRa, UART, EByte, e32, esp32, esp8266, stm32, SAMD, Arduino, Raspberry Pi Pico, MicroPython, sx1278, sx1276",
     url="https://github.com/xreef/EByte_LoRa_E32_micropython_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `ebyte-lora-e32-0.0.3/src/ebyte_lora_e32.egg-info/PKG-INFO` & `ebyte-lora-e32-0.0.4/src/ebyte_lora_e32.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebyte-lora-e32
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ebyte E32 LoRa micropython library device very cheap and very long range (from 3Km to 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino, esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276.
 Home-page: https://github.com/xreef/EByte_LoRa_E32_micropython_library
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
+ - 2023-05-02 0.0.4 Fix 900Mhz devices frequency
  - 2023-04-18 0.0.3 Add power for new kind of devices and fix regex for device name
  - 2023-04-18 0.0.2 Distinct frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-e32-900t-modules/)
  - 2023-03-21 0.0.1 Fully functional library
 
 ### Library usage
 Here an example of constructor, you must pass the UART interface and (if you want, but It's reccomended)
 the AUX pin, M0 and M1.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.3 Summary: Ebyte E32
+Metadata-Version: 2.1 Name: ebyte-lora-e32 Version: 0.0.4 Summary: Ebyte E32
 LoRa micropython library device very cheap and very long range (from 3Km to
 8Km). Arduino LoRa EBYTE E32 device library complete and tested with Arduino,
 esp8266, esp32, STM32 and Raspberry Pi Pico. sx1278/sx1276. Home-page: https://
 github.com/xreef/EByte_LoRa_E32_micropython_library Author: Renzo Mischianti
 Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
@@ -54,47 +54,47 @@
 structured-data-part-5/) 6. [LoRa E32 device for Arduino, esp32 or esp8266: WOR
 (wake on radio) the microcontroller and Arduino shield](https://
 www.mischianti.org/2019/12/28/lora-e32-device-for-arduino-esp32-or-esp8266-wor-
 wake-on-radio-the-microcontroller-also-and-new-arduino-shield-part-6/) 7. [LoRa
 E32 device for Arduino, esp32 or esp8266: WOR (wake on radio) microcontroller
 and new WeMos D1 mini shield](https://www.mischianti.org/2020/01/17/lora-e32-
 device-for-arduino-esp32-or-esp8266-wor-wake-on-radio-microcontroller-and-new-
-wemos-d1-mini-shield-part-7/) ### Changelog - 2023-04-18 0.0.3 Add power for
-new kind of devices and fix regex for device name - 2023-04-18 0.0.2 Distinct
-frequency from 900MHz and 915Mhz devices [Forum](https://www.mischianti.org/
-forums/topic/e32-915t-and-e32-900t-modules/) - 2023-03-21 0.0.1 Fully
-functional library ### Library usage Here an example of constructor, you must
-pass the UART interface and (if you want, but It's reccomended) the AUX pin, M0
-and M1. ### Installation To install the library execute the following command:
-```bash pip install ebyte-lora-e32 ``` #### Initialization ```python from
-lora_e32 import LoRaE32 from machine import UART uart2 = UART(2) lora = LoRaE32
-('433T20D', uart2, aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module
-transmission ```python code = lora.begin() print
-(ResponseStatusCode.get_description(code)) ``` #### Get Configuration ```python
-from lora_e32 import LoRaE32, print_configuration, Configuration from
-lora_e32_operation_constant import ResponseStatusCode code, configuration =
-lora.get_configuration() print(ResponseStatusCode.get_description(code))
-print_configuration(configuration) ``` The result ``` -------------------------
---------------- HEAD : 0b11000000 192 AddH : 0 AddL : 2 Chan : 23 -> 433
-SpeedParityBit : 0b0 -> 8N1 (Default) SpeedUARTDatte : 0b11 -> 9600bps
-(default) SpeedAirDataRate : 0b10 -> 2.4kbps (default) OptionTrans : 0b1 -
-> Fixed transmission (first three bytes can be used a s high/low address and
-channel) OptionPullup : 0b1 -> TXD, RXD, AUX are push-pulls/pull-ups (default)
-OptionWakeup : 0b0 -> 250ms (default) OptionFEC : 0b1 -> Turn on Forward Error
-Correction Switch (Default) OptionPower : 0b0 -> 20dBm (Default) --------------
--------------------------- ``` #### Set Configuration ```python
-configuration_to_set = Configuration('433T20D') configuration_to_set.ADDL =
-0x02 configuration_to_set.OPTION.fixedTransmission =
-FixedTransmission.FIXED_TRANSMISSION code, confSetted = lora.set_configuration
-(configuration_to_set) ``` The configuration object has a lot of parameters.
-```python class Configuration: class Speed: def __init__(self, model):
-self.model = model self.airDataRate = AirDataRate.AIR_DATA_RATE_010_24
-self.uartBaudRate = UARTBaudRate.BPS_9600 self.uartParity =
-UARTParity.MODE_00_8N1 class Option: def __init__(self, model): self.model =
-model self.transmissionPower = TransmissionPower
+wemos-d1-mini-shield-part-7/) ### Changelog - 2023-05-02 0.0.4 Fix 900Mhz
+devices frequency - 2023-04-18 0.0.3 Add power for new kind of devices and fix
+regex for device name - 2023-04-18 0.0.2 Distinct frequency from 900MHz and
+915Mhz devices [Forum](https://www.mischianti.org/forums/topic/e32-915t-and-
+e32-900t-modules/) - 2023-03-21 0.0.1 Fully functional library ### Library
+usage Here an example of constructor, you must pass the UART interface and (if
+you want, but It's reccomended) the AUX pin, M0 and M1. ### Installation To
+install the library execute the following command: ```bash pip install ebyte-
+lora-e32 ``` #### Initialization ```python from lora_e32 import LoRaE32 from
+machine import UART uart2 = UART(2) lora = LoRaE32('433T20D', uart2,
+aux_pin=15, m0_pin=21, m1_pin=19) ``` #### Start the module transmission
+```python code = lora.begin() print(ResponseStatusCode.get_description(code))
+``` #### Get Configuration ```python from lora_e32 import LoRaE32,
+print_configuration, Configuration from lora_e32_operation_constant import
+ResponseStatusCode code, configuration = lora.get_configuration() print
+(ResponseStatusCode.get_description(code)) print_configuration(configuration)
+``` The result ``` ---------------------------------------- HEAD : 0b11000000
+192 AddH : 0 AddL : 2 Chan : 23 -> 433 SpeedParityBit : 0b0 -> 8N1 (Default)
+SpeedUARTDatte : 0b11 -> 9600bps (default) SpeedAirDataRate : 0b10 -> 2.4kbps
+(default) OptionTrans : 0b1 -> Fixed transmission (first three bytes can be
+used a s high/low address and channel) OptionPullup : 0b1 -> TXD, RXD, AUX are
+push-pulls/pull-ups (default) OptionWakeup : 0b0 -> 250ms (default) OptionFEC :
+0b1 -> Turn on Forward Error Correction Switch (Default) OptionPower : 0b0 -
+> 20dBm (Default) ---------------------------------------- ``` #### Set
+Configuration ```python configuration_to_set = Configuration('433T20D')
+configuration_to_set.ADDL = 0x02 configuration_to_set.OPTION.fixedTransmission
+= FixedTransmission.FIXED_TRANSMISSION code, confSetted =
+lora.set_configuration(configuration_to_set) ``` The configuration object has a
+lot of parameters. ```python class Configuration: class Speed: def __init__
+(self, model): self.model = model self.airDataRate =
+AirDataRate.AIR_DATA_RATE_010_24 self.uartBaudRate = UARTBaudRate.BPS_9600
+self.uartParity = UARTParity.MODE_00_8N1 class Option: def __init__(self,
+model): self.model = model self.transmissionPower = TransmissionPower
 (self.model).get_transmission_power().get_default_value() self.fec =
 ForwardErrorCorrectionSwitch.FEC_1_ON self.wirelessWakeupTime =
 WirelessWakeUpTime.WAKE_UP_250 self.ioDriveMode =
 IODriveMode.PUSH_PULLS_PULL_UPS self.fixedTransmission =
 FixedTransmission.TRANSPARENT_TRANSMISSION class Configuration: def __init__
 (self, model): self.HEAD = 0 self.ADDH = 0 self.ADDL = 0 self.SPED = Speed
 (model) self.CHAN = 23 self.OPTION = Option(model) ``` I create a CONSTANTS
```

### Comparing `ebyte-lora-e32-0.0.3/src/lora_e32.py` & `ebyte-lora-e32-0.0.4/src/lora_e32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #############################################################################################
 # EBYTE LoRa E32 Series for MicroPython
 #
 # AUTHOR:  Renzo Mischianti
-# VERSION: 0.0.3
+# VERSION: 0.0.4
 #
 # This library is based on the work of:
 # https://www.mischianti.org/category/my-libraries/lora-e32-devices/
 #
 # This library implements the EBYTE LoRa E32 Series for MicroPython.
 #
 # The MIT License (MIT)
```

### Comparing `ebyte-lora-e32-0.0.3/src/lora_e32_constants.py` & `ebyte-lora-e32-0.0.4/src/lora_e32_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+class Logger:
+    def __init__(self, enable_debug):
+        self.enable_debug = enable_debug
+        self.name = ''
+
+    def debug(self, msg, *args):
+        if self.enable_debug:
+            print(self.name + ' DEBUG ' + msg, *args)
+
+    def info(self, msg, *args):
+        if self.enable_debug:
+            print(self.name + ' INFO ' + msg, *args)
+
+    def error(self, msg, *args):
+        if self.enable_debug:
+            print(self.name + ' ERROR ' + msg, *args)
+
+    def getLogger(self, name):
+        self.name = name
+        return Logger(self.enable_debug)
+
+
+logging = Logger(False)
+
+logger = logging.getLogger(__name__)
+
+
 class UARTParity:
     MODE_00_8N1 = 0b00
     MODE_01_8O1 = 0b01
     MODE_10_8E1 = 0b10
     MODE_11_8N1 = 0b11
 
     @staticmethod
@@ -269,14 +296,17 @@
     POWER_37_00 = 0b00
     POWER_37_01 = 0b01
     POWER_37_10 = 0b10
     POWER_37_11 = 0b11
 
     @staticmethod
     def get_description(transmission_power):
+        logger.debug("TransmissionPower37.get_description: transmission_power = %s", transmission_power)
+        logger.debug("TransmissionPower37.POWER_37_00: transmission_power = %s", TransmissionPower37.POWER_37_00)
+
         if transmission_power == TransmissionPower37.POWER_37_00:
             return "37dBm (Default)"
         elif transmission_power == TransmissionPower37.POWER_37_01:
             return "37dBm"
         elif transmission_power == TransmissionPower37.POWER_37_10:
             return "37dBm"
         elif transmission_power == TransmissionPower37.POWER_37_11:
@@ -292,15 +322,15 @@
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
 
@@ -331,14 +361,17 @@
         self.frequency = None
         self.transmission_power = None
 
         if model is not None:
             self.package_type = model[6]
             self.frequency = int(model[0:3])
             self.transmission_power = int(model[4:6])
+            logger.debug("Package type: " + self.package_type)
+            logger.debug("Frequency: " + str(self.frequency))
+            logger.debug("Transmission power: " + str(self.transmission_power))
 
     def get_transmission_power(self):
         if self.transmission_power == 20:
             return TransmissionPower20
         elif self.transmission_power == 27:
             return TransmissionPower27
         elif self.transmission_power == 30:
@@ -347,19 +380,8 @@
             return TransmissionPower33
         elif self.transmission_power == 37:
             return TransmissionPower37
         else:
             return "Invalid transmission power param"
 
     def get_transmission_power_description(self, transmission_power):
-        if self.transmission_power == 20:
-            return TransmissionPower20.get_description(transmission_power)
-        elif self.transmission_power == 27:
-            return TransmissionPower27.get_description(transmission_power)
-        elif self.transmission_power == 30:
-            return TransmissionPower30.get_description(transmission_power)
-        elif self.transmission_power == 33:
-            return TransmissionPower33.get_description(transmission_power)
-        elif self.transmission_power == 37:
-            return TransmissionPower37.get_description(transmission_power)
-        else:
-            return "Invalid transmission power param"
+        return self.get_transmission_power().get_description(transmission_power)
```

### Comparing `ebyte-lora-e32-0.0.3/src/lora_e32_operation_constant.py` & `ebyte-lora-e32-0.0.4/src/lora_e32_operation_constant.py`

 * *Files identical despite different names*

