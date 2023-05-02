# Comparing `tmp/pipecheck-0.4.1.tar.gz` & `tmp/pipecheck-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipecheck-0.4.1.tar", max compression
+gzip compressed data, was "pipecheck-0.4.2.tar", max compression
```

## Comparing `pipecheck-0.4.1.tar` & `pipecheck-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2022-07-25 08:09:50.806541 pipecheck-0.4.1/LICENSE
--rw-r--r--   0        0        0       22 2022-07-25 08:09:50.806541 pipecheck-0.4.1/pipecheck/__init__.py
--rwxr-xr-x   0        0        0     4091 2022-07-25 08:09:50.806541 pipecheck-0.4.1/pipecheck/__main__.py
--rw-r--r--   0        0        0      981 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/api.py
--rw-r--r--   0        0        0      274 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/checks/__init__.py
--rw-r--r--   0        0        0     1184 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/checks/dns.py
--rw-r--r--   0        0        0     2608 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/checks/http.py
--rw-r--r--   0        0        0      583 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/checks/icmp.py
--rw-r--r--   0        0        0      662 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/checks/tcp.py
--rw-r--r--   0        0        0     2956 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/cli.py
--rw-r--r--   0        0        0     1147 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/cli_backport.py
--rw-r--r--   0        0        0      254 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/cmdfile.py
--rw-r--r--   0        0        0      680 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pipecheck/utils.py
--rw-r--r--   0        0        0     1156 2022-07-25 08:09:50.810541 pipecheck-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      890 2022-07-25 08:10:52.371343 pipecheck-0.4.1/setup.py
--rw-r--r--   0        0        0      879 2022-07-25 08:10:52.371645 pipecheck-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 15:37:20.944762 pipecheck-0.4.2/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-02 15:37:59.725248 pipecheck-0.4.2/pipecheck/__init__.py
+-rwxr-xr-x   0        0        0     4204 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/__main__.py
+-rw-r--r--   0        0        0      981 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/api.py
+-rw-r--r--   0        0        0      332 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/checks/__init__.py
+-rw-r--r--   0        0        0     1184 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/checks/dns.py
+-rw-r--r--   0        0        0     2608 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/checks/http.py
+-rw-r--r--   0        0        0      583 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/checks/icmp.py
+-rw-r--r--   0        0        0      988 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/checks/mysql.py
+-rw-r--r--   0        0        0      662 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/checks/tcp.py
+-rw-r--r--   0        0        0     3504 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/cli.py
+-rw-r--r--   0        0        0     1146 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/cli_backport.py
+-rw-r--r--   0        0        0      254 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/cmdfile.py
+-rw-r--r--   0        0        0      680 2023-05-02 15:37:20.948762 pipecheck-0.4.2/pipecheck/utils.py
+-rw-r--r--   0        0        0     1444 2023-05-02 15:37:59.725248 pipecheck-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 pipecheck-0.4.2/PKG-INFO
```

### Comparing `pipecheck-0.4.1/LICENSE` & `pipecheck-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipecheck-0.4.1/pipecheck/__main__.py` & `pipecheck-0.4.2/pipecheck/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,22 +119,26 @@
 
 if __name__ == "__main__":
     args = parse_args()
 
     if not supports_color() or ("no_color" in args and args["no_color"]):
         no_color = True
 
+    sys.tracebacklimit = 0
+    if "verbose" in args and args["verbose"]:
+        sys.tracebacklimit = None
+
     calls = list(gen_calls(args))
     if len(calls) <= 0:
         print_error("No probes specified")
         sys.exit(0)
 
     last_status = 0
     if "interval" in args and args["interval"]:
-        start_http_server(args["port"])
+        start_http_server(args["prom_port"])
 
         signal.signal(signal.SIGINT, signal_handler)
         signal.signal(signal.SIGTERM, signal_handler)
 
         while True:
             last_status = run(calls)
             time.sleep(float(args["interval"]))
