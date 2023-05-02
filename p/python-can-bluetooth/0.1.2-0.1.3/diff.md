# Comparing `tmp/python-can-bluetooth-0.1.2.tar.gz` & `tmp/python-can-bluetooth-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-can-bluetooth-0.1.2.tar", last modified: Wed Apr 26 22:11:54 2023, max compression
+gzip compressed data, was "python-can-bluetooth-0.1.3.tar", last modified: Tue May  2 05:35:14 2023, max compression
```

## Comparing `python-can-bluetooth-0.1.2.tar` & `python-can-bluetooth-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.641863 python-can-bluetooth-0.1.2/can_bluetooth/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth/_bluetooth_can.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.641863 python-can-bluetooth-0.1.2/can_bluetooth_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_examples/bluetooth_tx_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/can_bluetooth_test/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_test/test_interface_bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/can_bluetooth_test/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:11:54.645863 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 22:11:54.000000 python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-26 22:11:54.649863 python-can-bluetooth-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 22:11:39.000000 python-can-bluetooth-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:35:14.419885 python-can-bluetooth-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-02 05:35:14.419885 python-can-bluetooth-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:35:14.419885 python-can-bluetooth-0.1.3/can_bluetooth/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/can_bluetooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20132 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/can_bluetooth/_bluetooth_can.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/can_bluetooth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:35:14.419885 python-can-bluetooth-0.1.3/can_bluetooth_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/can_bluetooth_examples/bluetooth_tx_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:35:14.419885 python-can-bluetooth-0.1.3/can_bluetooth_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/can_bluetooth_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/can_bluetooth_test/test_interface_bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/can_bluetooth_test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:35:14.419885 python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-02 05:35:14.000000 python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-02 05:35:14.000000 python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:35:14.000000 python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 05:35:14.000000 python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 05:35:14.000000 python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 05:35:14.000000 python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 05:35:14.419885 python-can-bluetooth-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-02 05:35:01.000000 python-can-bluetooth-0.1.3/setup.py
```

### Comparing `python-can-bluetooth-0.1.2/PKG-INFO` & `python-can-bluetooth-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can-bluetooth
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python-can interface driver for CAN transmitted over a Bluetooth SPP connection
 Author-email: Matt Woodhead <woody.w62@gmail.com>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: homepage, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: documentation, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: repository, https://github.com/MattWoodhead/python-can-bluetooth
 Keywords: CANbus,Bluetooth,python-can,ESP32
