# Comparing `tmp/nornir_srl-0.1.1.tar.gz` & `tmp/nornir_srl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_srl-0.1.1.tar", max compression
+gzip compressed data, was "nornir_srl-0.1.2.tar", max compression
```

## Comparing `nornir_srl-0.1.1.tar` & `nornir_srl-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    12132 2023-04-26 13:29:14.866549 nornir_srl-0.1.1/README.md
--rw-r--r--   0        0        0       22 2022-11-20 12:27:33.451929 nornir_srl-0.1.1/nornir_srl/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 18:28:42.918760 nornir_srl-0.1.1/nornir_srl/connections/__init__.py
--rw-r--r--   0        0        0     3854 2023-04-27 15:04:05.839013 nornir_srl-0.1.1/nornir_srl/connections/helpers.py
--rw-r--r--   0        0        0    22336 2023-04-28 14:58:03.317817 nornir_srl-0.1.1/nornir_srl/connections/srlinux.py
--rw-r--r--   0        0        0     9593 2023-04-28 15:22:20.913311 nornir_srl-0.1.1/nornir_srl/fsc.py
--rw-r--r--   0        0        0        0 2022-10-30 22:33:33.108689 nornir_srl-0.1.1/nornir_srl/tasks/__init__.py
--rw-r--r--   0        0        0      373 2022-11-25 22:31:43.343296 nornir_srl-0.1.1/nornir_srl/tasks/helpers.py
--rw-r--r--   0        0        0     8844 2023-01-03 20:18:09.232105 nornir_srl-0.1.1/nornir_srl/tasks/srl_config.py
--rw-r--r--   0        0        0      846 2023-04-28 15:33:39.158264 nornir_srl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    13562 2023-04-28 15:33:46.522847 nornir_srl-0.1.1/setup.py
--rw-r--r--   0        0        0    13142 2023-04-28 15:33:46.523670 nornir_srl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    12132 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/nornir_srl/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/nornir_srl/connections/__init__.py
+-rw-r--r--   0        0        0     3854 2023-05-02 12:36:36.599945 nornir_srl-0.1.2/nornir_srl/connections/helpers.py
+-rw-r--r--   0        0        0    22594 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/connections/srlinux.py
+-rw-r--r--   0        0        0     9593 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/fsc.py
+-rw-r--r--   0        0        0        0 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/tasks/__init__.py
+-rw-r--r--   0        0        0      373 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/tasks/helpers.py
+-rw-r--r--   0        0        0     8844 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/nornir_srl/tasks/srl_config.py
+-rw-r--r--   0        0        0      846 2023-05-02 12:36:36.603945 nornir_srl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13193 1970-01-01 00:00:00.000000 nornir_srl-0.1.2/PKG-INFO
```

### Comparing `nornir_srl-0.1.1/README.md` & `nornir_srl-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.1.1/nornir_srl/connections/helpers.py` & `nornir_srl-0.1.2/nornir_srl/connections/helpers.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.1.1/nornir_srl/connections/srlinux.py` & `nornir_srl-0.1.2/nornir_srl/connections/srlinux.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,20 +268,23 @@
             for ni in resp[0]["network-instance"]:
                 if ni.get('protocols') and ni['protocols'].get('bgp'):
                     for peer in ni['protocols']['bgp']['neighbor']:
                         peer_data = dict()
                         if our_version == 1:
                             peer_data['evpn'] = peer.get('evpn')
                             peer_data['ipv4-unicast'] = peer.get('ipv4-unicast')
+                            peer_data['local-as'] = peer.get('local-as', [{}])[0].get('as-number', '-')
                         elif our_version == 2:
+                            peer_data['local-as'] = peer.get('local-as', {}).get('as-number', '-')
                             for afi in peer.get('afi-safi', []):
                                 if afi['afi-safi-name'] == 'evpn':
                                     peer_data['evpn'] = afi
                                 elif afi['afi-safi-name'] == 'ipv4-unicast':
                                     peer_data['ipv4-unicast'] = afi
+                        peer["_local-asn"] = peer_data['local-as']
                         if peer_data.get('evpn'):
                             peer["_evpn"] = str(peer_data["evpn"]["received-routes"]) + "/" + \
                             str(peer_data["evpn"]["active-routes"]) + "/" + \
                             str(peer_data["evpn"]["sent-routes"]) if peer_data["evpn"]["admin-state"] == "enable" else "disabled"
                         else:
                             peer["_evpn"] = "-"
                         if peer_data.get('ipv4-unicast'):
