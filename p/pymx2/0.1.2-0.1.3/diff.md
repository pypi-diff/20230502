# Comparing `tmp/pymx2-0.1.2.tar.gz` & `tmp/pymx2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymx2-0.1.2.tar", last modified: Fri Apr 28 12:13:27 2023, max compression
+gzip compressed data, was "pymx2-0.1.3.tar", last modified: Tue May  2 15:02:54 2023, max compression
```

## Comparing `pymx2-0.1.2.tar` & `pymx2-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.231017 pymx2-0.1.2/
--rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.2/.gitignore
--rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.2/LICENSE
--rw-r--r--   0 vpaeder    (501) staff       (20)     3501 2023-04-28 12:13:27.230457 pymx2-0.1.2/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)     2749 2023-04-27 12:33:54.000000 pymx2-0.1.2/README.md
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.215235 pymx2-0.1.2/docs/
--rw-r--r--   0 vpaeder    (501) staff       (20)   127613 2023-04-27 12:18:08.000000 pymx2-0.1.2/docs/mx2.enums.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-04-27 12:18:16.000000 pymx2-0.1.2/docs/mx2.exceptions.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    21831 2023-04-27 12:17:38.000000 pymx2-0.1.2/docs/mx2.html
--rw-r--r--   0 vpaeder    (501) staff       (20)     9646 2023-04-27 12:18:12.000000 pymx2-0.1.2/docs/mx2.types.html
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.220393 pymx2-0.1.2/examples/
--rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.2/examples/01_connect.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.2/examples/02_read_write_coil.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.2/examples/03_read_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.2/examples/04_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.2/examples/05_read_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.2/examples/06_data_types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.223231 pymx2-0.1.2/mx2/
--rw-r--r--   0 vpaeder    (501) staff       (20)    31385 2023-04-27 14:23:48.000000 pymx2-0.1.2/mx2/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    48702 2023-04-28 12:11:12.000000 pymx2-0.1.2/mx2/enums.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.2/mx2/exceptions.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    11343 2023-04-27 12:20:33.000000 pymx2-0.1.2/mx2/types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.226009 pymx2-0.1.2/pymx2.egg-info/
--rw-r--r--   0 vpaeder    (501) staff       (20)     3501 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/SOURCES.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/dependency_links.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/requires.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/top_level.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-04-28 12:13:27.231159 pymx2-0.1.2/setup.cfg
--rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-04-28 12:11:32.000000 pymx2-0.1.2/setup.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.229437 pymx2-0.1.2/tests/
--rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.2/tests/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    14195 2023-04-27 14:35:49.000000 pymx2-0.1.2/tests/inverter.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     4509 2023-04-25 14:12:46.000000 pymx2-0.1.2/tests/modbus.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.2/tests/ser.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.2/tests/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:54.003892 pymx2-0.1.3/
+-rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.3/.gitignore
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.3/LICENSE
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-02 15:02:54.003408 pymx2-0.1.3/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2938 2023-04-28 18:35:35.000000 pymx2-0.1.3/README.md
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:53.990566 pymx2-0.1.3/docs/
+-rw-r--r--   0 vpaeder    (501) staff       (20)   214194 2023-05-02 15:01:56.000000 pymx2-0.1.3/docs/mx2.enums.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-05-02 15:02:06.000000 pymx2-0.1.3/docs/mx2.exceptions.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    22217 2023-05-02 15:01:50.000000 pymx2-0.1.3/docs/mx2.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10077 2023-05-02 15:02:00.000000 pymx2-0.1.3/docs/mx2.types.html
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:53.994374 pymx2-0.1.3/examples/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.3/examples/01_connect.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.3/examples/02_read_write_coil.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.3/examples/03_read_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.3/examples/04_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.3/examples/05_read_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.3/examples/06_data_types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:53.997564 pymx2-0.1.3/mx2/
+-rw-r--r--   0 vpaeder    (501) staff       (20)    31996 2023-05-02 14:54:17.000000 pymx2-0.1.3/mx2/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    48702 2023-04-28 12:11:12.000000 pymx2-0.1.3/mx2/enums.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.3/mx2/exceptions.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    11345 2023-05-02 14:57:19.000000 pymx2-0.1.3/mx2/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:54.000048 pymx2-0.1.3/pymx2.egg-info/
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/SOURCES.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/dependency_links.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/requires.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/top_level.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-02 15:02:54.004025 pymx2-0.1.3/setup.cfg
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-05-02 15:01:18.000000 pymx2-0.1.3/setup.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:54.002729 pymx2-0.1.3/tests/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.3/tests/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    15021 2023-05-02 15:00:57.000000 pymx2-0.1.3/tests/inverter.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     4511 2023-05-02 14:58:17.000000 pymx2-0.1.3/tests/modbus.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.3/tests/ser.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.3/tests/types.py
```

### Comparing `pymx2-0.1.2/LICENSE` & `pymx2-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/PKG-INFO` & `pymx2-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,24 +57,32 @@
 An exception is made for fault monitors, for which as specific class method is provided.
 Several examples are available in the [examples](examples) folder.
 API documentation can be found within the code or in the *docs* folder (see [below](#api)).
 Don't hesitate to report bugs [here](https://github.com/vpaeder/pymx2/issues).
 
 ## Setup
 
+You can download a release from pypi using pip or clone this repository and install manually.
+
+### From pypi
+
 From command line, use:
 
 ```bash
-python -m setup.py install
+python -m pip install pymx2
 ```
 
-or for Linux/OSX:
+### From repository
+
+From command line, use:
 
 ```bash
-sudo python -m setup.py install
+git clone https://github.com/vpaeder/pymx2.git
+cd pymx2
+python -m setup.py install
 ```
 
 ## Examples
 
 See [examples](examples) folder.
 
 ## Tests
```

### Comparing `pymx2-0.1.2/README.md` & `pymx2-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -37,24 +37,32 @@
 An exception is made for fault monitors, for which as specific class method is provided.
 Several examples are available in the [examples](examples) folder.
 API documentation can be found within the code or in the *docs* folder (see [below](#api)).
 Don't hesitate to report bugs [here](https://github.com/vpaeder/pymx2/issues).
 
 ## Setup
 
+You can download a release from pypi using pip or clone this repository and install manually.
+
+### From pypi
+
 From command line, use:
 
 ```bash
-python -m setup.py install
+python -m pip install pymx2
 ```
 
-or for Linux/OSX:
+### From repository
+
+From command line, use:
 
 ```bash
-sudo python -m setup.py install
+git clone https://github.com/vpaeder/pymx2.git
+cd pymx2
+python -m setup.py install
 ```
 
 ## Examples
 
 See [examples](examples) folder.
 
 ## Tests
```

### Comparing `pymx2-0.1.2/docs/mx2.exceptions.html` & `pymx2-0.1.3/docs/mx2.exceptions.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/docs/mx2.html` & `pymx2-0.1.3/docs/mx2.html`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 <td colspan=2><tt><a href="#MX2">MX2</a>(port:&nbsp;str&nbsp;=&nbsp;'',&nbsp;baud_rate:&nbsp;int&nbsp;=&nbsp;9600,&nbsp;parity:&nbsp;str&nbsp;=&nbsp;'N')&nbsp;-&amp;gt;&nbsp;None<br>
 &nbsp;<br>
 A&nbsp;driver&nbsp;to&nbsp;control&nbsp;an&nbsp;Omron&nbsp;<a href="#MX2">MX2</a>&nbsp;inverter<br>
 using&nbsp;RS-485&nbsp;(Modbus).<br>
 &nbsp;<br>
 Protected&nbsp;attributes:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;_latency_time(int):&nbsp;additional&nbsp;delay,&nbsp;in&nbsp;ms,&nbsp;between&nbsp;request&nbsp;and&nbsp;response&nbsp;(default:&nbsp;30).<br>
-&nbsp;&nbsp;&nbsp;&nbsp;_wait_time(int):&nbsp;total&nbsp;delay,&nbsp;in&nbsp;ms,&nbsp;between&nbsp;request&nbsp;and&nbsp;response&nbsp;(_latency_time&nbsp;+&nbsp;3.5&nbsp;characters).<br>
+&nbsp;&nbsp;&nbsp;&nbsp;_wait_time(float):&nbsp;total&nbsp;delay,&nbsp;in&nbsp;s,&nbsp;between&nbsp;request&nbsp;and&nbsp;response&nbsp;(_latency_time&nbsp;+&nbsp;3.5&nbsp;characters).<br>
 &nbsp;&nbsp;&nbsp;&nbsp;_last_req_time(float):&nbsp;time&nbsp;when&nbsp;last&nbsp;request&nbsp;was&nbsp;issued.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;_dev_id(int):&nbsp;device&nbsp;ID&nbsp;(default:&nbsp;1).<br>
 &nbsp;&nbsp;&nbsp;&nbsp;_ser(serial.rs485.RS485):&nbsp;Modbus&nbsp;driver&nbsp;instance.<br>&nbsp;</tt></td></tr>
 <tr><td>&nbsp;</td>
 <td width="100%">Methods defined here:<br>
 <dl><dt><a name="MX2-__init__"><strong>__init__</strong></a>(self, port: str = '', baud_rate: int = 9600, parity: str = 'N') -&gt; None</dt><dd><tt>Constructor.<br>
 &nbsp;<br>
@@ -137,19 +137,19 @@
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;read&nbsp;start&nbsp;address&nbsp;is&nbsp;outside&nbsp;bounds.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;write&nbsp;start&nbsp;address&nbsp;is&nbsp;outside&nbsp;bounds.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;read_count&nbsp;is&nbsp;outside&nbsp;bounds.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;len(values)&nbsp;is&nbsp;zero&nbsp;or&nbsp;more&nbsp;than&nbsp;16.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;any&nbsp;of&nbsp;the&nbsp;values&nbsp;is&nbsp;less&nbsp;than&nbsp;0&nbsp;or&nbsp;more&nbsp;than&nbsp;65535.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadResponseLengthException:&nbsp;if&nbsp;response&nbsp;length&nbsp;doesn't&nbsp;match&nbsp;read_count.</tt></dd></dl>
 
-<dl><dt><a name="MX2-read_coil_status"><strong>read_coil_status</strong></a>(self, start_address: mx2.enums.Coil, coil_count: int) -&gt; 'list[CoilValue]'</dt><dd><tt>Read&nbsp;the&nbsp;status&nbsp;of&nbsp;one&nbsp;or&nbsp;more&nbsp;coils.<br>
+<dl><dt><a name="MX2-read_coil_status"><strong>read_coil_status</strong></a>(self, start_address: mx2.enums.Coil, coil_count: int = 1) -&gt; 'list[CoilValue]'</dt><dd><tt>Read&nbsp;the&nbsp;status&nbsp;of&nbsp;one&nbsp;or&nbsp;more&nbsp;coils.<br>
 &nbsp;<br>
 Parameters:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;start_address(Coil):&nbsp;address&nbsp;of&nbsp;1st&nbsp;coil&nbsp;to&nbsp;read.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;coil_count(int):&nbsp;number&nbsp;of&nbsp;coils&nbsp;to&nbsp;query,&nbsp;between&nbsp;1&nbsp;and&nbsp;31.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;coil_count(int):&nbsp;number&nbsp;of&nbsp;coils&nbsp;to&nbsp;query,&nbsp;between&nbsp;1&nbsp;and&nbsp;31&nbsp;(default:&nbsp;1).<br>
 &nbsp;<br>
 Returns:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;list[CoilValue]:&nbsp;the&nbsp;coil&nbsp;states&nbsp;as&nbsp;coil&nbsp;value&nbsp;objects.<br>
 &nbsp;<br>
 Raises:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadRequestException:&nbsp;if&nbsp;device&nbsp;ID&nbsp;is&nbsp;a&nbsp;broadcast&nbsp;address.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;start&nbsp;address&nbsp;is&nbsp;outside&nbsp;bounds.<br>
@@ -165,29 +165,34 @@
 Returns:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;int:&nbsp;fault&nbsp;monitor&nbsp;value.<br>
 &nbsp;<br>
 Raises:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;fault&nbsp;monitor&nbsp;index&nbsp;if&nbsp;outside&nbsp;bounds.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;fault&nbsp;monitor&nbsp;data&nbsp;index&nbsp;is&nbsp;outside&nbsp;bounds.</tt></dd></dl>
 
-<dl><dt><a name="MX2-read_registers"><strong>read_registers</strong></a>(self, start_address: mx2.enums.Register, register_count: int) -&gt; 'list[RegisterValue]'</dt><dd><tt>Read&nbsp;the&nbsp;content&nbsp;of&nbsp;one&nbsp;or&nbsp;more&nbsp;registers.<br>
+<dl><dt><a name="MX2-read_registers"><strong>read_registers</strong></a>(self, start_address: mx2.enums.Register, register_count: int = 1) -&gt; 'list[RegisterValue]'</dt><dd><tt>Read&nbsp;the&nbsp;content&nbsp;of&nbsp;one&nbsp;or&nbsp;more&nbsp;registers.<br>
 &nbsp;<br>
 Parameters:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;start_address(Register):&nbsp;address&nbsp;of&nbsp;1st&nbsp;register&nbsp;to&nbsp;read.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;register_count(int):&nbsp;number&nbsp;of&nbsp;registers&nbsp;to&nbsp;query,&nbsp;from&nbsp;1&nbsp;to&nbsp;16.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;register_count(int):&nbsp;number&nbsp;of&nbsp;registers&nbsp;to&nbsp;query,&nbsp;from&nbsp;1&nbsp;to&nbsp;16&nbsp;(default:&nbsp;1).<br>
 &nbsp;<br>
 Returns:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;list[RegisterValue]:&nbsp;register&nbsp;values&nbsp;as&nbsp;a&nbsp;list&nbsp;of&nbsp;RegisterValue&nbsp;objects.<br>
 &nbsp;<br>
 Raises:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadRequestException:&nbsp;if&nbsp;device&nbsp;ID&nbsp;is&nbsp;a&nbsp;broadcast&nbsp;address.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;start&nbsp;address&nbsp;is&nbsp;outside&nbsp;bounds.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadParameterException:&nbsp;if&nbsp;register&nbsp;count&nbsp;is&nbsp;outside&nbsp;bounds.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;BadResponseLengthException:&nbsp;if&nbsp;response&nbsp;length&nbsp;doesn't&nbsp;match&nbsp;register&nbsp;count.</tt></dd></dl>
 
+<dl><dt><a name="MX2-save_settings_to_eeprom"><strong>save_settings_to_eeprom</strong></a>(self) -&gt; None</dt><dd><tt>Attempt&nbsp;to&nbsp;save&nbsp;modified&nbsp;registers&nbsp;to&nbsp;EEPROM.<br>
+&nbsp;<br>
+Raises:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;MX2Exception:&nbsp;if&nbsp;writing&nbsp;to&nbsp;EEPROM&nbsp;failed.</tt></dd></dl>
+
 <dl><dt><a name="MX2-set_baud_rate"><strong>set_baud_rate</strong></a>(self, baud_rate: int) -&gt; None</dt><dd><tt>Set&nbsp;serial&nbsp;baud&nbsp;rate.&nbsp;Can&nbsp;take&nbsp;the&nbsp;following&nbsp;values:<br>
 &nbsp;&nbsp;&nbsp;2400,&nbsp;4800,&nbsp;9600,&nbsp;19200,&nbsp;38400,&nbsp;57600,&nbsp;76800,&nbsp;115200.<br>
 Must&nbsp;match&nbsp;setting&nbsp;C071&nbsp;of&nbsp;<a href="#MX2">MX2</a>&nbsp;inverter.<br>
 &nbsp;<br>
 Parameters:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;<a href="#MX2-baud_rate">baud_rate</a>(int):&nbsp;serial&nbsp;baud&nbsp;rate.<br>
 &nbsp;<br>
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
              MX2(port: str = '', baud_rate: int = 9600, parity: str = 'N') -&gt; None
               
              A driver to control an Omron MX2 inverter
              using RS-485 (Modbus).
               
              Protected attributes:
                  _latency_time(int): additional delay, in ms, between request and response (default: 30).
-                 _wait_time(int): total delay, in ms, between request and response (_latency_time + 3.5 characters).
+                 _wait_time(float): total delay, in s, between request and response (_latency_time + 3.5 characters).
                  _last_req_time(float): time when last request was issued.
                  _dev_id(int): device ID (default: 1).
                  _ser(serial.rs485.RS485): Modbus driver instance.
               
                Methods defined here:
                  __init__(self, port: str = '', baud_rate: int = 9600, parity: str = 'N') -> None
                      Constructor.
@@ -86,16 +86,16 @@
                          BadResponseException: if response data differs from request.
                  open(self) -> None
                      Open serial connection with MX2 inverter.
                       
                      Raises:
                          SerialException: if connection is already open.
                          SerialException: if connection couldn't be opened.
-                 read_and_write_registers(self, read_start_address: mx2.enums.Register, write_start_address:
-                 mx2.enums.Register, read_count: int, write_values: 'list[int]') -> bytes
+                 read_and_write_registers(self, read_start_address: mx2.enums.Register, write_start_address: mx2.enums.Register,
+                 read_count: int, write_values: 'list[int]') -> bytes
                      Read from and write to one or more registers at once.
                       
                      Parameters:
                          read_start_address(Register): address of 1st register to read.
                          write_start_address(Register): address of 1st register to set.
                          read_count(int): number of registers to query, from 1 to 16.
                          values(list[int]): register values to write.
@@ -107,20 +107,20 @@
                          BadRequestException: if device ID is a broadcast address.
                          BadParameterException: if read start address is outside bounds.
                          BadParameterException: if write start address is outside bounds.
                          BadParameterException: if read_count is outside bounds.
                          BadParameterException: if len(values) is zero or more than 16.
                          BadParameterException: if any of the values is less than 0 or more than 65535.
                          BadResponseLengthException: if response length doesn't match read_count.
-                 read_coil_status(self, start_address: mx2.enums.Coil, coil_count: int) -> 'list[CoilValue]'
+                 read_coil_status(self, start_address: mx2.enums.Coil, coil_count: int = 1) -> 'list[CoilValue]'
                      Read the status of one or more coils.
                       
                      Parameters:
                          start_address(Coil): address of 1st coil to read.
-                         coil_count(int): number of coils to query, between 1 and 31.
+                         coil_count(int): number of coils to query, between 1 and 31 (default: 1).
                       
                      Returns:
                          list[CoilValue]: the coil states as coil value objects.
                       
                      Raises:
                          BadRequestException: if device ID is a broadcast address.
                          BadParameterException: if start address is outside bounds.
@@ -135,37 +135,42 @@
                       
                      Returns:
                          int: fault monitor value.
                       
                      Raises:
                          BadParameterException: if fault monitor index if outside bounds.
                          BadParameterException: if fault monitor data index is outside bounds.
-                 read_registers(self, start_address: mx2.enums.Register, register_count: int) -> 'list[RegisterValue]'
+                 read_registers(self, start_address: mx2.enums.Register, register_count: int = 1) -> 'list[RegisterValue]'
                      Read the content of one or more registers.
                       
                      Parameters:
                          start_address(Register): address of 1st register to read.
-                         register_count(int): number of registers to query, from 1 to 16.
+                         register_count(int): number of registers to query, from 1 to 16 (default: 1).
                       
                      Returns:
                          list[RegisterValue]: register values as a list of RegisterValue objects.
                       
                      Raises:
                          BadRequestException: if device ID is a broadcast address.
                          BadParameterException: if start address is outside bounds.
                          BadParameterException: if register count is outside bounds.
-   �                 BadResponseLengthException: if response length doesn't match register count.
+                         BadResponseLengthException: if response length doesn't match register count.
+                 save_settings_to_eeprom(self) -> None
+   �             Attempt to save modified registers to EEPROM.
+                      
+                  Raises:
+                         MX2Exception: if writing to EEPROM failed.
                  set_baud_rate(self, baud_rate: int) -> None
-                  Set serial baud rate. Can take the following values:
+                     Set serial baud rate. Can take the following values:
                         2400, 4800, 9600, 19200, 38400, 57600, 76800, 115200.
                      Must match setting C071 of MX2 inverter.
-                      
+                     
                      Parameters:
                          baud_rate(int): serial baud rate.
-                     
+                      
                      Raises:
                          SerialException: if connection is already open.
                          BadParameterException: if baud rate is invalid.
                  set_device_id(self, dev_id: int) -> None
                      Set device ID. This can be between 1 and 247 for
                      single device or between 250 and 254 for broadcast and
                      must match setting C072 of MX2 inverter.
@@ -247,18 +252,18 @@
                          value(int): value to set, from 0 to 65535.
                       
                      Raises:
                          BadParameterException: if address is outside bounds.
                          BadParameterException: if value is outside bounds.
                          BadResponseLengthException: if response length isn't 8.
                          BadResponseException: if response data differs from request.
-               ================================================================================================================
+               =====================================================================================================================
                Readonly properties defined here:
                  is_open
-               ================================================================================================================
+               =====================================================================================================================
                Data descriptors defined here:
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
                  baud_rate
                      Get serial baud rate.
```

### Comparing `pymx2-0.1.2/docs/mx2.types.html` & `pymx2-0.1.3/docs/mx2.types.html`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 
 <dl><dt><a name="RegisterValue-__ilshift__"><strong>__ilshift__</strong></a>(self, amount) -&gt; 'RegisterValue'</dt></dl>
 
 <dl><dt><a name="RegisterValue-__imod__"><strong>__imod__</strong></a>(self, other) -&gt; 'RegisterValue'</dt></dl>
 
 <dl><dt><a name="RegisterValue-__imul__"><strong>__imul__</strong></a>(self, other) -&gt; 'RegisterValue'</dt></dl>
 
-<dl><dt><a name="RegisterValue-__init__"><strong>__init__</strong></a>(self, register: mx2.enums.Register, value: int)</dt><dd><tt>Initialize&nbsp;self.&nbsp;&nbsp;See&nbsp;help(type(self))&nbsp;for&nbsp;accurate&nbsp;signature.</tt></dd></dl>
+<dl><dt><a name="RegisterValue-__index__"><strong>__index__</strong></a>(self) -&gt; int</dt></dl>
 
-<dl><dt><a name="RegisterValue-__int__"><strong>__int__</strong></a>(self) -&gt; int</dt></dl>
+<dl><dt><a name="RegisterValue-__init__"><strong>__init__</strong></a>(self, register: mx2.enums.Register, value: int)</dt><dd><tt>Initialize&nbsp;self.&nbsp;&nbsp;See&nbsp;help(type(self))&nbsp;for&nbsp;accurate&nbsp;signature.</tt></dd></dl>
 
 <dl><dt><a name="RegisterValue-__inv__"><strong>__inv__</strong></a>(self) -&gt; int</dt></dl>
 
 <dl><dt><a name="RegisterValue-__ior__"><strong>__ior__</strong></a>(self, other) -&gt; 'RegisterValue'</dt></dl>
 
 <dl><dt><a name="RegisterValue-__ipow__"><strong>__ipow__</strong></a>(self, other) -&gt; 'RegisterValue'</dt></dl>
 
@@ -166,9 +166,16 @@
 <dl><dt><strong>__weakref__</strong></dt>
 <dd><tt>list&nbsp;of&nbsp;weak&nbsp;references&nbsp;to&nbsp;the&nbsp;object&nbsp;(if&nbsp;defined)</tt></dd>
 </dl>
 <hr>
 Data and other attributes defined here:<br>
 <dl><dt><strong>__hash__</strong> = None</dl>
 
-</td></tr></table></td></tr></table>
+</td></tr></table></td></tr></table><p>
+<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
+<tr bgcolor="#55aa55">
+<td colspan=3 valign=bottom>&nbsp;<br>
+<font color="#ffffff" face="helvetica, arial"><big><strong>Data</strong></big></font></td></tr>
+    
+<tr><td bgcolor="#55aa55"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
+<td width="100%"><strong>__all__</strong> = ['CoilValue', 'RegisterValue']</td></tr></table>
 </body></html>
```

#### html2text {}

```diff
@@ -60,17 +60,17 @@
                      Return self>value.
                  __iadd__(self, other) -> 'RegisterValue'
                  __iand__(self, other) -> 'RegisterValue'
                  __ifloordiv__(self, other) -> 'RegisterValue'
                  __ilshift__(self, amount) -> 'RegisterValue'
                  __imod__(self, other) -> 'RegisterValue'
                  __imul__(self, other) -> 'RegisterValue'
+                 __index__(self) -> int
                  __init__(self, register: mx2.enums.Register, value: int)
                      Initialize self.  See help(type(self)) for accurate signature.
-                 __int__(self) -> int
                  __inv__(self) -> int
                  __ior__(self, other) -> 'RegisterValue'
                  __ipow__(self, other) -> 'RegisterValue'
               __irshift__(self, amount) -> 'RegisterValue'
                  __isub__(self, other) -> 'RegisterValue'
                  __ixor__(self, other) -> 'RegisterValue'
                  __le__(self, other) -> bool
@@ -99,7 +99,10 @@
                  __dict__
                      dictionary for instance variables (if defined)
                  __weakref__
                      list of weak references to the object (if defined)
                ======================================================================================
                Data and other attributes defined here:
                  __hash__ = None
+ 
+Data
+   � __all__ = ['CoilValue', 'RegisterValue']
```

### Comparing `pymx2-0.1.2/examples/02_read_write_coil.py` & `pymx2-0.1.3/examples/02_read_write_coil.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/examples/03_read_registers.py` & `pymx2-0.1.3/examples/03_read_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/examples/04_write_registers.py` & `pymx2-0.1.3/examples/04_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/examples/05_read_write_registers.py` & `pymx2-0.1.3/examples/05_read_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/examples/06_data_types.py` & `pymx2-0.1.3/examples/06_data_types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/mx2/__init__.py` & `pymx2-0.1.3/mx2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 """
 import serial
 from serial.rs485 import RS485
 from time import time, sleep
 
 __all__ = ["MX2"]
 
-from .enums import FunctionCode, ExceptionCode, Coil, Register, MonitoringFunctions, FaultMonitorData
+from .enums import FunctionCode, ExceptionCode, Coil, Register, MonitoringFunctions,\
+                   FaultMonitorData, ModbusRegisters, TripFactor
 from .exceptions import *
 from .types import CoilValue, RegisterValue
 
 
 def crc16(data:bytes) -> bytes:
     """Compute CRC-16-Modbus of a byte string.
 
@@ -46,21 +47,21 @@
 
 class MX2():
     """A driver to control an Omron MX2 inverter
     using RS-485 (Modbus).
     
     Protected attributes:
         _latency_time(int): additional delay, in ms, between request and response (default: 30).
-        _wait_time(int): total delay, in ms, between request and response (_latency_time + 3.5 characters).
+        _wait_time(float): total delay, in s, between request and response (_latency_time + 3.5 characters).
         _last_req_time(float): time when last request was issued.
         _dev_id(int): device ID (default: 1).
         _ser(serial.rs485.RS485): Modbus driver instance.
     """
     _latency_time = 30
-    _wait_time = 30 + int(11*3500/9600)
+    _wait_time = 0.030 + 11*3.5/9600
     _last_req_time = 0
     _dev_id = 1
     _ser = None
 
     def __init__(self, port:str="", baud_rate:int=9600, parity:str=serial.PARITY_NONE) -> None:
         """Constructor.
         
@@ -121,15 +122,15 @@
             SerialException: if connection is already open.
             BadParameterException: if baud rate is invalid.
         """
         if self._ser.is_open:
             raise SerialException("Connection is currently open.")
         if baud_rate in [2400, 4800, 9600, 19200, 38400, 57600, 76800, 115200]:
             self._ser.baudrate = baud_rate
-            self._wait_time = self._latency_time + int(11*3500/baud_rate)
+            self._wait_time = self._latency_time/1000.0 + 11*3.5/baud_rate
         else:
             raise BadParameterException("Invalid baud rate.")
     
     baud_rate = property(get_baud_rate, set_baud_rate)
 
     def get_parity(self) -> str:
         """Get serial parity.
@@ -229,15 +230,15 @@
     def set_latency_time(self, latency_time:int) -> None:
         """Set latency time, betweeen 0 and 1000 ms.
         Must be at least as much as setting C078 of MX2 inverter.
         In case device returns no data, try increasing this.
         """
         if latency_time>=0 and latency_time<=1000:
             self._latency_time = latency_time
-            self._wait_time = latency_time + int(11*3500/self._ser.baudrate)
+            self._wait_time = latency_time/1000.0 + 11*3.5/self._ser.baudrate
         else:
             raise BadParameterException("Latency can be between 0 and 1000 ms.")
     
     latency_time = property(get_latency_time, set_latency_time)
 
     def get_device_id(self) -> int:
         """Get device ID.
@@ -280,15 +281,15 @@
         self._ser.write(request)
         self._last_req_time = time()
     
 
     def _wait(self) -> None:
         """Wait, if necessary, until enough time has elapsed
         after previous request."""
-        rem_time = self._wait_time/1000.0 - time() + self._last_req_time
+        rem_time = self._wait_time - time() + self._last_req_time
         if rem_time<=0:
             return
         sleep(rem_time)
 
 
     def _read(self) -> bytes:
         """Read incoming bytes.
@@ -350,20 +351,20 @@
                     raise ReadOnlyTargetException("Target is read-only.")
                 else:
                     raise MX2Exception("Unknown exception.")
             else:
                 raise BadResponseException("Data issued for incorrect function code.")
     
 
-    def read_coil_status(self, start_address:Coil, coil_count:int) -> 'list[CoilValue]':
+    def read_coil_status(self, start_address:Coil, coil_count:int=1) -> 'list[CoilValue]':
         """Read the status of one or more coils.
 
         Parameters:
             start_address(Coil): address of 1st coil to read.
-            coil_count(int): number of coils to query, between 1 and 31.
+            coil_count(int): number of coils to query, between 1 and 31 (default: 1).
         
         Returns:
             list[CoilValue]: the coil states as coil value objects.
         
         Raises:
             BadRequestException: if device ID is a broadcast address.
             BadParameterException: if start address is outside bounds.
@@ -434,20 +435,20 @@
                         addr = addr.next()[0]
                     except IndexError:
                         break
                     nb = addr.n_words
         return values
 
 
-    def read_registers(self, start_address:Register, register_count:int) -> 'list[RegisterValue]':
+    def read_registers(self, start_address:Register, register_count:int=1) -> 'list[RegisterValue]':
         """Read the content of one or more registers.
 
         Parameters:
             start_address(Register): address of 1st register to read.
-            register_count(int): number of registers to query, from 1 to 16.
+            register_count(int): number of registers to query, from 1 to 16 (default: 1).
         
         Returns:
             list[RegisterValue]: register values as a list of RegisterValue objects.
 
         Raises:
             BadRequestException: if device ID is a broadcast address.
             BadParameterException: if start address is outside bounds.
@@ -804,7 +805,20 @@
 
         if value in [FaultMonitorData.Frequency, FaultMonitorData.RunningTime, FaultMonitorData.PowerOnTime]:
             result = self.read_registers(addr, 2)
             return (result[0] << 16) + result[1]
         else:
             result = self.read_registers(addr, 1)
             return result[0]
+
+
+    def save_settings_to_eeprom(self) -> None:
+        """Attempt to save modified registers to EEPROM.
+        
+        Raises:
+            MX2Exception: if writing to EEPROM failed.
+        """
+        self.write_in_register(ModbusRegisters.WriteToEEPROM, 1)
+        while self.read_coil_status(Coil.DataWritingInProgress, 1)[0] == True:
+            sleep(self._wait_time)
+            if self.read_registers(MonitoringFunctions.FaultMonitor1, 1)[0] == TripFactor.EEPROMError:
+                raise MX2Exception("EEPROM write failed.")
```

### Comparing `pymx2-0.1.2/mx2/enums.py` & `pymx2-0.1.3/mx2/enums.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/mx2/exceptions.py` & `pymx2-0.1.3/mx2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/mx2/types.py` & `pymx2-0.1.3/mx2/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if not isinstance(register, Register):
             raise TypeError("Incompatible type given for register.")
         if not isinstance(value, int):
             raise TypeError("Value must be integer.")
         self.register = register
         self.value = value
     
-    def __int__(self) -> int:
+    def __index__(self) -> int:
         return self.value
     
     def __eq__(self, other) -> bool:
         if isinstance(other, int):
             return self.value == other
         elif isinstance(other, RegisterValue):
             return self.value == other.value and self.register == other.register
```

### Comparing `pymx2-0.1.2/pymx2.egg-info/PKG-INFO` & `pymx2-0.1.3/pymx2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,24 +57,32 @@
 An exception is made for fault monitors, for which as specific class method is provided.
 Several examples are available in the [examples](examples) folder.
 API documentation can be found within the code or in the *docs* folder (see [below](#api)).
 Don't hesitate to report bugs [here](https://github.com/vpaeder/pymx2/issues).
 
 ## Setup
 
+You can download a release from pypi using pip or clone this repository and install manually.
+
+### From pypi
+
 From command line, use:
 
 ```bash
-python -m setup.py install
+python -m pip install pymx2
 ```
 
-or for Linux/OSX:
+### From repository
+
+From command line, use:
 
 ```bash
-sudo python -m setup.py install
+git clone https://github.com/vpaeder/pymx2.git
+cd pymx2
+python -m setup.py install
 ```
 
 ## Examples
 
 See [examples](examples) folder.
 
 ## Tests
```

### Comparing `pymx2-0.1.2/pymx2.egg-info/SOURCES.txt` & `pymx2-0.1.3/pymx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/setup.py` & `pymx2-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymx2",
-    version="0.1.2",
+    version="0.1.3",
     author="Vincent Paeder",
     author_email="python@paeder.fi",
     description="A Python driver to communicate with an Omron MX2 inverter through Modbus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['omron', 'mx2', 'inverter'],
     url="https://github.com/vpaeder/pymx2",
```

### Comparing `pymx2-0.1.2/tests/inverter.py` & `pymx2-0.1.3/tests/inverter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 from unittest.mock import Mock
 import mx2
 from mx2.exceptions import *
 from mx2.enums import FunctionCode, ExceptionCode, Coil, MonitoringFunctions,\
                       StandardFunctions, MainProfileParameters
+from mx2.types import CoilValue, RegisterValue
 
 
 class TestInverter(unittest.TestCase):
     def setUp(self):
         self.mx = mx2.MX2()
         self.mx._ser = Mock()
         self.mx._ser.write = Mock()
@@ -238,7 +239,21 @@
             self.mx.read_fault_monitor(0, 0)
         with self.assertRaises(BadParameterException):
             self.mx.read_fault_monitor(7, 0)
         with self.assertRaises(BadParameterException):
             self.mx.read_fault_monitor(1, -1)
         with self.assertRaises(BadParameterException):
             self.mx.read_fault_monitor(1, 10)
+
+    def test_save_settings_to_eeprom_ok(self):
+        self.mx.read_coil_status = Mock(return_value=[CoilValue(Coil.DataWritingInProgress, False)])
+        self.mx._dev_id = 8
+        self.mx._ser.read.return_value = bytes([8, 6, 0x08, 0xff, 0, 1, 0x7A, 0xC3])
+        self.mx.save_settings_to_eeprom()
+        
+    def test_save_settings_to_eeprom_fail(self):
+        self.mx.read_coil_status = Mock(return_value=[CoilValue(Coil.DataWritingInProgress, True)])
+        self.mx.read_registers = Mock(return_value=[RegisterValue(MonitoringFunctions.FaultMonitor1Factor, 8)])
+        self.mx._ser.read.return_value = bytes([8, 6, 0x08, 0xff, 0, 1, 0x7A, 0xC3])
+        self.mx._dev_id = 8
+        with self.assertRaises(MX2Exception):
+            self.mx.save_settings_to_eeprom()
```

### Comparing `pymx2-0.1.2/tests/modbus.py` & `pymx2-0.1.3/tests/modbus.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     
     def test_set_latency_time_ok(self):
         self.mx._ser.is_open = False
         for t in range(0,1001):
             self.mx.set_latency_time(t)
             self.assertEqual(self.mx.get_latency_time(), t)
             self.mx.set_baud_rate(9600)
-            self.assertEqual(self.mx._wait_time, t + int(11*3500/self.mx.get_baud_rate()))
+            self.assertEqual(self.mx._wait_time, t/1000.0 + 11*3.5/self.mx.get_baud_rate())
             self.mx.set_baud_rate(2400)
-            self.assertEqual(self.mx._wait_time, t + int(11*3500/self.mx.get_baud_rate()))
+            self.assertEqual(self.mx._wait_time, t/1000.0 + 11*3.5/self.mx.get_baud_rate())
     
     def test_set_latency_time_fail(self):
         for t in [-100, 1100]:
             with self.assertRaises(BadParameterException):
                 self.mx.set_latency_time(t)
             self.assertNotEqual(self.mx.get_latency_time(), t)
```

### Comparing `pymx2-0.1.2/tests/ser.py` & `pymx2-0.1.3/tests/ser.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.2/tests/types.py` & `pymx2-0.1.3/tests/types.py`

 * *Files identical despite different names*

