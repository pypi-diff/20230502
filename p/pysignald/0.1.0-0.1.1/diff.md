# Comparing `tmp/pysignald-0.1.0.tar.gz` & `tmp/pysignald-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysignald-0.1.0.tar", max compression
+gzip compressed data, was "pysignald-0.1.1.tar", max compression
```

## Comparing `pysignald-0.1.0.tar` & `pysignald-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1060 2021-07-11 22:56:49.954190 pysignald-0.1.0/LICENSE
--rw-r--r--   0        0        0     5002 2022-07-30 23:39:06.983600 pysignald-0.1.0/README.md
--rw-r--r--   0        0        0      559 2022-07-30 23:40:31.675662 pysignald-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       73 2021-07-11 22:56:49.958192 pysignald-0.1.0/signald/__init__.py
--rw-r--r--   0        0        0    20570 2022-07-31 00:05:14.498326 pysignald-0.1.0/signald/main.py
--rw-r--r--   0        0        0     2716 2022-07-30 23:39:06.983600 pysignald-0.1.0/signald/types.py
--rw-r--r--   0        0        0     5909 2022-07-31 00:06:41.742667 pysignald-0.1.0/setup.py
--rw-r--r--   0        0        0     5884 2022-07-31 00:06:41.744534 pysignald-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2020-06-01 11:40:25.065216 pysignald-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5108 2023-05-01 23:18:28.416934 pysignald-0.1.1/README.md
+-rw-r--r--   0        0        0      559 2023-05-01 23:19:26.948692 pysignald-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-05-01 23:19:20.916717 pysignald-0.1.1/signald/__init__.py
+-rw-r--r--   0        0        0    20884 2023-05-01 23:12:11.810494 pysignald-0.1.1/signald/main.py
+-rw-r--r--   0        0        0     2886 2023-05-01 23:12:11.810494 pysignald-0.1.1/signald/types.py
+-rw-r--r--   0        0        0     6041 1970-01-01 00:00:00.000000 pysignald-0.1.1/PKG-INFO
```

### Comparing `pysignald-0.1.0/LICENSE` & `pysignald-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysignald-0.1.0/README.md` & `pysignald-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,21 @@
 
 # Get the profile information of someone
 profile_info = s.get_profile(recipient="+1098765432")
 print(profile_info)
 
 for message in s.receive_messages():
     print(message)
-    s.react(message.source, Reaction("🥳", message.source, message.timestamp))
+    s.react(Reaction("🥳", message.source, message.timestamp), message.source["number"])
 
     # Send a read receipt notification which shows the message read checkmark on the receipient side
     s.send_read_receipt(recipient=message.source["number"], timestamps=[message.timestamp])
+
+    # Echo the message back.
+    s.send(recipient=message.source["number"], text=message.text)
 ```
 
 You can also use the chat decorator interface:
 
 ```python
 from signald import Signal
```

### Comparing `pysignald-0.1.0/pyproject.toml` & `pysignald-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysignald"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library that allows communication via the Signal IM service using the signald daemon."
 license = "MIT"
 authors = ["Stavros Korokithakis <hi@stavros.io>"]
 packages = [{include = "signald"}]
 readme = "README.md"
 repository = "https://gitlab.com/stavros/pysignald/"
```

### Comparing `pysignald-0.1.0/signald/main.py` & `pysignald-0.1.1/signald/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from .types import AccessControl
 from .types import Address
 from .types import Attachment
 from .types import Group
 from .types import Identity
 from .types import MemberDetail
+from .types import Mention
 from .types import Message
 from .types import Payment
 from .types import Reaction
 from .types import TrustLevel
 
 # We'll need to know the compiled RE object later.
 RE_TYPE = type(re.compile(""))
@@ -221,14 +222,22 @@
                         size=attachment["size"],
                         stored_filename=attachment["storedFilename"],
                     )
                     for attachment in data_message.get("attachments", [])
                 ],
                 reaction=reaction,
                 payment=payment,