```

### Comparing `python-can-bluetooth-0.1.2/README.rst` & `python-can-bluetooth-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `python-can-bluetooth-0.1.2/can_bluetooth/_bluetooth_can.py` & `python-can-bluetooth-0.1.3/can_bluetooth/_bluetooth_can.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,33 +7,36 @@
 See the interface documentation for the format being used.
 
 Created on Wed Dec 28 20:56:33 2022
 
 Copyright (C) 2023 Matt Woodhead
 """
 
+# standard library modules
 import io
 import logging
 import string
 import struct
 import time
 from typing import Any, List, Tuple, Optional
 
+# external library modules
 from can import (
     BusABC,
     BusState,
     CanError,
     CanInterfaceNotImplementedError,
     CanInitializationError,
     CanOperationError,
     CanTimeoutError,
     Message,
 )
 from can.typechecking import AutoDetectedConfig
 
+
 logger = logging.getLogger("can.bluetoothspp")
 
 try:
     import serial
 except ImportError:
     logger.warning(
         (
@@ -45,33 +48,39 @@
 
 try:
     from serial.tools.list_ports import comports as list_comports
 except ImportError:
     # If unavailable on some platform, just return nothing
     def list_comports() -> List[Any]:
         """
-        A dummy function to cover the case where the list_comports method from the serial library is not available
+        A dummy function to cover the case where the list_comports method from the
+        serial library is not available
         """
         return []
 
 
 def list_bluetooth_ports() -> List[Any]:
     """
-    A function to filter the COM ports on computer to those acting as Serial over Bluetooth (SPP) links
+    A function to filter the COM ports on computer to those acting as Serial over
+    Bluetooth (SPP) links
     :return: DESCRIPTION
     :rtype: List[Any]
-
     """
     ports = list_comports()
     if ports:
-        ports = [p for p in ports if r"BTHENUM\{" in p.hwid]  # TODO: detection currently Windows only
+        # TODO: detection currently Windows only
+        ports = [p for p in ports if r"BTHENUM\{" in p.hwid]
         return ports
     return []
 
 
+MIN_BUFFER_LEN = 14
+MAX_BUFFER_LEN = 23
+
+
 class BluetoothSPPBus(BusABC):
     """
     Enable basic can communication over a serial device.
 
     .. note:: See :meth:`~_recv_internal` for some special semantics.
 
     """
@@ -80,40 +89,62 @@
         self,
         channel: str,
         bitrate: int = 250000,
         bt_baudrate: int = 921600,
         timeout: float = 0.1,
         state: BusState = BusState.PASSIVE,
         rtscts: bool = False,
-        timestamps_use_computer_time: bool = True,
         *args,
         **kwargs,
     ) -> None:
         """
         :param channel:
             The serial port to open. For example "/dev/ttyS1" or
             "/dev/ttyUSB0" on Linux or "COM1" on Windows systems.
             This should be the 'Outgoing' port of the bluetooth SPP com port pair.
 
         :param bitrate:
-            Bit rate of the BT CAN interface in bit/s (default 250000).
+            Bit rate of the BT CAN interface in bit/s.
+            defaults to 250000
 
-        :param baudrate:
-            Baud rate of the Bluetooth SPP port in bit/s (default 921600).
+        :param bt_baudrate:
+            Baud rate of the Bluetooth SPP port in bit/s.
+            defaults to 921600
 
         :param timeout:
-            Timeout for the serial device in seconds (default 0.1).
+            Timeout for the serial device in seconds.
+            defaults to 0.1
 
         :param rtscts:
             turn hardware handshake (RTS/CTS) on and off
+            defaults to False
 
         :param timestamps_use_computer_time:
-            enable/disbale the adjustment of the timestamp values to match the
+            enable/disable the adjustment of the timestamp values to match the
             computers time (useful when datalogging and trying to establish
             event timings)
+            defaults to False
+
+        :param ignore_bluetooth_rx_crc:
+            enable/disable the checking of the bluetooth transmission with a CRC.
+            This is disabled / enabled both in the python module and at the
+            bluetooth adapter if the functionality is supported.
+            defaults to False
+
+        :param ignore_bluetooth_tx_crc:
+            enable/disable the calculation of the message CRC before it is sent
+            to the adapter. This can olny be used if the bluetooth adapter supports
+            disabling the CRC check in its logic too.
+            defaults to False
+
+        :param behaviour_on_data_error:
+            The behaviour that should be taken if a malformed message arrives
+            (e.g. CRC check fails, invalid delimiter byte etc.).
+            One of 'raise' or 'ignore'.
+            defaults to 'raise'
 
         :raises ~can.exceptions.CanInitializationError:
             If the given parameters are invalid.
         :raises ~can.exceptions.CanInterfaceNotImplementedError:
             If the serial module is not installed.
         """
 
@@ -122,29 +153,52 @@
 
         if not channel:
             raise TypeError("Must specify a serial port.")
 
         self.channel_info = f"Serial interface: {channel}"
 
         try:
-            self._ser = serial.serial_for_url(channel, baudrate=bt_baudrate, timeout=timeout, rtscts=rtscts)
+            self._ser = serial.serial_for_url(
+                channel,
+                baudrate=bt_baudrate,
+                timeout=timeout,
+                rtscts=rtscts,
+            )
         except ValueError as error:
-            raise CanInitializationError("could not create the serial device") from error
+            raise CanInitializationError("Could not create the serial device") from error
 
-        if timestamps_use_computer_time:
+        if kwargs.get("timestamps_use_computer_time"):
             self._bus_pc_start_time_s = round(time.time(), 4)
         else:
             self._bus_pc_start_time_s = 0
 
+        # A bytes object buffer in which the recevied bytes will be stored
+        self._rx_byte_buffer = b""
+
         # interface configuration attributes
-        # if these are changed after initialisation, self._send_interface_can_config() must be called
+        # if these are changed after init, self._send_interface_can_config() must be called
         self.bitrate = bitrate  # CAN Bit rate
         self._state = state  # 0 = Active, 1 = passive, 2 = error
         self.interface_enable_can = True  # Enable/disable can interface
 
+        if kwargs.get("ignore_bluetooth_rx_crc"):
+            self.ignore_bt_rx_crc = True
+        else:
+            self.ignore_bt_rx_crc = False
+
+        if kwargs.get("ignore_bluetooth_tx_crc"):
+            self.ignore_bt_tx_crc = True
+        else:
+            self.ignore_bt_tx_crc = False
+
+        if kwargs.get("behaviour_on_data_error", "raise") == "ignore":
+            self._raise_exceptions_on_data_errors = True
+        else:
+            self._raise_exceptions_on_data_errors = False
+
         super().__init__(channel, *args, **kwargs)
 
     @property
     def state(self):
         return self._state
 
     @state.setter
@@ -174,17 +228,17 @@
                       to an integer.
 
         :param timeout:
             This parameter will be ignored. The timeout value of the channel is
             used instead.
 
         :param interface_control:
-            This boolean determines if the message is a CAN message or an interface control message (the difference
-            being the start and termination bytes of the message stream to allow the interface to distinguish between
-            the different types of data)
+            This boolean determines if the message is a CAN message or an interface control message
+            (the difference being the start and termination bytes of the message stream to allow
+            the interface to distinguish between the different types of data)
 
         """
         # Pack timestamp
         try:
             timestamp = struct.pack(">I", int(msg.timestamp * 1000))
         except struct.error as ste:
             raise ValueError("Timestamp is out of range") from ste
@@ -209,141 +263,170 @@
         # Assemble core message (for CRC calculation)
         byte_msg_core.append(msg.dlc)
         byte_msg_core += flag_byte
         byte_msg_core += arbitration_id
         byte_msg_core += msg.data
 
         # CRC is calculated on the DLC, flags, ID, and Data bytes
-        print(f"CRC: {calculate_crc15(byte_msg_core)}")
-        byte_msg_core += struct.pack("<H", calculate_crc15(byte_msg_core))
+        if not self.ignore_bt_tx_crc:
+            crc = calculate_crc15(byte_msg_core)
+        else:
+            crc = 0x0
+        # print(f"CRC: 0x{calculate_crc15(byte_msg_core):02x}")
+        byte_msg_core += struct.pack("<H", crc)
 
         # prepend start byte and timestamp to the main message bytearray
         if interface_control:
             byte_msg.append(0xCC)  # interface control message
         else:
             byte_msg.append(0xAA)  # CAN message
         byte_msg += timestamp
 
         # combine the byte arrays into the final message array
         byte_msg += byte_msg_core
         if interface_control:
             byte_msg.append(0xDD)  # interface control message
         else:
             byte_msg.append(0xBB)  # CAN message
-        # <AA><Time 0><Time 1><Time 2><Time 3><DLC><Flags><ID 0><ID 1><ID 2><ID 3><Data 0>...<CRC 0><CRC 1><BB>
+
+        # bt can protocol format:
+        # <AA><Time 0><Time 1><Time 2><Time 3><DLC><Flags><ID 0><ID 1> \
+        # <ID 2><ID 3><Data 0>...<CRC 0><CRC 1><BB>
 
         # Write to serial device
         try:
-            print(byte_msg.hex())
+            # print(byte_msg.hex())
             self._ser.write(byte_msg)
         except serial.PortNotOpenError as error:
             raise CanOperationError("writing to closed port") from error
         except serial.SerialTimeoutException as error:
             raise CanTimeoutError() from error
 
+    def _read_msg_from_buffer(self, dlc) -> Tuple[Optional[Message], bool]:
+        """
+        An internal helper function that reads a CAN message from the class buffer.
+        The identification of a valid message must already have occured elsewhere
+        :raises ValueError: A ValueError is raised when the arbitration ID is
+        outside of the allowable range
+        :raises BusCRCError: A BusCRCError is raised if the bluetooth transmission CRC fails
+        :return: A tuple is returned, containing a message object and a boolean value
+        signifying if the message is from a filter
+        :rtype: (Tuple[Optional[Message], bool])
+        """
+
+        timestamp_bytes = self._rx_byte_buffer[1:5]
+        timestamp = struct.unpack("<I", timestamp_bytes)[0]
+
+        dlc_byte = self._rx_byte_buffer[5:6]
+        flag_int = self._rx_byte_buffer[6]
+
+        id_bytes = self._rx_byte_buffer[7:11]
+        arbitration_id = struct.unpack("<I", id_bytes)[0]
+        if self._raise_exceptions_on_data_errors:
+            if arbitration_id >= 0x20000000:
+                raise ValueError("received arbitration id may not exceed 2^29 (0x20000000)")
+
+        if 0 < dlc <= 8:  # if DLC isnt zero. TODO - allow can_fd?
+            data = self._rx_byte_buffer[11 : 11 + dlc]
+        else:
+            data = b""  # TODO - should this be None?
+
+        # Get the CRC value sent by the adapter
+        sent_crc = struct.unpack("<H", self._rx_byte_buffer[11 + dlc + 1 : 11 + dlc + 3])[0]
+
+        # CRC is calculated on the Timestamp, DLC, flags, ID, and Data bytes
+        if not self.ignore_bt_rx_crc:
+            crc_byte_array = bytearray()  # create a bytearray to store data for CRC
+            crc_byte_array += timestamp_bytes
+            crc_byte_array += dlc_byte
+            crc_byte_array.append(flag_int)  # use append as the value is an int
+            crc_byte_array += id_bytes
+            crc_byte_array += data
+            calc_crc = calculate_crc15(crc_byte_array)
+            if self._raise_exceptions_on_data_errors:
+                if sent_crc != calc_crc:
+                    raise BusCRCError(
+                        f"The message CRC (0x{sent_crc:02x}) and calculated CRC (0x{calc_crc:02x}) don't match\n"
+                        f"message: {self._rx_byte_buffer[1:13 + dlc]}"
+                    )
+
+        # construct the python-can message object
+        msg = Message(
+            # TODO: We are only guessing that they are milliseconds
+            timestamp=self._bus_pc_start_time_s + (timestamp / 1000),
+            arbitration_id=arbitration_id,
+            dlc=dlc,
+            data=data,
+            is_extended_id=(flag_int & 1) == 1,
+            is_error_frame=(flag_int & 2) == 2,
+            is_remote_frame=(flag_int & 4) == 4,
+        )
+
+        # advance the buffer to prevent duplicate message reads
+        self._rx_byte_buffer = self._rx_byte_buffer[1:]
+
+        return msg, False
+
     def _recv_internal(self, timeout: Optional[float]) -> Tuple[Optional[Message], bool]:
         """
         Read a message from the serial device.
 
         :param timeout:
 
             .. warning::
                 This parameter will be ignored. The timeout value of the channel is used.
 
         :returns:
             Received message and :obj:`False` (because no filtering has taken place).
         """
+        buffer_changed = False
         try:
-            rx_byte = self._ser.read()
-            if rx_byte:
-                can_start_byte = ord(rx_byte) == 0xAA
-                interface_start_byte = ord(rx_byte) == 0xCC
-            else:
-                return None, False
-
-            if can_start_byte or interface_start_byte:
-                crc_byte_array = bytearray()  # create a bytearray to store data for CRC
-
-                # read in timestamp bytes
-                timestamp_byte = self._ser.read(4)
-                timestamp = struct.unpack("<I", timestamp_byte)[0]
-
-                # read in DLC byte
-                dlc_byte = self._ser.read()
-                try:
-                    dlc = ord(dlc_byte)
-                except TypeError:
-                    dlc = 0
-                if dlc > 8:
-                    raise ValueError("received DLC may not exceed 8 bytes")
-                crc_byte_array += dlc_byte
-
-                # read in flag byte
-                flag_byte = ord(self._ser.read())
-                is_extended_id = (flag_byte & 1) == 1
-                is_error_frame = (flag_byte & 2) == 1
-                is_remote_frame = (flag_byte & 4) == 1
-                crc_byte_array.append(flag_byte)
-
-                # read in arbitration id
-                id_bytes = self._ser.read(4)
-                arbitration_id = struct.unpack("<I", id_bytes)[0]
-                if arbitration_id >= 0x20000000:
-                    raise ValueError("received arbitration id may not exceed 2^29 (0x20000000)")
-                crc_byte_array += id_bytes
-
-                # read in data bytes
-                data = self._ser.read(dlc)  # read as many bytes as the DLC stated there were
-                crc_byte_array += data
-
-                ser = self._ser.read(2)
-                sent_crc = struct.unpack("<H", ser)[0]
+            # try and fetch enough bytes to fill the FIFO buffer
+            buffer_len = len(self._rx_byte_buffer)
+            rx_bytes = self._ser.read(MAX_BUFFER_LEN - buffer_len)
+        except serial.SerialException as error:
+            raise CanOperationError("could not read from serial") from error
 
-                # CRC is calculated on the DLC, flags, ID, and Data bytes
-                calc_crc = calculate_crc15(crc_byte_array)
-                if sent_crc != calc_crc:
-                    raise BusCRCError(
-                        f"The message CRC (0x{sent_crc:02x}) and calculated CRC (0x{calc_crc:02x}) don't match"
-                    )
+        if rx_bytes:
+            self._rx_byte_buffer += rx_bytes  # put the bytes into the buffer
+            if buffer_len > MAX_BUFFER_LEN:
+                # make sure the buffer stays below the maximum length
+                self._rx_byte_buffer = self._rx_byte_buffer[buffer_len - MAX_BUFFER_LEN :]
+            buffer_changed = True
+        else:  # there were no waiting messages to receive
+            # maximise chance of receiving final bus transmission:
+            if len(self._rx_byte_buffer) > MIN_BUFFER_LEN:
+                # discard the first byte in the buffer
+                self._rx_byte_buffer = self._rx_byte_buffer[1:]
+                buffer_changed = True
+
+        if buffer_changed and (len(self._rx_byte_buffer) >= MIN_BUFFER_LEN):
+            buffer_changed = False
+            can_start_byte = self._rx_byte_buffer[0] == 0xAA
+            interface_start_byte = self._rx_byte_buffer[0] == 0xCC
+        else:
+            return None, False  # either no change or we dont have enough data yet
 
-                delimiter_byte = ord(self._ser.read())
-                if can_start_byte and delimiter_byte == 0xBB:
-                    # received message data okay
-                    msg = Message(
-                        # TODO: We are only guessing that they are milliseconds
-                        timestamp=self._bus_pc_start_time_s + (timestamp / 1000),
-                        arbitration_id=arbitration_id,
-                        dlc=dlc,
-                        data=data,
-                        is_extended_id=is_extended_id,
-                        is_error_frame=is_error_frame,
-                        is_remote_frame=is_remote_frame,
-                    )
-                    return msg, False
-                if interface_start_byte and delimiter_byte == 0xDD:
-                    # received message data okay
-                    msg = Message(
-                        # TODO: We are only guessing that they are milliseconds
-                        timestamp=self._bus_pc_start_time_s + (timestamp / 1000),
-                        arbitration_id=arbitration_id,
-                        dlc=dlc,
-                        data=data,
-                        is_extended_id=is_extended_id,
-                        is_error_frame=is_error_frame,
-                        is_remote_frame=is_remote_frame,
-                    )
-                    return self._process_interface_msg(msg)
-                else:
-                    # TODO: do we actually want to raise the below exception, or just return 'None, False'?
-                    raise CanOperationError(f"invalid delimiter byte while reading message: {delimiter_byte:02x}")
-            else:
-                return None, False
+        # bt can protocol format:
+        # <AA><Time 0><Time 1><Time 2><Time 3><DLC><Flags><ID 0><ID 1> \
+        # <ID 2><ID 3><Data 0>...<CRC 0><CRC 1><BB>
+
+        if can_start_byte or interface_start_byte:
+            dlc = self._rx_byte_buffer[5]
+            if (0 <= dlc <= 8) and (buffer_len >= MIN_BUFFER_LEN + dlc):  # TODO - allow can_fd?
+                # use the dlc value to check if the end byte is present
+                can_end_byte = self._rx_byte_buffer[13 + dlc] == 0xBB
+                interface_end_byte = self._rx_byte_buffer[13 + dlc] == 0xDD
+
+                if can_start_byte and can_end_byte:
+                    return self._read_msg_from_buffer(dlc)
+                if interface_start_byte and interface_end_byte:
+                    return self._process_interface_msg(self._read_msg_from_buffer(dlc))
 
-        except serial.SerialException as error:
-            raise CanOperationError("could not read from serial") from error
+        return None, False  # if a valid message was not identified
 
     def fileno(self) -> int:
         try:
             return self._ser.fileno()
         except io.UnsupportedOperation as ioe:
             raise NotImplementedError("fileno is not implemented using current CAN bus on this platform") from ioe
         except Exception as exception:
@@ -351,38 +434,39 @@
 
     @staticmethod
     def _detect_available_configs() -> List[AutoDetectedConfig]:
         return [{"interface": "bluetooth", "channel": port.device} for port in list_bluetooth_ports()]
 
     def _process_interface_msg(self, message_obj: Message = None) -> Tuple[Optional[Message], bool]:
         """
-        This private function processes any messages from the interface board. Generally these are responses to
-        confiuration requests or IO statuses for some implementations of the bluetooth interface.
+        This private function processes any messages from the interface board. Generally these
+        are responses to confiuration requests or IO statuses for some implementations of the
+        bluetooth interface.
         """
         print("Received interface message:", message_obj)
         # TODO
 
     def set_device_bt_name(self, name: str = "") -> bool:
         """
-        This method sends a message containing a string to the bluetooth CAN adapter. The adapter then changes
-        its name to match the sent string.
+        This method sends a message containing a string to the bluetooth CAN adapter.
+        The adapter then changes its name to match the sent string.
         """
 
         if not isinstance(name, str):
             return False
         name.strip()
         if not name:
             return False
 
         allowed_chars = set(string.ascii_letters + string.digits + "_-")
         if set(name) - allowed_chars:  # if the name contains characters that arent allowed
             raise ValueError(f"The bluetooth name can only contain {allowed_chars}" f"Provided name: '{name}'")
 
-        string_chunk_len = 7  # 7 bytes - the eighth is used as a message counter (i.e. message)
-        string_chunks = [name[i : i + string_chunk_len] for i in range(0, len(name), string_chunk_len)]
+        str_chunk_len = 7  # 7 bytes - the eighth is used as a message counter (i.e. message)
+        string_chunks = [name[i : i + str_chunk_len] for i in range(0, len(name), str_chunk_len)]
         number_of_chunks = len(string_chunks)
 
         if len(string_chunks) > 0xF:
             raise ValueError("The bluetooth name cannot be more than 35 characters")
 
         for i, chunk in enumerate(string_chunks):
             config_msg = Message(arbitration_id=0x002, is_extended_id=False)
@@ -391,15 +475,16 @@
             config_msg.data += chunk.encode("ASCII")
             self.send(config_msg, interface_control=True)
 
         return True
 
     def _send_interface_can_config(self) -> bool:
         """
-        This private function sends the values of the class configuration attributes to the BT interface
+        This private function sends the values of the class configuration attributes to
+        the BT interface
         """
 
         config_msg = Message(arbitration_id=0x001, is_extended_id=False)
         if self.interface_enable_can:  # if the bus is enabled when the update function is called
             if self._state == BusState.ACTIVE:
                 config_bits = (1 << 1) + int(self.interface_enable_can)
             else:
@@ -410,15 +495,16 @@
             config_msg.data += bytearray((0, 0, 0, 0, 0))  # otherwise disable CAN on the interface
 
         self.send(config_msg, interface_control=True)
 
 
 def calculate_crc15(byte_array: bytearray = None):
     """
-    A function that calculates the CRC value for a python-can Message object using the DLC, flags, ID, and Data bytes
+    A function that calculates the CRC value for a python-can Message object using the DLC,
+    flags, ID, and Data bytes
 
     :param byte_array:
         Expects a byte_array (length not specified).
         .. warning::
             There is no type checking in this function as it is only intended
             for internal use in the can-bluetooth module.
```