```

### Comparing `pipecheck-0.4.1/pipecheck/api.py` & `pipecheck-0.4.2/pipecheck/api.py`

 * *Files identical despite different names*

### Comparing `pipecheck-0.4.1/pipecheck/checks/dns.py` & `pipecheck-0.4.2/pipecheck/checks/dns.py`

 * *Files identical despite different names*

### Comparing `pipecheck-0.4.1/pipecheck/checks/http.py` & `pipecheck-0.4.2/pipecheck/checks/http.py`

 * *Files identical despite different names*

### Comparing `pipecheck-0.4.1/pipecheck/checks/icmp.py` & `pipecheck-0.4.2/pipecheck/checks/icmp.py`

 * *Files identical despite different names*

### Comparing `pipecheck-0.4.1/pipecheck/checks/tcp.py` & `pipecheck-0.4.2/pipecheck/checks/tcp.py`

 * *Files identical despite different names*

### Comparing `pipecheck-0.4.1/pipecheck/cli.py` & `pipecheck-0.4.2/pipecheck/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+from urllib.parse import urlparse
 
 from pipecheck import __version__
 from pipecheck.checks import probes
 from pipecheck.cli_backport import BooleanOptionalAction
 
 
 def parse_args(args=None):
@@ -41,15 +42,15 @@
         "--interval",
         nargs="?",
         const=5,
         type=int,
         help="don't exit but repeat checks in given interval. Also activates prometheus exporter",
     )
 
-    parser.add_argument("-p", "--port", nargs="?", default=9000, type=int, help="promtheus exporter port")
+    parser.add_argument("-p", "--prom-port", nargs="?", default=9000, type=int, help="promtheus exporter port")
 
     for probe in probes:
         parser.add_argument("--%s" % probes[probe].get_type(), nargs="*", help=probes[probe].get_help())
 
     return vars(parser.parse_args(args=args))
 
 
@@ -67,14 +68,33 @@
 
 
 def parse_tcp(x):
     (host, port) = x.split(":")
     return {"type": "tcp", "host": host, "port": int(port)}
 
 
+def parse_mysql(x):
+    if not x.startswith("mysql://"):
+        x = "mysql://" + x
+    try:
+        u = urlparse(x)
+        o = {
+            "type": "mysql",
+            "host": u.hostname,
+            "user": u.username,
+            "password": u.password,
+            "database": str(u.path).removeprefix("/"),
+        }
+        if u.port:
+            o["port"] = int(u.port)
+        return o
+    except Exception as e:
+        raise Exception(f"Unable to parse mysql-probe target-url ({e})") from None
+
+
 def parse_http(x):
     return {"type": "http", "url": x}
 
 
 def parse_ping(x):
     return {"type": "ping", "host": x}
```

### Comparing `pipecheck-0.4.1/pipecheck/cli_backport.py` & `pipecheck-0.4.2/pipecheck/cli_backport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from argparse import Action
 
 
 class BooleanOptionalAction(Action):
     def __init__(self, option_strings, dest, default=None, type=None, choices=None, required=False, help=None, metavar=None):
-
         _option_strings = []
         for option_string in option_strings:
             _option_strings.append(option_string)
 
             if option_string.startswith("--"):
                 option_string = "--no-" + option_string[2:]
                 _option_strings.append(option_string)
```

### Comparing `pipecheck-0.4.1/pipecheck/utils.py` & `pipecheck-0.4.2/pipecheck/utils.py`

 * *Files identical despite different names*

### Comparing `pipecheck-0.4.1/PKG-INFO` & `pipecheck-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pipecheck
-Version: 0.4.1
+Version: 0.4.2
 Summary: This simple tool can be used to verify the state of a system's context.
 License: MIT
 Author: Michael Riedmann
 Author-email: michael_riedmann@live.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
-Requires-Dist: certifi (>=2021.5.30,<2022.0.0)
+Requires-Dist: certifi (>=2021.5.30,<2023.0.0)
 Requires-Dist: icmplib (>=3.0,<4.0)
 Requires-Dist: netaddr (>=0.8.0,<0.9.0)
 Requires-Dist: prometheus-client (>=0.11.0,<0.12.0)
+Requires-Dist: pymysql (>=1.0.3,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: urllib3 (>=1.26.5,<2.0.0)
```