+                mentions=[
+                    Mention(
+                        uuid=m["uuid"],
+                        start=m["start"],
+                        length=m["length"],
+                    )
+                    for m in data_message.get("mentions", [])
+                ],
             )
 
     @deprecated(version="0.1.0", reason="Use 'send' with keyword argument 'recipient'")
     def send_message(
         self,
         recipient: Union[str, dict],
         text: str,
@@ -536,15 +545,15 @@
                     reply = func(message, match)
                 except:  # noqa - We don't care why this failed.
                     continue
 
                 if not isinstance(reply, tuple):
                     stop = True
                     reaction = None
-                if len(reply) == 2:
+                elif len(reply) == 2:
                     stop, reply = reply
                     reaction = None
                 elif len(reply) == 3:
                     stop, reply, reaction = reply
 
                 # In case a message came from a group chat
                 group_id = message.group.get("groupId") or message.group_v2.get("id")
```

### Comparing `pysignald-0.1.0/signald/types.py` & `pysignald-0.1.1/signald/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,28 +32,36 @@
 @attr.s
 class Payment:
     note = attr.ib(type=str)
     receipt = attr.ib(type=str)
 
 
 @attr.s
+class Mention:
+    uuid = attr.ib(type=str)
+    start = attr.ib(type=int)
+    length = attr.ib(type=int)
+
+
+@attr.s
 class Message:
     username = attr.ib(type=str)
     source = attr.ib(type=Union[str, dict])
     text = attr.ib(type=str)
     source_device = attr.ib(type=int, default=0)
     timestamp = attr.ib(type=int, default=None)
     expiration_secs = attr.ib(type=int, default=0)
     is_receipt = attr.ib(type=bool, default=False)
     attachments = attr.ib(type=list, default=[])
     quote = attr.ib(type=str, default=None)
     group = attr.ib(type=dict, default={})
     group_v2 = attr.ib(type=dict, default={})
     reaction = attr.ib(type=Optional[Reaction], default=None)
     payment = attr.ib(type=Optional[Payment], default=None)
+    mentions = attr.ib(type=List[Mention], default=[])
 
 
 @attr.s
 class MemberDetail:
     uuid = attr.ib(type=str)
     role = attr.ib(type=str)
     joined_revision = attr.ib(type=int)
```

### Comparing `pysignald-0.1.0/setup.py` & `pysignald-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,197 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pysignald
+Version: 0.1.1
+Summary: A library that allows communication via the Signal IM service using the signald daemon.
+Home-page: https://gitlab.com/stavros/pysignald/
+License: MIT
+Author: Stavros Korokithakis
+Author-email: hi@stavros.io
+Requires-Python: >=3.5,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Deprecated (>=1.2.11,<2.0.0)
+Requires-Dist: attrs (>=21.2,<22.0)
+Project-URL: Repository, https://gitlab.com/stavros/pysignald/
+Description-Content-Type: text/markdown
 
-packages = \
-['signald']
+pysignald
+=======
 
-package_data = \
-{'': ['*']}
+[![PyPI](https://img.shields.io/pypi/v/pysignald.svg)](https://pypi.org/project/pysignald/)
+[![pipeline status](https://gitlab.com/stavros/pysignald/badges/master/pipeline.svg)](https://gitlab.com/stavros/pysignald/commits/master)
 
-install_requires = \
-['Deprecated>=1.2.11,<2.0.0', 'attrs>=21.2,<22.0']
-
-setup_kwargs = {
-    'name': 'pysignald',
-    'version': '0.1.0',
-    'description': 'A library that allows communication via the Signal IM service using the signald daemon.',
-    'long_description': 'pysignald\n=======\n\n[![PyPI](https://img.shields.io/pypi/v/pysignald.svg)](https://pypi.org/project/pysignald/)\n[![pipeline status](https://gitlab.com/stavros/pysignald/badges/master/pipeline.svg)](https://gitlab.com/stavros/pysignald/commits/master)\n\npysignald is a Python client for the excellent [signald](https://signald.org/) project, which in turn\nis a command-line client for the Signal messaging service.\n\npysignald allows you to programmatically send and receive messages to Signal.\n\nNOTE: Unfortunately, this library might be somewhat out of date or parts of it might not be working, as the upstream API\nkeeps changing, breaking compatibility. If you notice any breakage, MRs to fix it would be appreciated.\n\n\nInstallation\n------------\n\nYou can install pysignald with pip:\n\n```\n$ pip install pysignald\n```\n\n\nRunning\n-------\n\nJust make sure you have signald installed. Here\'s an example of how to use pysignald:\n\n\n```python\nfrom signald import Signal, Reaction\n\ns = Signal("+1234567890")\n\n# If you haven\'t registered/verified signald, do that first:\ns.register(voice=False)\ns.verify("sms code")\n\n# If you want to set your display name, mobilecoin payments address (if using payments), or avatar, you can call set_profile:\ns.set_profile(\n    display_name="My user name",\n    mobilecoin_address="...", # Base64-encoded PublicAddress, see https://github.com/mobilecoinfoundation/mobilecoin/blob/master/api/proto/external.proto\n    avatar_filename="/signald-data/avatar.png", # Must be accessible by signald\n)\n\ns.send(recipient="+1098765432", text="Hello there!")\ns.send(recipient_group_id="YXNkZkFTREZhc2RmQVNERg==", text="Hello group!")\n\n# Get the profile information of someone\nprofile_info = s.get_profile(recipient="+1098765432")\nprint(profile_info)\n\nfor message in s.receive_messages():\n    print(message)\n    s.react(message.source, Reaction("🥳", message.source, message.timestamp))\n\n    # Send a read receipt notification which shows the message read checkmark on the receipient side\n    s.send_read_receipt(recipient=message.source["number"], timestamps=[message.timestamp])\n```\n\nYou can also use the chat decorator interface:\n\n```python\nfrom signald import Signal\n\ns = Signal("+1234567890")\n\n@s.chat_handler("hello there", order=10)  # This is case-insensitive.\ndef hello_there(message, match):\n    # Returning `False` as the first argument will cause matching to continue\n    # after this handler runs.\n    stop = False\n    reply = "Hello there!"\n    return stop, reply\n\n\n# Matching is case-insensitive. The `order` argument signifies when\n# the handler will try to match (default is 100), and functions get sorted\n# by order of declaration secondly.\n@s.chat_handler("hello", order=10)\ndef hello(message, match):\n    # This will match on "hello there" as well because of the "stop" return code in\n    # the function above. Both replies will be sent.\n    return "Hello!"\n\n\n@s.chat_handler("wave", order=20)\ndef react_with_waving_hand(message, match):\n    # This will only react to the received message.\n    # But it would be possible to send a reply and a reaction at the same time.\n    stop = True\n    reply = None\n    reaction = "👋"\n    return stop, reply, reaction\n\n\n@s.chat_handler(re.compile("my name is (.*)"))  # This is case-sensitive.\ndef name(message, match):\n    return "Hello %s." % match.group(1)\n\n\n@s.chat_handler("")\ndef catch_all(message, match):\n    # This will only be sent if nothing else matches, because matching\n    # stops by default on the first function that matches.\n    return "I don\'t know what you said."\n\ns.run_chat()\n```\n\n### Identity handling:\n\n```python\nfrom signald import Signal\nfrom signald.types import TrustLevel\n\ns = Signal("+1234567890")\n\n# Revoke trust for all identities of a given number\nfor identity in s.get_identities("+1234001100"):\n    s.trust(\n        "+1234001100",\n        identity.safety_number,\n        TrustLevel.UNTRUSTED,\n    )\n\n# Generate QR code data for identity validation\nids = s.get_identities("+1234001177")\nids.sort(key=lambda x: x.added, reverse=True)\n# prints base64 encoded validation code of the latest identity of the given number\nprint(ids[0].qr_code_data)\n```\nYou can pipe the content of `ids[0].qr_code_data`  to `| base64 -D | qrencode -t ansi` to validate the identity via the Singal app QR scanner.\n\n\n### Group information:\n```python\nfrom signald import Signal\n\ns = Signal("+1234567890")\n\n# list all groups and members\nfor group in s.list_groups():\n    print(group.title)\n    for member in group.members:\n        print(member.get("uuid"))\n```\n\nVarious\n-------\n\npysignald also supports different socket paths:\n\n```python\ns = Signal("+1234567890", socket_path="/var/some/other/socket.sock")\n```\n\nIt supports TCP sockets too, if you run a proxy. For example, you can proxy signald\'s UNIX socket over TCP with socat:\n\n```bash\n$ socat -d -d TCP4-LISTEN:15432,fork UNIX-CONNECT:/var/run/signald/signald.sock\n```\n\nThen in pysignald:\n\n```python\ns = Signal("+1234567890", socket_path=("your.serveri.ip", 15432))\n```\n',
-    'author': 'Stavros Korokithakis',
-    'author_email': 'hi@stavros.io',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.com/stavros/pysignald/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.5,<4.0',
-}
+pysignald is a Python client for the excellent [signald](https://signald.org/) project, which in turn
+is a command-line client for the Signal messaging service.
 
+pysignald allows you to programmatically send and receive messages to Signal.
+
+NOTE: Unfortunately, this library might be somewhat out of date or parts of it might not be working, as the upstream API
+keeps changing, breaking compatibility. If you notice any breakage, MRs to fix it would be appreciated.
+
+
+Installation
+------------
+
+You can install pysignald with pip:
+
+```
+$ pip install pysignald
+```
+
+
+Running
+-------
+
+Just make sure you have signald installed. Here's an example of how to use pysignald:
+
+
+```python
+from signald import Signal, Reaction
+
+s = Signal("+1234567890")
+
+# If you haven't registered/verified signald, do that first:
+s.register(voice=False)
+s.verify("sms code")
+
+# If you want to set your display name, mobilecoin payments address (if using payments), or avatar, you can call set_profile:
+s.set_profile(
+    display_name="My user name",
+    mobilecoin_address="...", # Base64-encoded PublicAddress, see https://github.com/mobilecoinfoundation/mobilecoin/blob/master/api/proto/external.proto
+    avatar_filename="/signald-data/avatar.png", # Must be accessible by signald
+)
+
+s.send(recipient="+1098765432", text="Hello there!")
+s.send(recipient_group_id="YXNkZkFTREZhc2RmQVNERg==", text="Hello group!")
+
+# Get the profile information of someone
+profile_info = s.get_profile(recipient="+1098765432")
+print(profile_info)
+
+for message in s.receive_messages():
+    print(message)
+    s.react(Reaction("🥳", message.source, message.timestamp), message.source["number"])
+
+    # Send a read receipt notification which shows the message read checkmark on the receipient side
+    s.send_read_receipt(recipient=message.source["number"], timestamps=[message.timestamp])
+
+    # Echo the message back.
+    s.send(recipient=message.source["number"], text=message.text)
+```
+
+You can also use the chat decorator interface:
+
+```python
+from signald import Signal
+
+s = Signal("+1234567890")
+
+@s.chat_handler("hello there", order=10)  # This is case-insensitive.
+def hello_there(message, match):
+    # Returning `False` as the first argument will cause matching to continue
+    # after this handler runs.
+    stop = False
+    reply = "Hello there!"
+    return stop, reply
+
+
+# Matching is case-insensitive. The `order` argument signifies when
+# the handler will try to match (default is 100), and functions get sorted
+# by order of declaration secondly.
+@s.chat_handler("hello", order=10)
+def hello(message, match):
+    # This will match on "hello there" as well because of the "stop" return code in
+    # the function above. Both replies will be sent.
+    return "Hello!"
+
+
+@s.chat_handler("wave", order=20)
+def react_with_waving_hand(message, match):
+    # This will only react to the received message.
+    # But it would be possible to send a reply and a reaction at the same time.
+    stop = True
+    reply = None
+    reaction = "👋"
+    return stop, reply, reaction
+
+
+@s.chat_handler(re.compile("my name is (.*)"))  # This is case-sensitive.
+def name(message, match):
+    return "Hello %s." % match.group(1)
+
+
+@s.chat_handler("")
+def catch_all(message, match):
+    # This will only be sent if nothing else matches, because matching
+    # stops by default on the first function that matches.
+    return "I don't know what you said."
+
+s.run_chat()
+```
+
+### Identity handling:
+
+```python
+from signald import Signal
+from signald.types import TrustLevel
+
+s = Signal("+1234567890")
+
+# Revoke trust for all identities of a given number
+for identity in s.get_identities("+1234001100"):
+    s.trust(
+        "+1234001100",
+        identity.safety_number,
+        TrustLevel.UNTRUSTED,
+    )
+
+# Generate QR code data for identity validation
+ids = s.get_identities("+1234001177")
+ids.sort(key=lambda x: x.added, reverse=True)
+# prints base64 encoded validation code of the latest identity of the given number
+print(ids[0].qr_code_data)
+```
+You can pipe the content of `ids[0].qr_code_data`  to `| base64 -D | qrencode -t ansi` to validate the identity via the Singal app QR scanner.
+
+
+### Group information:
+```python
+from signald import Signal
+
+s = Signal("+1234567890")
+
+# list all groups and members
+for group in s.list_groups():
+    print(group.title)
+    for member in group.members:
+        print(member.get("uuid"))
+```
+
+Various
+-------
+
+pysignald also supports different socket paths:
+
+```python
+s = Signal("+1234567890", socket_path="/var/some/other/socket.sock")
+```
+
+It supports TCP sockets too, if you run a proxy. For example, you can proxy signald's UNIX socket over TCP with socat:
+
+```bash
+$ socat -d -d TCP4-LISTEN:15432,fork UNIX-CONNECT:/var/run/signald/signald.sock
+```
+
+Then in pysignald:
+
+```python
+s = Signal("+1234567890", socket_path=("your.serveri.ip", 15432))
+```
 
-setup(**setup_kwargs)
```

