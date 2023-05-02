# Comparing `tmp/NetworkScanner-1.0.1.tar.gz` & `tmp/NetworkScanner-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetworkScanner-1.0.1.tar", last modified: Sat Mar 19 22:29:14 2022, max compression
+gzip compressed data, was "NetworkScanner-2.0.0.tar", last modified: Tue May  2 10:33:52 2023, max compression
```

## Comparing `NetworkScanner-1.0.1.tar` & `NetworkScanner-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-03-19 22:29:14.774095 NetworkScanner-1.0.1/
--rw-r--r--   0 chris     (1000) chris     (1000)    35823 2022-03-13 16:18:30.000000 NetworkScanner-1.0.1/LICENSE.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       29 2022-03-13 16:18:30.000000 NetworkScanner-1.0.1/MANIFEST.in
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2022-03-19 22:29:14.774095 NetworkScanner-1.0.1/NetworkScanner.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     5883 2022-03-19 22:29:14.000000 NetworkScanner-1.0.1/NetworkScanner.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      317 2022-03-19 22:29:14.000000 NetworkScanner-1.0.1/NetworkScanner.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2022-03-19 22:29:14.000000 NetworkScanner-1.0.1/NetworkScanner.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       53 2022-03-19 22:29:14.000000 NetworkScanner-1.0.1/NetworkScanner.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       15 2022-03-19 22:29:14.000000 NetworkScanner-1.0.1/NetworkScanner.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       15 2022-03-19 22:29:14.000000 NetworkScanner-1.0.1/NetworkScanner.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)    35919 2022-03-19 15:49:52.000000 NetworkScanner-1.0.1/NetworkScanner.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5883 2022-03-19 22:29:14.774095 NetworkScanner-1.0.1/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4850 2022-03-18 17:20:10.000000 NetworkScanner-1.0.1/README.md
--rw-r--r--   0 chris     (1000) chris     (1000)       21 2022-03-06 17:21:32.000000 NetworkScanner-1.0.1/requirements.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2022-03-19 22:29:14.774095 NetworkScanner-1.0.1/setup.cfg
--rw-r--r--   0 chris     (1000) chris     (1000)     1719 2022-03-19 15:51:28.000000 NetworkScanner-1.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-02 10:33:52.624050 NetworkScanner-2.0.0/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35823 2023-05-02 12:16:08.000000 NetworkScanner-2.0.0/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       29 2023-05-02 12:16:08.000000 NetworkScanner-2.0.0/MANIFEST.in
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-02 10:33:52.624050 NetworkScanner-2.0.0/NetworkScanner.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     6352 2023-05-02 10:33:52.000000 NetworkScanner-2.0.0/NetworkScanner.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      317 2023-05-02 10:33:52.000000 NetworkScanner-2.0.0/NetworkScanner.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-02 10:33:52.000000 NetworkScanner-2.0.0/NetworkScanner.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       52 2023-05-02 10:33:52.000000 NetworkScanner-2.0.0/NetworkScanner.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-02 10:33:52.000000 NetworkScanner-2.0.0/NetworkScanner.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-02 10:33:52.000000 NetworkScanner-2.0.0/NetworkScanner.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    36022 2023-05-02 14:45:36.000000 NetworkScanner-2.0.0/NetworkScanner.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6352 2023-05-02 10:33:52.624050 NetworkScanner-2.0.0/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     5327 2023-05-02 16:28:50.000000 NetworkScanner-2.0.0/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2023-05-02 12:16:08.000000 NetworkScanner-2.0.0/requirements.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-02 10:33:52.624050 NetworkScanner-2.0.0/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1719 2023-05-02 16:25:40.000000 NetworkScanner-2.0.0/setup.py
```

### Comparing `NetworkScanner-1.0.1/LICENSE.txt` & `NetworkScanner-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NetworkScanner-1.0.1/NetworkScanner.egg-info/PKG-INFO` & `NetworkScanner-2.0.0/NetworkScanner.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetworkScanner
-Version: 1.0.1
+Version: 2.0.0
 Summary: This module implements a NetworkScanner.
 Home-page: https://github.com/mauricelambert/NetworkScanner
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -21,15 +21,15 @@
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![NetworkScanner logo](https://mauricelambert.github.io/info/python/security/NetworkScanner_small.png "NetworkScanner logo")
 
 # NetworkScanner
 
@@ -65,14 +65,15 @@
 ./NetworkScanner.pyz --help
 
 # Python module
 python3 -m NetworkScanner -t 172.18.0.1-172.18.0.15
 
 # Entry point (console)
 NetworkScanner -d --noping --hostname --ports 22 80 -p 445 139 443 -T 1 -R -s -t 172.18.0.0/28
+NetworkScanner -i 172.18.0. -P -t 172.18.0.0/28 # Passive scan using scapy sniffer
 ```
 
 ### Python3
 
 ```python
 # Simple usage to print results in your console
 from NetworkScanner import NetworkScanner, logger
@@ -102,14 +103,15 @@
     def handle_UP(self, ip: str, detection_type: str, details = None): # details is a kwarg
         print(f"IP: {ip} is UP (detection type: {detection_type}, details: {details}")
     def handle_DOWN(self, ip: str):
         print(f"IP: {ip} is DOWN")
 
 scanner = NetworkScanner({"172.18.0.1", "172.18.0.3"})
 scanner.scan()
+scanner.scan(passive=True) # passive mode using scapy sniffer
 ```
 
 ## Useful usages
 
 With scapy, *hosts discovery (best performances)*:
 
 ```bash
@@ -183,37 +185,39 @@
  - [Pypi](https://pypi.org/project/NetworkScanner/)
  - [Documentation](https://mauricelambert.github.io/info/python/security/NetworkScanner.html)
  - [Executable](https://mauricelambert.github.io/info/python/security/NetworkScanner.pyz)
 
 ## Help
 
 ```text
-~# python3 NetworkScanner.py --help
 usage: NetworkScanner.py [-h] [--interface INTERFACE] --targets TARGETS [TARGETS ...] [--noping] [--noarp]
                          [--hostname] [--ports PORTS [PORTS ...]] [--timeout TIMEOUT] [--no-realtime] [--debug]
-                         [--print-state]
+                         [--print-ip] [--force-asynchronous] [--passive-scan]
 
 This program scans networks and IP address ranges.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --interface INTERFACE, -i INTERFACE
                         Part of the IP, MAC or name of the interface
   --targets TARGETS [TARGETS ...], -t TARGETS [TARGETS ...]
                         Targets from networks and IP address ranges.
-  --noping, -P          No ping detection. [Without scapy ping is required for ARP detection]
-  --noarp, -A           No arp detection.
+  --noping, -g          No ping detection. [Without scapy ping is required for ARP detection]
+  --noarp, -A           No arp cache.
   --hostname, -H        Test the hostname resolution to defined if host is UP (longer).
   --ports PORTS [PORTS ...], -p PORTS [PORTS ...]
                         Test the TCP port connections to defined if the host is UP.
   --timeout TIMEOUT, -T TIMEOUT
                         Connections timeout.
   --no-realtime, -R     Do not print results in real time.
   --debug, -d           Debug mode (logger level debug).
-  --print-state, -s     Print IP state (default print IP UP only).
+  --print-ip, -I        Print only the IP address if UP.
+  --force-asynchronous, --async, -a
+                        Force asynchronous mode, using asyncio instead of scapy.
+  --passive-scan, --passive, -P
+                        Passive scan, sniff the network packets to identify who is up. This scan is endless because
+                        you can never be sure to have detected all the IP addresses.
 ```
 
 ## Licence
 
 Licensed under the [GPL, version 3](https://www.gnu.org/licenses/).
-
-
```

### Comparing `NetworkScanner-1.0.1/NetworkScanner.py` & `NetworkScanner-2.0.0/NetworkScanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 ###################
 #    This module implements a NetworkScanner.
-#    Copyright (C) 2021, 2022  Maurice Lambert
+#    Copyright (C) 2021, 2022, 2023  Maurice Lambert
 
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 
 #    This program is distributed in the hope that it will be useful,
@@ -16,47 +16,24 @@
 #    GNU General Public License for more details.
 
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
-This module implements a NetworkScanner.
+This module implements a passive NetworkScanner and an active NetworkScanner
+using ARP and ping scan IP sweep and hostname resolution.
 
 ~# python3 NetworkScanner.py -I -t 172.18.0.1-172.18.0.15
-
-NetworkScanner  Copyright (C) 2021, 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
-
-PythonToolsKit  Copyright (C) 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
 172.18.0.9
 172.18.0.13
 172.18.0.14
 172.18.0.10
 
 ~# python3 NetworkScanner.py -d --async --noping --hostname --ports 22 80 -p 445 139 443 -T 1 -R -t 172.18.0.0/28
-
-NetworkScanner  Copyright (C) 2021, 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
-
-PythonToolsKit  Copyright (C) 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
 [2016-06-22 05:01:12] DEBUG    (10) {__main__ - NetworkScanner.py:490} Build NetworkScanner...
 [2016-06-22 05:01:12] DEBUG    (10) {__main__ - NetworkScanner.py:501} Configure real time...
 [2016-06-22 05:01:12] DEBUG    (10) {__main__ - NetworkScanner.py:509} The scan begins...
 [2016-06-22 05:01:12] INFO     (20) {__main__ - NetworkScanner.py:295} Run asynchronous scan (without scapy).
 [2016-06-22 05:01:12] INFO     (20) {__main__ - NetworkScanner.py:204} Start asynchronous scan without scapy...
 [2016-06-22 05:01:12] DEBUG    (10) {__main__ - NetworkScanner.py:350} Check '172.18.0.11' (step 1: PING)...
 [2016-06-22 05:01:12] DEBUG    (10) {__main__ - NetworkScanner.py:355} Check '172.18.0.11' (step 2: HOSTNAME)...
@@ -117,26 +94,14 @@
 [2016-06-22 05:03:03] DEBUG    (10) {__main__ - NetworkScanner.py:215} Start ARP detection...
 [2016-06-22 05:03:04] INFO     (20) {__main__ - NetworkScanner.py:227} Scan end.
 [2016-06-22 05:03:04] DEBUG    (10) {__main__ - NetworkScanner.py:511} Scan end.
 UP: 172.18.0.9
 DOWN:
 
 ~# python NetworkScanner.py -d -I -t 172.18.0.0/28
-
-NetworkScanner  Copyright (C) 2021, 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
-
-PythonToolsKit  Copyright (C) 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
 [2016-06-22 05:02:24] DEBUG    (10) {__main__ - NetworkScanner.py:651} Build NetworkScanner...
 [2016-06-22 05:02:24] DEBUG    (10) {__main__ - NetworkScanner.py:662} Configure real time...
 [2016-06-22 05:02:24] DEBUG    (10) {__main__ - NetworkScanner.py:670} The scan begins...
 [2016-06-22 05:02:24] INFO     (20) {__main__ - NetworkScanner.py:445} Run scapy scan.
 [2016-06-22 05:02:24] INFO     (20) {__main__ - NetworkScanner.py:385} Start AsyncSniffer using Scapy...
 [2016-06-22 05:02:24] DEBUG    (10) {__main__ - NetworkScanner.py:402} Sending ARP packets...
 [2016-06-22 05:02:24] DEBUG    (10) {__main__ - NetworkScanner.py:309} Send ARP packet for '172.18.0.6'
@@ -203,26 +168,14 @@
 [2016-06-22 05:02:53] DEBUG    (10) {__main__ - NetworkScanner.py:499} Quit handle_DOWN for '172.18.0.6'.
 [2016-06-22 05:02:53] DEBUG    (10) {__main__ - NetworkScanner.py:497} Start handle_DOWN for '172.18.0.2'...
 [2016-06-22 05:02:53] DEBUG    (10) {__main__ - NetworkScanner.py:499} Quit handle_DOWN for '172.18.0.2'.
 [2016-06-22 05:02:53] INFO     (20) {__main__ - NetworkScanner.py:433} Stop AsyncSniffer, scan end.
 [2016-06-22 05:02:53] DEBUG    (10) {__main__ - NetworkScanner.py:672} Scan end.
 
 ~# python NetworkScanner.py --noping --hostname --ports 22 80 -p 445 139 443 -T 1 -R -t 172.18.0.0/28
-
-NetworkScanner  Copyright (C) 2021, 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
-
-PythonToolsKit  Copyright (C) 2022  Maurice Lambert
-This program comes with ABSOLUTELY NO WARRANTY.
-This is free software, and you are welcome to redistribute it
-under certain conditions.
-
 [+] IP: '172.18.0.9' is UP and MAC address is '00:11:22:33:44:55'
 [+] IP: '172.18.0.10' is UP and MAC address is 'aa:bb:cc:dd:ee:ff'
 [-] IP: '172.18.0.13' is DOWN
 [-] IP: '172.18.0.5' is DOWN
 [-] IP: '172.18.0.12' is DOWN
 [-] IP: '172.18.0.14' is DOWN
 [-] IP: '172.18.0.7' is DOWN
@@ -232,14 +185,20 @@
 [-] IP: '172.18.0.6' is DOWN
 [-] IP: '172.18.0.2' is DOWN
 [-] IP: '172.18.0.1' is DOWN
 [-] IP: '172.18.0.8' is DOWN
 
 ~#
 
+~# python NetworkScanner.py -i 172.18.0. -P -t 172.18.0.0/28
+[+] IP: '172.18.0.9' is UP and MAC address is '00:11:22:33:44:55'
+[+] IP: '172.18.0.10' is UP and MAC address is 'aa:bb:cc:dd:ee:ff'
+^C
+~#
+
 >>> from NetworkScanner import NetworkScanner, logger
 >>> scanner = NetworkScanner({"172.18.0.1", "172.18.0.3"})
 >>> scanner.scan()      # Without scapy
 IP: '172.18.0.1' is UP ('ARP', None).
 IP: '172.18.0.3' is UP ('ARP', None).
 [True, True]
 >>> def do_IP_UP(ip, reason, detail = None):
@@ -258,28 +217,32 @@
 >>> scanner = NetworkScanner({"172.18.0.1"}, False, [22, 80], False, True, False, 1, conf.iface)
 >>> scanner.handle_UP = do_IP_UP
 >>> scanner.handle_DOWN = print
 >>> scanner.scan()
 172.18.0.1
 [False]
 >>> logger.setLevel(10)  # debug mode
+>>> scanner.scan(passive=True) # passive scan
 >>>
 """
 
-__version__ = "1.0.1"
+__version__ = "2.0.0"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
-__description__ = "This module implements a NetworkScanner."
+__description__ = """
+This module implements a passive NetworkScanner and an active NetworkScanner
+using ARP and ping scan IP sweep and hostname resolution.
+"""
 license = "GPL-3.0 License"
 __url__ = "https://github.com/mauricelambert/NetworkScanner"
 
 copyright = """
-NetworkScanner  Copyright (C) 2021, 2022  Maurice Lambert
+NetworkScanner  Copyright (C) 2021, 2022, 2023  Maurice Lambert
 This program comes with ABSOLUTELY NO WARRANTY.
 This is free software, and you are welcome to redistribute it
 under certain conditions.
 """
 __license__ = license
 __copyright__ = copyright
 
@@ -311,15 +274,15 @@
 from sys import exit
 
 try:
     from scapy.error import log_runtime
     from scapy.sendrecv import sendp, send
     from scapy.layers.l2 import Ether, ARP
     from scapy.interfaces import NetworkInterface
-    from scapy.all import Packet, IP, ICMP, AsyncSniffer, TCP
+    from scapy.all import Packet, IP, ICMP, AsyncSniffer, TCP, sniff
     from PythonToolsKit.ScapyTools import ScapyArguments as ArgumentParser
 except ImportError:
     NetworkInterface = TypeVar("NetworkInterface")
     Packet = TypeVar("Packet")
     SCAPY = False
 else:
     SCAPY = True
@@ -333,15 +296,14 @@
 error: Callable = logger.error
 critical: Callable = logger.critical
 
 
 async def ping_command(
     command: List[str], ip: str, stdout: int = None
 ) -> bool:
-
     """
     This function executes ping command and checks for success/response.
     """
 
     command = command.copy()
     command.append(ip)
 
@@ -356,15 +318,14 @@
         return False
 
     debug(f"Ping match for {ip}")
     return True
 
 
 def get_linux_arp_cache() -> bytes:
-
     """
     This function returns ARP cache on Linux.
     """
 
     info("Get Linux ARP cache.")
     with open(
         NO_SCAPY_BEHAVIOR.LINUX_ARP_FILE, "r", encoding="latin-1"
@@ -432,52 +393,54 @@
         self.hosts_up = []
         self.hosts_down = []
         self.iface = iface
         self.ip = getattr(iface, "ip", None)
         self.mac = getattr(iface, "mac", None)
 
     def scapy_ping(self, ip: str) -> None:
-
         """
         This function pings a host with Scapy.
         """
 
         debug(f"Send ICMP packet for {ip!r}")
-        send(IP(dst=ip, src=self.ip) / ICMP(), iface=self.iface, verbose=False)
+        sendp(
+            Ether(dst="ff:ff:ff:ff:ff:ff", src=self.mac)
+            / IP(dst=ip, src=self.ip)
+            / ICMP(),
+            iface=self.iface,
+            verbose=False,
+        )
 
     def scapy_arp(self, ip: str) -> None:
-
         """
         This function send an ARP request with Scapy.
         """
 
         debug(f"Send ARP packet for {ip!r}")
         sendp(
             Ether(dst="ff:ff:ff:ff:ff:ff", src=self.mac)
             / ARP(op=1, psrc=self.ip, pdst=ip),
             iface=self.iface,
             verbose=False,
         )
 
     def scapy_tcp(self, ip: str, dport: int, sport: int) -> None:
-
         """
         This function send a TCP packet with Scapy.
         """
 
         debug(f"Send TCP packet for {ip!r}")
         send(
             IP(src=self.ip, dst=ip)
             / TCP(sport=sport, dport=dport, flags="S", seq=1000),
             iface=self.iface,
             verbose=False,
         )
 
     def no_scapy_scan(self) -> List[bool]:
-
         """
         This function starts the scan without scapy.
         """
 
         async def tasks() -> List[bool]:
             return await gather(
                 *[no_scapy_check_ip(target) for target in targets]
@@ -509,15 +472,14 @@
             else:
                 self._handle_DOWN(ip)
 
         info("Scan end.")
         return results
 
     def scapy_match(self, packet: Packet) -> None:
-
         """
         This function gets IP address of matching packets with scapy.
         """
 
         if packet.haslayer(ARP):
             ip = packet[ARP].psrc
             mode = "ARP"
@@ -528,25 +490,25 @@
         debug(f"{mode} detected in packet...")
         targets = self._targets
         if ip in targets:
             targets.remove(ip)
             self._handle_UP(ip, mode, packet[Ether].src)
 
     def start_scapy_scan(self) -> List[bool]:
-
         """
         This function starts AsyncSniffer and scapy scan,
         finally stops AsyncSniffer.
         """
 
         no_error = False
         _targets = self._targets
         info("Start AsyncSniffer using Scapy...")
 
         sniffer = AsyncSniffer(
+        	store=False,
             iface=self.iface,
             lfilter=lambda p: (
                 (ARP in p and p.psrc in _targets)
                 or (IP in p and p.src in _targets)
             ),
             prn=self.scapy_match,
         )
@@ -564,15 +526,14 @@
 
         if no_error:
             return results
         else:
             raise error
 
     def scapy_scan(self) -> List[bool]:
-
         """
         This function starts the scapy scan.
         """
 
         targets = self.targets
 
         scapy_ping = self.scapy_ping
@@ -609,40 +570,60 @@
         results = [
             (handle_DOWN(target) or False) if target not in hosts_up else True
             for target in targets
         ]
 
         return results
 
-    def scan(self, scapy: bool = False) -> List[bool]:
+    def start_passive_scan(self) -> None:
+        """
+        This method starts the passive scan (sniffer).
+        """
+
+        sniff(
+        	store=False,
+            iface=self.iface,
+            lfilter=lambda p: p.haslayer(IP)
+            and p[IP].src in self.targets
+            or p.haslayer(ARP)
+            and p[ARP].psrc in self.targets,
+            prn=self.scapy_match,
+        )
 
+    def scan(self, scapy: bool = False, passive: bool = False) -> List[bool]:
         """
         This function starts the scan (using scapy
         if available otherwise an asynchronous scanner).
         """
 
-        if scapy and SCAPY:
+        if passive and SCAPY:
+            info("Start passive scan.")
+            return self.start_passive_scan()
+        elif passive:
+            raise RuntimeError(
+                "Passive scan require scapy and PythonToolsKit,"
+                " please install requirements first."
+            )
+        elif scapy and SCAPY:
             info("Run scapy scan.")
             return self.start_scapy_scan()
-        else:
-            info("Run asynchronous scan (without scapy).")
-            return self.no_scapy_scan()
 
-    def handle_UP(self, ip: str, reason: str, detail: Any = None) -> None:
+        info("Run asynchronous scan (without scapy).")
+        return self.no_scapy_scan()
 
+    def handle_UP(self, ip: str, reason: str, detail: Any = None) -> None:
         """
         This function is the default behavior when IP is UP.
 
         Print the IP address.
         """
 
         print(f"IP: {ip!r} is UP ({reason!r}, {detail!r}).")
 
     def _handle_UP(self, ip: str, reason: str, detail: Any = None) -> None:
-
         """
         This function is the default behavior when IP is UP.
 
         Store IP address in self.hosts_up and call self.handle_UP.
         """
 
         self.hosts_up.append(ip)
@@ -651,38 +632,35 @@
                 '' if detail is None else detail
             })..."""
         )
         self.handle_UP(ip, reason, detail)
         debug(f"Quit handle_UP for {ip!r}.")
 
     def handle_DOWN(self, ip: str) -> None:
-
         """
         This function is the default behavior when IP is DOWN.
 
         Print the IP address.
         """
 
         print(f"IP: {ip!r} is DOWN.")
 
     def _handle_DOWN(self, ip: str) -> None:
-
         """
         This function is the default behavior when IP is DOWN.
 
         Store IP address in self.hosts_down and call self.handle_DOWN.
         """
 
         self.hosts_down.append(ip)
         debug(f"Start handle_DOWN for {ip!r}...")
         self.handle_DOWN(ip)
         debug(f"Quit handle_DOWN for {ip!r}.")
 
     async def no_scapy_check_ip(self, ip: str) -> bool:
-
         """
         This function checks the IP address to see if it is being used.
         """
 
         if self.ping and await NO_SCAPY_BEHAVIOR.PING(ip):
             debug(f"Check {ip!r} (step 1: PING)...")
             self._handle_UP(ip, "ping")
@@ -716,23 +694,21 @@
 
         debug(f"{ip!r} does not responds to ping/hostname/TCP.")
         return False
 
 
 class ConsoleScanner(NetworkScanner):
     def handle_DOWN(self, ip: str) -> None:
-
         """
         This function prints IP address down using printf.
         """
 
         printf(f"IP: {ip!r} is DOWN", "NOK")
 
     def handle_UP(self, ip: str, reason: str, detail: Any = None) -> None:
-
         """
         This function prints IP address up using printf.
         """
 
         if reason == "tcp":
             printf(f"IP: {ip!r} is UP and port {detail!r} is open.")
         elif reason == "hostname":
@@ -744,15 +720,14 @@
         elif reason == "ARP":
             printf(f"IP: {ip!r} is UP but does not respond to ping.")
         else:
             printf(f"IP: {ip!r} is UP.")
 
 
 def parse_args() -> Namespace:
-
     """
     This function parses the command line arguments.
     """
 
     parser = ArgumentParser(
         description="This program scans networks and IP address ranges."
     )
@@ -765,15 +740,15 @@
         required=True,
         nargs="+",
         action="extend",
         type=get_ipv4_addresses,
     )
     add_argument(
         "--noping",
-        "-P",
+        "-g",
         help=(
             "No ping detection. [Without scapy ping "
             "is required for ARP detection]"
         ),
         action="store_false",
     )
     add_argument("--noarp", "-A", help="No arp cache.", action="store_false")
@@ -820,20 +795,30 @@
     add_argument(
         "--force-asynchronous",
         "--async",
         "-a",
         help="Force asynchronous mode, using asyncio instead of scapy.",
         action="store_true",
     )
+    add_argument(
+        "--passive-scan",
+        "--passive",
+        "-P",
+        help=(
+            "Passive scan, sniff the network packets to identify who is up."
+            " This scan is endless because you can never be sure to have "
+            "detected all the IP addresses."
+        ),
+        action="store_true",
+    )
 
     return parser.parse_args()
 
 
 def main() -> int:
-
     """
     This function executes this program from the command line.
     """
 
     arguments = parse_args()
 
     if arguments.debug:
@@ -861,15 +846,17 @@
         scanner.handle_UP = lambda *args: None
         scanner.handle_DOWN = lambda x: None
     elif print_ip:
         scanner.handle_UP = lambda *args: print(args[0])
         scanner.handle_DOWN = lambda x: None
 
     debug("The scan begins...")
-    scanner.scan(SCAPY and not arguments.force_asynchronous)
+    scanner.scan(
+        SCAPY and not arguments.force_asynchronous, arguments.passive_scan
+    )
     debug("Scan end.")
 
     if no_realtime and print_ip:
         print("\n".join(scanner.hosts_up))
     elif no_realtime:
         print("UP:", "\nUP: ".join(scanner.hosts_up))
         print("DOWN:", "\nDOWN: ".join(scanner.hosts_down))
```

### Comparing `NetworkScanner-1.0.1/PKG-INFO` & `NetworkScanner-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetworkScanner
-Version: 1.0.1
+Version: 2.0.0
 Summary: This module implements a NetworkScanner.
 Home-page: https://github.com/mauricelambert/NetworkScanner
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -21,15 +21,15 @@
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![NetworkScanner logo](https://mauricelambert.github.io/info/python/security/NetworkScanner_small.png "NetworkScanner logo")
 
 # NetworkScanner
 
@@ -65,14 +65,15 @@
 ./NetworkScanner.pyz --help
 
 # Python module
 python3 -m NetworkScanner -t 172.18.0.1-172.18.0.15
 
 # Entry point (console)
 NetworkScanner -d --noping --hostname --ports 22 80 -p 445 139 443 -T 1 -R -s -t 172.18.0.0/28
+NetworkScanner -i 172.18.0. -P -t 172.18.0.0/28 # Passive scan using scapy sniffer
 ```
 
 ### Python3
 
 ```python
 # Simple usage to print results in your console
 from NetworkScanner import NetworkScanner, logger
@@ -102,14 +103,15 @@
     def handle_UP(self, ip: str, detection_type: str, details = None): # details is a kwarg
         print(f"IP: {ip} is UP (detection type: {detection_type}, details: {details}")
     def handle_DOWN(self, ip: str):
         print(f"IP: {ip} is DOWN")
 
 scanner = NetworkScanner({"172.18.0.1", "172.18.0.3"})
 scanner.scan()
+scanner.scan(passive=True) # passive mode using scapy sniffer
 ```
 
 ## Useful usages
 
 With scapy, *hosts discovery (best performances)*:
 
 ```bash
@@ -183,37 +185,39 @@
  - [Pypi](https://pypi.org/project/NetworkScanner/)
  - [Documentation](https://mauricelambert.github.io/info/python/security/NetworkScanner.html)
  - [Executable](https://mauricelambert.github.io/info/python/security/NetworkScanner.pyz)
 
 ## Help
 
 ```text
-~# python3 NetworkScanner.py --help
 usage: NetworkScanner.py [-h] [--interface INTERFACE] --targets TARGETS [TARGETS ...] [--noping] [--noarp]
                          [--hostname] [--ports PORTS [PORTS ...]] [--timeout TIMEOUT] [--no-realtime] [--debug]
-                         [--print-state]
+                         [--print-ip] [--force-asynchronous] [--passive-scan]
 
 This program scans networks and IP address ranges.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --interface INTERFACE, -i INTERFACE
                         Part of the IP, MAC or name of the interface
   --targets TARGETS [TARGETS ...], -t TARGETS [TARGETS ...]
                         Targets from networks and IP address ranges.
-  --noping, -P          No ping detection. [Without scapy ping is required for ARP detection]
-  --noarp, -A           No arp detection.
+  --noping, -g          No ping detection. [Without scapy ping is required for ARP detection]
+  --noarp, -A           No arp cache.
   --hostname, -H        Test the hostname resolution to defined if host is UP (longer).
   --ports PORTS [PORTS ...], -p PORTS [PORTS ...]
                         Test the TCP port connections to defined if the host is UP.
   --timeout TIMEOUT, -T TIMEOUT
                         Connections timeout.
   --no-realtime, -R     Do not print results in real time.
   --debug, -d           Debug mode (logger level debug).
-  --print-state, -s     Print IP state (default print IP UP only).
+  --print-ip, -I        Print only the IP address if UP.
+  --force-asynchronous, --async, -a
+                        Force asynchronous mode, using asyncio instead of scapy.
+  --passive-scan, --passive, -P
+                        Passive scan, sniff the network packets to identify who is up. This scan is endless because
+                        you can never be sure to have detected all the IP addresses.
 ```
 
 ## Licence
 
 Licensed under the [GPL, version 3](https://www.gnu.org/licenses/).
-
-
```

### Comparing `NetworkScanner-1.0.1/README.md` & `NetworkScanner-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 ./NetworkScanner.pyz --help
 
 # Python module
 python3 -m NetworkScanner -t 172.18.0.1-172.18.0.15
 
 # Entry point (console)
 NetworkScanner -d --noping --hostname --ports 22 80 -p 445 139 443 -T 1 -R -s -t 172.18.0.0/28
+NetworkScanner -i 172.18.0. -P -t 172.18.0.0/28 # Passive scan using scapy sniffer
 ```
 
 ### Python3
 
 ```python
 # Simple usage to print results in your console
 from NetworkScanner import NetworkScanner, logger
@@ -71,14 +72,15 @@
     def handle_UP(self, ip: str, detection_type: str, details = None): # details is a kwarg
         print(f"IP: {ip} is UP (detection type: {detection_type}, details: {details}")
     def handle_DOWN(self, ip: str):
         print(f"IP: {ip} is DOWN")
 
 scanner = NetworkScanner({"172.18.0.1", "172.18.0.3"})
 scanner.scan()
+scanner.scan(passive=True) # passive mode using scapy sniffer
 ```
 
 ## Useful usages
 
 With scapy, *hosts discovery (best performances)*:
 
 ```bash
@@ -152,35 +154,39 @@
  - [Pypi](https://pypi.org/project/NetworkScanner/)
  - [Documentation](https://mauricelambert.github.io/info/python/security/NetworkScanner.html)
  - [Executable](https://mauricelambert.github.io/info/python/security/NetworkScanner.pyz)
 
 ## Help
 
 ```text
-~# python3 NetworkScanner.py --help
 usage: NetworkScanner.py [-h] [--interface INTERFACE] --targets TARGETS [TARGETS ...] [--noping] [--noarp]
                          [--hostname] [--ports PORTS [PORTS ...]] [--timeout TIMEOUT] [--no-realtime] [--debug]
-                         [--print-state]
+                         [--print-ip] [--force-asynchronous] [--passive-scan]
 
 This program scans networks and IP address ranges.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --interface INTERFACE, -i INTERFACE
                         Part of the IP, MAC or name of the interface
   --targets TARGETS [TARGETS ...], -t TARGETS [TARGETS ...]
                         Targets from networks and IP address ranges.
-  --noping, -P          No ping detection. [Without scapy ping is required for ARP detection]
-  --noarp, -A           No arp detection.
+  --noping, -g          No ping detection. [Without scapy ping is required for ARP detection]
+  --noarp, -A           No arp cache.
   --hostname, -H        Test the hostname resolution to defined if host is UP (longer).
   --ports PORTS [PORTS ...], -p PORTS [PORTS ...]
                         Test the TCP port connections to defined if the host is UP.
   --timeout TIMEOUT, -T TIMEOUT
                         Connections timeout.
   --no-realtime, -R     Do not print results in real time.
   --debug, -d           Debug mode (logger level debug).
-  --print-state, -s     Print IP state (default print IP UP only).
+  --print-ip, -I        Print only the IP address if UP.
+  --force-asynchronous, --async, -a
+                        Force asynchronous mode, using asyncio instead of scapy.
+  --passive-scan, --passive, -P
+                        Passive scan, sniff the network packets to identify who is up. This scan is endless because
+                        you can never be sure to have detected all the IP addresses.
 ```
 
 ## Licence
 
 Licensed under the [GPL, version 3](https://www.gnu.org/licenses/).
```

### Comparing `NetworkScanner-1.0.1/setup.py` & `NetworkScanner-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="NetworkScanner",
-    version="1.0.1",
+    version="2.0.0",
     py_modules=["NetworkScanner"],
     install_requires=["PythonToolsKit"],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description="This module implements a NetworkScanner.",
@@ -30,15 +30,15 @@
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
     ],
     entry_points={
         "console_scripts": ["NetworkScan = NetworkScanner:main"],
     },
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     keywords=[
         "Network",
         "Scanner",
         "Discovery",
         "Host",
         "Ping",
         "nmap",
```