### Comparing `python-can-bluetooth-0.1.2/can_bluetooth_examples/bluetooth_tx_example.py` & `python-can-bluetooth-0.1.3/can_bluetooth_examples/bluetooth_tx_example.py`

 * *Files identical despite different names*

### Comparing `python-can-bluetooth-0.1.2/can_bluetooth_test/test_interface_bluetooth.py` & `python-can-bluetooth-0.1.3/can_bluetooth_test/test_interface_bluetooth.py`

 * *Files identical despite different names*

### Comparing `python-can-bluetooth-0.1.2/can_bluetooth_test/test_setup.py` & `python-can-bluetooth-0.1.3/can_bluetooth_test/test_setup.py`

 * *Files identical despite different names*

### Comparing `python-can-bluetooth-0.1.2/pyproject.toml` & `python-can-bluetooth-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-can-bluetooth"
-version = "0.1.2"
+version = "0.1.3"
 description = "A python-can interface driver for CAN transmitted over a Bluetooth SPP connection"
 readme = "README.rst"
 license = { text = "GNU Lesser General Public License v3 (LGPLv3)" }
 requires-python = ">=3.7"
 authors = [
     { name = "Matt Woodhead", email = "woody.w62@gmail.com" }
 ]
```

### Comparing `python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/PKG-INFO` & `python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can-bluetooth
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python-can interface driver for CAN transmitted over a Bluetooth SPP connection
 Author-email: Matt Woodhead <woody.w62@gmail.com>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: homepage, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: documentation, https://github.com/MattWoodhead/python-can-bluetooth
 Project-URL: repository, https://github.com/MattWoodhead/python-can-bluetooth
 Keywords: CANbus,Bluetooth,python-can,ESP32
```

### Comparing `python-can-bluetooth-0.1.2/python_can_bluetooth.egg-info/SOURCES.txt` & `python-can-bluetooth-0.1.3/python_can_bluetooth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