@@ -295,15 +298,15 @@
                                 peer["_ipv4"] = "disabled"
                         else:
                             peer["_ipv4"] = "-"
 
         path_spec = {
                 "path": f"/network-instance[name={network_instance}]/protocols/bgp/neighbor",
                 "jmespath": '"network-instance"[].{NetwInst:name, Neighbors: protocols.bgp.neighbor[].{"1_peer":"peer-address",\
-                    peer_as:"peer-as", state:"session-state",local_as:"local-as"[]."as-number",\
+                    peer_as:"peer-as", state:"session-state",local_as:"_local-asn",\
                     "group":"peer-group", "export_policy":"export-policy", "import_policy":"import-policy",\
                     "AFI/SAFI\\nIPv4-UC\\nRx/Act/Tx":"_ipv4", "AFI/SAFI\\nEVPN\\nRx/Act/Tx":"_evpn"}}',
                 "datatype": "state",
                 "key": "index",
             }
         resp = self.get(paths = [ path_spec.get("path")], datatype=path_spec["datatype"])
         augment_resp(resp)
```

### Comparing `nornir_srl-0.1.1/nornir_srl/fsc.py` & `nornir_srl-0.1.2/nornir_srl/fsc.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.1.1/nornir_srl/tasks/srl_config.py` & `nornir_srl-0.1.2/nornir_srl/tasks/srl_config.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.1.1/pyproject.toml` & `nornir_srl-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir_srl"
-version = "0.1.1"
+version = "0.1.2"
 description = "Nornir connection plugin for SRLinux"
 authors = ["Walter De Smedt <walter.de.smedt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/wdesmedt/nornir_srl"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nornir_srl-0.1.1/setup.py` & `nornir_srl-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,198 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nornir-srl
+Version: 0.1.2
+Summary: Nornir connection plugin for SRLinux
+Home-page: https://github.com/wdesmedt/nornir_srl
+Author: Walter De Smedt
+Author-email: walter.de.smedt@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: deepdiff (>=6.2.1,<7.0.0)
+Requires-Dist: jmespath (>=1.0.1,<2.0.0)
+Requires-Dist: jsondiff (>=2.0.0,<3.0.0)
+Requires-Dist: natsort (>=8.2.0,<9.0.0)
+Requires-Dist: nornir (>=3.3.0,<4.0.0)
+Requires-Dist: nornir-jinja2 (>=0.2.0,<0.3.0)
+Requires-Dist: nornir-scrapli (>=2022.1.30,<2023.0.0)
+Requires-Dist: nornir-utils (>=0.2.0,<0.3.0)
+Requires-Dist: pygnmi (>=0.8.9,<0.9.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
+Project-URL: Repository, https://github.com/wdesmedt/nornir_srl
+Description-Content-Type: text/markdown
+
+# nornir_srl
+This module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations.
+
+The current functionality is focused on a read-only _network-wide CLI_ to perform show commands across an entire set or subset for SRLinux nodes, as defined in the Nornir inventory and through command-line filter options. It shows output in a tabular format for easy reading.
+Following versions will focus on configuration management and command execution on the nodes.
+
+# Prerequisites
+
+This module requires [Nornir Core](https://github.com/nornir-automation/nornir) that includes the Nornir core components for which this module is an add-on.
+Nornir needs a [configuration file](https://nornir.readthedocs.io/en/latest/configuration/index.html) to tell it at a minimum where to find the inventory and what inventory plugin is used. Also runner configuration parameters, like #threads/workers for parallel execution are defined here but sane defaults are used.
+
+Since this module is using gNMI as the management inteface, at a minimum, a CA certificate is required that was used to create per-device certs and keys. If you use [Containerlab](https://containerlab.dev/) this root cert is auto-generated for SRLinux nodes and available in the lab subfolder created by the containerlab cli. This file needs to be referenced via the inventory (per-device or per-group). See below for details.
+
+# Installation
+
+Create a Python virtual-env using your favorite workflow, For example:
+```
+mkdir nornir-srl && cd nornir-srl
+python3 -m venv .venv
+source .venv/bin/activate
+```
+Following command will install the the `nornir_srl` module and all its dependencies, including Nornir core.
+
+```
+pip install wheel
+pip install -U nornir-srl
+```
+Create the Nornir confguration file, for example:
+
+```yaml
+# nornir_config.yaml
+inventory:
+    #    plugin: SimpleInventory
+    plugin: YAMLInventory
+    options:
+        host_file: "./inventory/hosts.yaml"
+        group_file: "./inventory/groups.yaml"
+        defaults_file: "./inventory/defaults.yaml"
+runner:
+    plugin: threaded
+    options:
+        num_workers: 20
+```
+Create the inventory files as referenced in the above configuration file, for example:
+```yaml
+## hosts.yaml
+clab-4l2s-l1:
+    hostname: clab-4l2s-l1
+    groups: [srl, fabric, leafs]
+clab-4l2s-l2:
+    hostname: clab-4l2s-l2
+    groups: [srl, fabric, leafs]
+clab-4l2s-s1:
+    hostname: clab-4l2s-s1
+    groups: [srl, fabric, spines]
+```
+
+```yaml
+## groups.yaml
+global:
+    data:
+        domain: clab
+srl:
+    connection_options:
+        srlinux:
+            port: 57400
+            username: admin
+            password: admin
+            extras:
+                path_cert: "./root-ca.pem"
+spines:
+    groups: [ global ]
+    data:
+        role: spine
+        type: ixr-d3
+leafs:
+    groups: [ global ]
+    data:
+        role: leaf
+        type: ixr-d2
+```
+The root certificate is specified once for all devices in group `srl` via the `connection_options.srlinux.extras.path_cert` parameter.
+
+# Use
+
+Currently, only the network-wide cli functionality is supported via the `fcli` command
+```
+$ fcli --help
+Usage: fcli [OPTIONS] REPORT
+
+Options:
+  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]
+  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf
+  -f, --field-filter TEXT    filter fields, e.g. -f state=up -f
+                             admin_state=enable
+  -b, --box-type TEXT        box type of printed table, e.g. -b
+                             minimal_double_head. 'python -m rich.box' for
+                             options
+  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn
+                             -o route_type=2 for 'bgp-rib report
+  --help                     Show this message and exit.
+  ```
+  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:
+```
+$ fcli test
+Report test not found. Available reports: ['bgp-peers', 'subinterface', 'ipv4-rib', 'mac-table', 'sys-info', 'nwi-itfs', 'lldp-nbrs']
+```
+
+The nornir configuration file (`-c` option) is mandatory for nornir to find the inventory files.
+Optionally, you can specify filters to control the output. There are 2 types of filters:
+
+- inventory filters, specified with the `-i` option, filter on the inventory, e.g. `-i hostname=clab-4l2s-l1`  or `-i role=leaf` based on inventory data
+- field filters, specified with the `-f` option. This filters based on the fields shown in the report and a value substring, e.g. `-f state=esta`. Multiple field filters can be specified by repeated `-f` options
+- report-specific options are options specific to a report, if applicable. Currently, the only report that needs extra arguments is 'bgp-rib', i.e. `route_fam=evpn|ipv4|ipv6` and `route_type=1|2|3|4|5`. The latter relates to EVPN route-trypes and is optional. Defaults to '2' (mac-ip-routes). 
+
+Examples:
+```
+$ fcli bgp-peers -i role=spine
+                                        BGP Peers                                         
+                               Inventory:{'role': 'spine'}                                
+               ╷          ╷                 ╷         ╷          ╷         ╷              
+  Node         │ NetwInst │ 1_Peer          │ 2_Group │ local_as │ peer_as │ state        
+ ══════════════╪══════════╪═════════════════╪═════════╪══════════╪═════════╪═════════════ 
+  clab-4l2s-s1 │ default  │ 192.168.0.1     │ leafs   │ [65100]  │ 65001   │ established  
+               │          │ 192.168.0.3     │ leafs   │ [65100]  │ 65002   │ established  
+               │          │ 192.168.0.5     │ leafs   │ [65100]  │ 65003   │ established  
+               │          │ 192.168.0.7     │ leafs   │ [65100]  │ 65004   │ established  
+               │          │ 192.168.0.225   │ dcgw    │ [65100]  │ 65200   │ active       
+               │          │ 192.168.0.227   │ dcgw    │ [65100]  │ 65201   │ active       
+               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect      
+               │          │ 192.168.255.201 │ overlay │ [100]    │ 100     │ connect      
+ ──────────────┼──────────┼─────────────────┼─────────┼──────────┼─────────┼───────────── 
+  clab-4l2s-s2 │ default  │ 192.168.0.229   │ dcgw    │ [65100]  │ 65200   │ active       
+               │          │ 192.168.0.231   │ dcgw    │ [65100]  │ 65201   │ active       
+               │          │ 192.168.1.1     │ leafs   │ [65100]  │ 65001   │ established  
+               │          │ 192.168.1.3     │ leafs   │ [65100]  │ 65002   │ established  
+               │          │ 192.168.1.5     │ leafs   │ [65100]  │ 65003   │ established  
+               │          │ 192.168.1.7     │ leafs   │ [65100]  │ 65004   │ established  
+               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  
+               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect     
+```
+
+```
+fcli bgp-rib -r route_fam=evpn -r route_type=2 -f 0_st='u*>'
+                                                                                      BGP RIB                                                                                      
+                                                                              Fields:{'0_st': 'u*>'}                                                                               
+                                                              Report options:{'route_fam': 'evpn', 'route_type': '2'}                                                              
+               ╷         ╷      ╷                               ╷              ╷                   ╷                   ╷         ╷               ╷        ╷                 ╷      
+  Node         │ ni      │ 0_st │ ESI                           │ IP           │ MAC               │ RD                │ as-path │ next-hop      │ origin │ peer            │ vni  
+ ══════════════╪═════════╪══════╪═══════════════════════════════╪══════════════╪═══════════════════╪═══════════════════╪═════════╪═══════════════╪════════╪═════════════════╪═════ 
+  clab-4l2s-l1 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  
+               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 0.0.0.0      │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  
+               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 10.200.1.10  │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  
+               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  
+               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.2   │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  
+ ──────────────┼─────────┼──────┼───────────────────────────────┼──────────────┼───────────────────┼───────────────────┼─────────┼───────────────┼────────┼─────────────────┼───── 
+  clab-4l2s-l2 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  
+               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  
+               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.1   │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  
+```
 
-packages = \
-['nornir_srl', 'nornir_srl.connections', 'nornir_srl.tasks']
 
-package_data = \
-{'': ['*']}
+  
 
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'deepdiff>=6.2.1,<7.0.0',
- 'jmespath>=1.0.1,<2.0.0',
- 'jsondiff>=2.0.0,<3.0.0',
- 'natsort>=8.2.0,<9.0.0',
- 'nornir-jinja2>=0.2.0,<0.3.0',
- 'nornir-scrapli>=2022.1.30,<2023.0.0',
- 'nornir-utils>=0.2.0,<0.3.0',
- 'nornir>=3.3.0,<4.0.0',
- 'pygnmi>=0.8.9,<0.9.0',
- 'rich>=12.6.0,<13.0.0']
-
-entry_points = \
-{'console_scripts': ['fcli = nornir_srl.fsc:cli'],
- 'nornir.plugins.connections': ['srlinux = '
-                                'nornir_srl.connections.srlinux:SrLinux']}
-
-setup_kwargs = {
-    'name': 'nornir-srl',
-    'version': '0.1.1',
-    'description': 'Nornir connection plugin for SRLinux',
-    'long_description': '# nornir_srl\nThis module provides a [Nornir](https://nornir.readthedocs.io/en/latest/) connection [plugin](https://nornir.tech/nornir/plugins/) for Nokia SRLinux devices. It uses the gNMI management interface of SRLinux to fetch state and push configurations.\n\nThe current functionality is focused on a read-only _network-wide CLI_ to perform show commands across an entire set or subset for SRLinux nodes, as defined in the Nornir inventory and through command-line filter options. It shows output in a tabular format for easy reading.\nFollowing versions will focus on configuration management and command execution on the nodes.\n\n# Prerequisites\n\nThis module requires [Nornir Core](https://github.com/nornir-automation/nornir) that includes the Nornir core components for which this module is an add-on.\nNornir needs a [configuration file](https://nornir.readthedocs.io/en/latest/configuration/index.html) to tell it at a minimum where to find the inventory and what inventory plugin is used. Also runner configuration parameters, like #threads/workers for parallel execution are defined here but sane defaults are used.\n\nSince this module is using gNMI as the management inteface, at a minimum, a CA certificate is required that was used to create per-device certs and keys. If you use [Containerlab](https://containerlab.dev/) this root cert is auto-generated for SRLinux nodes and available in the lab subfolder created by the containerlab cli. This file needs to be referenced via the inventory (per-device or per-group). See below for details.\n\n# Installation\n\nCreate a Python virtual-env using your favorite workflow, For example:\n```\nmkdir nornir-srl && cd nornir-srl\npython3 -m venv .venv\nsource .venv/bin/activate\n```\nFollowing command will install the the `nornir_srl` module and all its dependencies, including Nornir core.\n\n```\npip install wheel\npip install -U nornir-srl\n```\nCreate the Nornir confguration file, for example:\n\n```yaml\n# nornir_config.yaml\ninventory:\n    #    plugin: SimpleInventory\n    plugin: YAMLInventory\n    options:\n        host_file: "./inventory/hosts.yaml"\n        group_file: "./inventory/groups.yaml"\n        defaults_file: "./inventory/defaults.yaml"\nrunner:\n    plugin: threaded\n    options:\n        num_workers: 20\n```\nCreate the inventory files as referenced in the above configuration file, for example:\n```yaml\n## hosts.yaml\nclab-4l2s-l1:\n    hostname: clab-4l2s-l1\n    groups: [srl, fabric, leafs]\nclab-4l2s-l2:\n    hostname: clab-4l2s-l2\n    groups: [srl, fabric, leafs]\nclab-4l2s-s1:\n    hostname: clab-4l2s-s1\n    groups: [srl, fabric, spines]\n```\n\n```yaml\n## groups.yaml\nglobal:\n    data:\n        domain: clab\nsrl:\n    connection_options:\n        srlinux:\n            port: 57400\n            username: admin\n            password: admin\n            extras:\n                path_cert: "./root-ca.pem"\nspines:\n    groups: [ global ]\n    data:\n        role: spine\n        type: ixr-d3\nleafs:\n    groups: [ global ]\n    data:\n        role: leaf\n        type: ixr-d2\n```\nThe root certificate is specified once for all devices in group `srl` via the `connection_options.srlinux.extras.path_cert` parameter.\n\n# Use\n\nCurrently, only the network-wide cli functionality is supported via the `fcli` command\n```\n$ fcli --help\nUsage: fcli [OPTIONS] REPORT\n\nOptions:\n  -c, --cfg TEXT             Nornir config file  [default: nornir_config.yaml]\n  -i, --inv-filter TEXT      filter inventory, e.g. -i site=lab -i role=leaf\n  -f, --field-filter TEXT    filter fields, e.g. -f state=up -f\n                             admin_state=enable\n  -b, --box-type TEXT        box type of printed table, e.g. -b\n                             minimal_double_head. \'python -m rich.box\' for\n                             options\n  -r, --report-options TEXT  report-specific options, e.g. -o route_fam=evpn\n                             -o route_type=2 for \'bgp-rib report\n  --help                     Show this message and exit.\n  ```\n  `REPORT` is a mandatory argument and specifies the report to run. To know which reports are supported, specify a dummy report name:\n```\n$ fcli test\nReport test not found. Available reports: [\'bgp-peers\', \'subinterface\', \'ipv4-rib\', \'mac-table\', \'sys-info\', \'nwi-itfs\', \'lldp-nbrs\']\n```\n\nThe nornir configuration file (`-c` option) is mandatory for nornir to find the inventory files.\nOptionally, you can specify filters to control the output. There are 2 types of filters:\n\n- inventory filters, specified with the `-i` option, filter on the inventory, e.g. `-i hostname=clab-4l2s-l1`  or `-i role=leaf` based on inventory data\n- field filters, specified with the `-f` option. This filters based on the fields shown in the report and a value substring, e.g. `-f state=esta`. Multiple field filters can be specified by repeated `-f` options\n- report-specific options are options specific to a report, if applicable. Currently, the only report that needs extra arguments is \'bgp-rib\', i.e. `route_fam=evpn|ipv4|ipv6` and `route_type=1|2|3|4|5`. The latter relates to EVPN route-trypes and is optional. Defaults to \'2\' (mac-ip-routes). \n\nExamples:\n```\n$ fcli bgp-peers -i role=spine\n                                        BGP Peers                                         \n                               Inventory:{\'role\': \'spine\'}                                \n               ╷          ╷                 ╷         ╷          ╷         ╷              \n  Node         │ NetwInst │ 1_Peer          │ 2_Group │ local_as │ peer_as │ state        \n ══════════════╪══════════╪═════════════════╪═════════╪══════════╪═════════╪═════════════ \n  clab-4l2s-s1 │ default  │ 192.168.0.1     │ leafs   │ [65100]  │ 65001   │ established  \n               │          │ 192.168.0.3     │ leafs   │ [65100]  │ 65002   │ established  \n               │          │ 192.168.0.5     │ leafs   │ [65100]  │ 65003   │ established  \n               │          │ 192.168.0.7     │ leafs   │ [65100]  │ 65004   │ established  \n               │          │ 192.168.0.225   │ dcgw    │ [65100]  │ 65200   │ active       \n               │          │ 192.168.0.227   │ dcgw    │ [65100]  │ 65201   │ active       \n               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect      \n               │          │ 192.168.255.201 │ overlay │ [100]    │ 100     │ connect      \n ──────────────┼──────────┼─────────────────┼─────────┼──────────┼─────────┼───────────── \n  clab-4l2s-s2 │ default  │ 192.168.0.229   │ dcgw    │ [65100]  │ 65200   │ active       \n               │          │ 192.168.0.231   │ dcgw    │ [65100]  │ 65201   │ active       \n               │          │ 192.168.1.1     │ leafs   │ [65100]  │ 65001   │ established  \n               │          │ 192.168.1.3     │ leafs   │ [65100]  │ 65002   │ established  \n               │          │ 192.168.1.5     │ leafs   │ [65100]  │ 65003   │ established  \n               │          │ 192.168.1.7     │ leafs   │ [65100]  │ 65004   │ established  \n               │          │ 192.168.255.1   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.2   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.3   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.4   │ overlay │ [100]    │ 100     │ established  \n               │          │ 192.168.255.200 │ overlay │ [100]    │ 100     │ connect     \n```\n\n```\nfcli bgp-rib -r route_fam=evpn -r route_type=2 -f 0_st=\'u*>\'\n                                                                                      BGP RIB                                                                                      \n                                                                              Fields:{\'0_st\': \'u*>\'}                                                                               \n                                                              Report options:{\'route_fam\': \'evpn\', \'route_type\': \'2\'}                                                              \n               ╷         ╷      ╷                               ╷              ╷                   ╷                   ╷         ╷               ╷        ╷                 ╷      \n  Node         │ ni      │ 0_st │ ESI                           │ IP           │ MAC               │ RD                │ as-path │ next-hop      │ origin │ peer            │ vni  \n ══════════════╪═════════╪══════╪═══════════════════════════════╪══════════════╪═══════════════════╪═══════════════════╪═════════╪═══════════════╪════════╪═════════════════╪═════ \n  clab-4l2s-l1 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 0.0.0.0      │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 01:24:24:24:24:24:24:00:00:01 │ 10.200.1.10  │ 1A:41:0E:FF:00:41 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.2   │ 1A:A2:09:FF:00:42 │ 192.168.255.2:202 │ i       │ 192.168.255.2 │ igp    │ 192.168.255.101 │ 202  \n ──────────────┼─────────┼──────┼───────────────────────────────┼──────────────┼───────────────────┼───────────────────┼─────────┼───────────────┼────────┼─────────────────┼───── \n  clab-4l2s-l2 │ default │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.254 │ 00:00:5E:00:01:01 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 0.0.0.0      │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n               │         │ u*>  │ 00:00:00:00:00:00:00:00:00:00 │ 10.200.1.1   │ 1A:5B:08:FF:00:42 │ 192.168.255.1:202 │ i       │ 192.168.255.1 │ igp    │ 192.168.255.101 │ 202  \n```\n\n\n  \n',
-    'author': 'Walter De Smedt',
-    'author_email': 'walter.de.smedt@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/wdesmedt/nornir_srl',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

