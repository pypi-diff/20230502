# Comparing `tmp/pan_os_python-1.8.1.tar.gz` & `tmp/pan_os_python-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_os_python-1.8.1.tar", max compression
+gzip compressed data, was "pan_os_python-1.9.0.tar", max compression
```

## Comparing `pan_os_python-1.8.1.tar` & `pan_os_python-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      759 2023-02-22 10:54:56.691053 pan_os_python-1.8.1/LICENSE
--rw-r--r--   0        0        0     5341 2023-02-22 10:54:56.691053 pan_os_python-1.8.1/README.md
--rwxr-xr-x   0        0        0    14455 2023-02-22 10:55:43.241847 pan_os_python-1.8.1/panos/__init__.py
--rw-r--r--   0        0        0   205418 2023-02-22 10:54:56.691053 pan_os_python-1.8.1/panos/base.py
--rw-r--r--   0        0        0    77233 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/device.py
--rw-r--r--   0        0        0     3099 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/errors.py
--rw-r--r--   0        0        0    23317 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/firewall.py
--rw-r--r--   0        0        0    19383 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/ha.py
--rw-r--r--   0        0        0   184248 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/network.py
--rw-r--r--   0        0        0    41752 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/objects.py
--rw-r--r--   0        0        0    43596 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/panorama.py
--rw-r--r--   0        0        0    23491 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/plugins.py
--rw-r--r--   0        0        0    52621 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/policies.py
--rw-r--r--   0        0        0    12389 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/predefined.py
--rw-r--r--   0        0        0    23720 2023-02-22 10:54:56.695053 pan_os_python-1.8.1/panos/updater.py
--rw-r--r--   0        0        0    27968 2023-02-22 10:54:56.699053 pan_os_python-1.8.1/panos/userid.py
--rw-r--r--   0        0        0     2033 2023-02-22 10:55:43.237847 pan_os_python-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     6278 1970-01-01 00:00:00.000000 pan_os_python-1.8.1/setup.py
--rw-r--r--   0        0        0     6921 1970-01-01 00:00:00.000000 pan_os_python-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      759 2023-04-26 07:58:03.409999 pan_os_python-1.9.0/LICENSE
+-rw-r--r--   0        0        0     5341 2023-04-26 07:58:03.413998 pan_os_python-1.9.0/README.md
+-rwxr-xr-x   0        0        0    14455 2023-04-26 07:59:00.670423 pan_os_python-1.9.0/panos/__init__.py
+-rw-r--r--   0        0        0   205418 2023-04-26 07:58:03.413998 pan_os_python-1.9.0/panos/base.py
+-rw-r--r--   0        0        0    77233 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/device.py
+-rw-r--r--   0        0        0     3099 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/errors.py
+-rw-r--r--   0        0        0    23317 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/firewall.py
+-rw-r--r--   0        0        0    19383 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/ha.py
+-rw-r--r--   0        0        0   184598 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/network.py
+-rw-r--r--   0        0        0    41752 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/objects.py
+-rw-r--r--   0        0        0    43596 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/panorama.py
+-rw-r--r--   0        0        0    23491 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/plugins.py
+-rw-r--r--   0        0        0    52621 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/policies.py
+-rw-r--r--   0        0        0    12389 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/predefined.py
+-rw-r--r--   0        0        0    23720 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/updater.py
+-rw-r--r--   0        0        0    27968 2023-04-26 07:58:03.417998 pan_os_python-1.9.0/panos/userid.py
+-rw-r--r--   0        0        0     2033 2023-04-26 07:59:00.666423 pan_os_python-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6278 1970-01-01 00:00:00.000000 pan_os_python-1.9.0/setup.py
+-rw-r--r--   0        0        0     6921 1970-01-01 00:00:00.000000 pan_os_python-1.9.0/PKG-INFO
```

### Comparing `pan_os_python-1.8.1/LICENSE` & `pan_os_python-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/README.md` & `pan_os_python-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/__init__.py` & `pan_os_python-1.9.0/panos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Documentation available at https://pan-os-python.readthedocs.io
 
 """
 
 __author__ = "Palo Alto Networks"
 __email__ = "devrel@paloaltonetworks.com"
-__version__ = "1.8.1"
+__version__ = "1.9.0"
 
 
 import logging
 import sys
 import xml.etree.ElementTree as ET
 from distutils.version import LooseVersion  # Used by PanOSVersion class
```

### Comparing `pan_os_python-1.8.1/panos/base.py` & `pan_os_python-1.9.0/panos/base.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/device.py` & `pan_os_python-1.9.0/panos/device.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/errors.py` & `pan_os_python-1.9.0/panos/errors.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/firewall.py` & `pan_os_python-1.9.0/panos/firewall.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/ha.py` & `pan_os_python-1.9.0/panos/ha.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/network.py` & `pan_os_python-1.9.0/panos/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1340,14 +1340,15 @@
         enable_dhcp (bool): Enable DHCP on this interface
         create_dhcp_default_route (bool): Layer3: Create default route pointing to default gateway provided by server
         dhcp_default_route_metric (int): Layer3: Metric for the DHCP default route
         lacp_enable (bool): Enables LACP
         lacp_passive_pre_negotiation (bool): Enable LACP passive pre-negotiation, off by default
         lacp_mode (str): Set LACP mode to 'active' or 'passive'
         lacp_rate (str): Set LACP transmission-rate to 'fast' or 'slow'
+        lacp_fast_failover (bool): Enable fast failover for LACP
 
     """
 
     ALLOW_SET_VLAN = True
     CHILDTYPES = (
         "network.Layer3Subinterface",
         "network.Layer2Subinterface",
@@ -1507,14 +1508,22 @@
             VersionedParamPath(
                 "lacp_rate",
                 condition={"mode": ["layer3", "layer2", "ha"], "lacp_enable": True},
                 values=["fast", "slow"],
                 path="{mode}/lacp/transmission-rate",
             )
         )
+        params.append(
+            VersionedParamPath(
+                "lacp_fast_failover",
+                condition={"mode": ["layer3", "layer2", "ha"], "lacp_enable": True},
+                vartype="yesno",
+                path="{mode}/lacp/fast-failover",
+            )
+        )
 
         self._params = tuple(params)
 
 
 class VlanInterface(Interface):
     """Vlan interface
```

### Comparing `pan_os_python-1.8.1/panos/objects.py` & `pan_os_python-1.9.0/panos/objects.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/panorama.py` & `pan_os_python-1.9.0/panos/panorama.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/plugins.py` & `pan_os_python-1.9.0/panos/plugins.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/policies.py` & `pan_os_python-1.9.0/panos/policies.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/predefined.py` & `pan_os_python-1.9.0/panos/predefined.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/updater.py` & `pan_os_python-1.9.0/panos/updater.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/panos/userid.py` & `pan_os_python-1.9.0/panos/userid.py`

 * *Files identical despite different names*

### Comparing `pan_os_python-1.8.1/pyproject.toml` & `pan_os_python-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pan-os-python"
-version = "1.8.1"
+version = "1.9.0"
 description = "Framework for interacting with Palo Alto Networks devices via API"
 authors = ["Palo Alto Networks <devrel@paloaltonetworks.com>"]
 license = "ISC"
 keywords = ["panos", "pan-os-python"]
 readme = "README.md"
 homepage = "https://github.com/PaloAltoNetworks/pan-os-python"
 repository = "https://github.com/PaloAltoNetworks/pan-os-python"
```

### Comparing `pan_os_python-1.8.1/setup.py` & `pan_os_python-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pan-python>=0.17.0,<0.18.0']
 
 setup_kwargs = {
     'name': 'pan-os-python',
-    'version': '1.8.1',
+    'version': '1.9.0',
     'description': 'Framework for interacting with Palo Alto Networks devices via API',
     'long_description': 'Palo Alto Networks PAN-OS SDK for Python\n========================================\n\nThe PAN-OS SDK for Python (pan-os-python) is a package to help interact with\nPalo Alto Networks devices (including physical and virtualized Next-generation\nFirewalls and Panorama).  The pan-os-python SDK is object oriented and mimics\nthe traditional interaction with the device via the GUI or CLI/API.\n\n* Documentation: http://pan-os-python.readthedocs.io\n\n-----\n\n[![Latest version released on PyPi](https://img.shields.io/pypi/v/pan-os-python.svg)](https://pypi.python.org/pypi/pan-os-python)\n[![Python versions](https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blueviolet)](https://pypi.python.org/pypi/pan-os-python)\n[![License](https://img.shields.io/pypi/l/pan-os-python)](https://github.com/PaloAltoNetworks/pan-os-python/blob/develop/LICENSE)\n[![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://pan-os-python.readthedocs.io/en/latest/?badge=latest)\n[![Chat on GitHub Discussions](https://img.shields.io/badge/chat%20on-GitHub%20Discussions-brightgreen)](https://github.com/PaloAltoNetworks/pan-os-python/discussions)\n\n[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org/)\n[![Powered by DepHell](https://img.shields.io/badge/Powered%20by-DepHell-red)](https://github.com/dephell/dephell)\n[![GitHub contributors](https://img.shields.io/github/contributors/PaloAltoNetworks/pan-os-python)](https://github.com/PaloAltoNetworks/pan-os-python/graphs/contributors/)\n\n-----\n\nFeatures\n--------\n\n- Object model of Firewall and Panorama configuration\n- Multiple connection methods including Panorama as a proxy\n- All operations natively vsys-aware\n- Support for high availability pairs and retry/recovery during node failure\n- Batch User-ID operations\n- Device API exception classification\n\nStatus\n------\n\nPalo Alto Networks PAN-OS SDK for Python is considered stable. It is fully tested\nand used in many production environments. Semantic versioning is applied to indicate\nbug fixes, new features, and breaking changes in each version.\n\nInstall\n-------\n\nInstall using pip:\n\n```shell\npip install pan-os-python\n```\n\nUpgrade to the latest version:\n\n```shell\npip install --upgrade pan-os-python\n```\n\nIf you have poetry installed, you can also add pan-os-python to your project:\n \n```shell\npoetry add pan-os-python\n```\n\nHow to import\n-------------\n\nTo use pan-os-python in a project:\n\n```python\nimport panos\n```\n\nYou can also be more specific about which modules you want to import:\n\n```python\nfrom panos import firewall\nfrom panos import network\n```\n\n\nA few examples\n--------------\n\nFor configuration tasks, create a tree structure using the classes in\neach module. Nodes hierarchy must follow the model in the\n[Configuration Tree](http://pan-os-python.readthedocs.io/en/latest/configtree.html).\n\nThe following examples assume the modules were imported as such:\n\n```python\nfrom panos import firewall\nfrom panos import network\n```\n\nCreate an interface and commit:\n\n```python\nfw = firewall.Firewall("10.0.0.1", api_username="admin", api_password="admin")\neth1 = network.EthernetInterface("ethernet1/1", mode="layer3")\nfw.add(eth1)\neth1.create()\nfw.commit()\n```\n\nOperational commands leverage the \'op\' method of the device:\n\n```python\nfw = firewall.Firewall("10.0.0.1", api_username="admin", api_password="admin")\nprint fw.op("show system info")\n```\n\nSome operational commands have methods to refresh the variables in an object:\n\n```python\n# populates the version, serial, and model variables from the live device\nfw.refresh_system_info()\n```\n\nSee more examples in the [Usage Guide](http://pan-os-python.readthedocs.io/en/latest/usage.html).\n\nUpgrade from pandevice\n----------------------\n\nThis `pan-os-python` package is the evolution of the older `pandevice` package. To\nupgrade from `pandevice` to `pan-os-python`, follow these steps.\n\nStep 1. Ensure you are using python3\n\n   [Python2 is end-of-life](https://www.python.org/doc/sunset-python-2/) and not\n   supported by `pan-os-python`.\n\nStep 2. Uninstall pandevice:\n\n```shell\npip uninstall pandevice\n # or\npoetry remove pandevice\n```\n\nStep 3. Install pan-os-python:\n\n```shell\npip3 install pan-os-python\n # or\npoetry add pan-os-python\n```\n\nStep 4. Change the import statements in your code from `pandevice` to `panos`. For example:\n\n```python\nimport pandevice\nfrom pandevice.firewall import Firewall\n\n # would change to\n\nimport panos\nfrom panos.firewall import Firewall\n```\n\nStep 5. Test your script or application\n\n   There are no known breaking changes\n   between `pandevice v0.14.0` and `pan-os-python v1.0.0`, but it is a major\n   upgrade so please verify everything works as expected.\n\nContributors\n------------\n\n- Brian Torres-Gil - [btorresgil](https://github.com/btorresgil)\n- Garfield Freeman - [shinmog](https://github.com/shinmog)\n- John Anderson - [lampwins](https://github.com/lampwins)\n- Aditya Sripal - [AdityaSripal](https://github.com/AdityaSripal)\n\nThank you to [Kevin Steves](https://github.com/kevinsteves), creator of the [pan-python library](https://github.com/kevinsteves/pan-python)\n',
     'author': 'Palo Alto Networks',
     'author_email': 'devrel@paloaltonetworks.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/PaloAltoNetworks/pan-os-python',
```

### Comparing `pan_os_python-1.8.1/PKG-INFO` & `pan_os_python-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-os-python
-Version: 1.8.1
+Version: 1.9.0
 Summary: Framework for interacting with Palo Alto Networks devices via API
 Home-page: https://github.com/PaloAltoNetworks/pan-os-python
 License: ISC
 Keywords: panos,pan-os-python
 Author: Palo Alto Networks
 Author-email: devrel@paloaltonetworks.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
```

