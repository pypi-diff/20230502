# Comparing `tmp/voip-utils-0.0.6.tar.gz` & `tmp/voip-utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voip-utils-0.0.6.tar", last modified: Mon May  1 15:26:07 2023, max compression
+gzip compressed data, was "voip-utils-0.0.7.tar", last modified: Tue May  2 19:51:42 2023, max compression
```

## Comparing `voip-utils-0.0.6.tar` & `voip-utils-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-01 15:26:07.727852 voip-utils-0.0.6/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.6/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      785 2023-05-01 15:26:07.727852 voip-utils-0.0.6/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.6/README.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1977 2023-05-01 15:25:43.000000 voip-utils-0.0.6/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-05-01 15:26:07.727852 voip-utils-0.0.6/setup.cfg
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-01 15:26:07.723852 voip-utils-0.0.6/voip_utils/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.6/voip_utils/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.6/voip_utils/error.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7191 2023-04-23 03:37:26.000000 voip-utils-0.0.6/voip_utils/rtp_audio.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7603 2023-05-01 15:11:40.000000 voip-utils-0.0.6/voip_utils/sip.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.6/voip_utils/util.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6284 2023-04-23 03:37:26.000000 voip-utils-0.0.6/voip_utils/voip.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-01 15:26:07.723852 voip-utils-0.0.6/voip_utils.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      785 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-05-01 15:26:07.000000 voip-utils-0.0.6/voip_utils.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.6/voip_utils.egg-info/zip-safe
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-02 19:51:42.322296 voip-utils-0.0.7/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.7/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      785 2023-05-02 19:51:42.322296 voip-utils-0.0.7/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.7/README.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1977 2023-05-02 19:51:07.000000 voip-utils-0.0.7/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-05-02 19:51:42.322296 voip-utils-0.0.7/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-02 19:51:42.322296 voip-utils-0.0.7/voip_utils/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.7/voip_utils/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       83 2023-05-02 19:50:57.000000 voip-utils-0.0.7/voip_utils/const.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.7/voip_utils/error.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7281 2023-05-02 19:50:57.000000 voip-utils-0.0.7/voip_utils/rtp_audio.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7755 2023-05-02 19:50:57.000000 voip-utils-0.0.7/voip_utils/sip.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.7/voip_utils/util.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6443 2023-05-02 19:50:57.000000 voip-utils-0.0.7/voip_utils/voip.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-02 19:51:42.322296 voip-utils-0.0.7/voip_utils.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      785 2023-05-02 19:51:42.000000 voip-utils-0.0.7/voip_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      386 2023-05-02 19:51:42.000000 voip-utils-0.0.7/voip_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-02 19:51:42.000000 voip-utils-0.0.7/voip_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-05-02 19:51:42.000000 voip-utils-0.0.7/voip_utils.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-05-02 19:51:42.000000 voip-utils-0.0.7/voip_utils.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.7/voip_utils.egg-info/zip-safe
```

### Comparing `voip-utils-0.0.6/LICENSE.md` & `voip-utils-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.6/PKG-INFO` & `voip-utils-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant-libs/voip-utils
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `voip-utils-0.0.6/pyproject.toml` & `voip-utils-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "voip-utils"
-version     = "0.0.6"
+version     = "0.0.7"
 license     = {text = "Apache-2.0"}
 description = "Voice over IP Utilities"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "voip", "phone"]
```

### Comparing `voip-utils-0.0.6/voip_utils/rtp_audio.py` & `voip-utils-0.0.7/voip_utils/rtp_audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 import struct
 from collections.abc import Iterable
 from dataclasses import dataclass
 from typing import Any
 
 import opuslib
 
+from .const import OPUS_PAYLOAD_TYPE
 from .error import RtpError
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
 class RtpOpusInput:
     """Extracts audio from RTP packets with OPUS."""
 
     opus_rate: int = 48000  # Hz
     opus_width: int = 2  # bytes
     opus_channels: int = 2
     opus_frame_size: int = 960  # samples per channel
-    opus_payload: int = 123  # set by GrandStream
+    opus_payload_type: int = OPUS_PAYLOAD_TYPE  # set by GrandStream
 
     def __post_init__(
         self,
     ) -> None:
         """Initialize encoder and state."""
         self._decoder = opuslib.api.decoder.create_state(
             self.opus_rate, self.opus_channels
@@ -52,17 +53,17 @@
             ">BBHLL", rtp_bytes[:12]
         )
 
         if flags != 0b10000000:
             raise RtpError("Padding and extension headers not supported")
 
         payload_type &= 0x7F  # Remove marker bit
-        if payload_type != self.opus_payload:
+        if payload_type != self.opus_payload_type:
             raise RtpError(
-                f"Expected payload type {self.opus_payload}, got {payload_type}"
+                f"Expected payload type {self.opus_payload_type}, got {payload_type}"
             )
 
         # Assume no padding, extension headers, etc.
         opus_bytes = rtp_bytes[12:]
 
         # Decode into raw audio.
         # This will always be 48Khz stereo with 16-bit samples.
@@ -110,15 +111,15 @@
 class RtpOpusOutput:
     """Prepares audio to send to an RTP client using OPUS."""
 
     opus_rate: int = 48000  # Hz
     opus_width: int = 2  # bytes
     opus_channels: int = 2
     opus_frame_size: int = 960  # samples per channel
-    opus_payload: int = 123  # set by GrandStream
+    opus_payload_type: int = OPUS_PAYLOAD_TYPE  # set by GrandStream
     opus_bytes_per_frame: int = 960 * 2 * 2  # 16-bit x stereo
 
     _rtp_flags: int = 0b10000000  # v2, no padding/extensions/CSRCs
     _rtp_sequence_num: int = 0
     _rtp_timestamp: int = 0
     _rtp_ssrc: int = 0
 
@@ -217,15 +218,15 @@
             )
 
             # Add RTP header
             # See: https://en.wikipedia.org/wiki/Real-time_Transport_Protocol#Packet_header
             rtp_bytes = struct.pack(
                 ">BBHLL",
                 self._rtp_flags,
-                self.opus_payload,
+                self.opus_payload_type,
                 self._rtp_sequence_num,
                 self._rtp_timestamp,
                 self._rtp_ssrc,
             )
 
             # RTP packet
             yield rtp_bytes + opus_bytes
```

### Comparing `voip-utils-0.0.6/voip_utils/sip.py` & `voip-utils-0.0.7/voip_utils/sip.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import asyncio
 import logging
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Dict, Optional, Tuple
 
+from .const import OPUS_PAYLOAD_TYPE
 from .error import VoipError
 from .util import is_ipv4_address
 
 SIP_PORT = 5060
 
 _LOGGER = logging.getLogger(__name__)
 _CRLF = "\r\n"
-_OPUS_PAYLOAD = "123"
 
 
 @dataclass
 class SdpInfo:
     """Information for Session Description Protocol (SDP)."""
 
     username: str
@@ -31,24 +31,24 @@
     """Information gathered from an INVITE message."""
 
     caller_ip: str
     caller_sip_port: int
     caller_rtp_port: int
     server_ip: str
     headers: dict[str, str]
+    opus_payload_type: int = OPUS_PAYLOAD_TYPE
 
 
 class SipDatagramProtocol(asyncio.DatagramProtocol, ABC):
     """UDP server for the Session Initiation Protocol (SIP)."""
 
     def __init__(self, sdp_info: SdpInfo) -> None:
         """Set up SIP server."""
         self.sdp_info = sdp_info
         self.transport = None
-        self._opus_payload = _OPUS_PAYLOAD
 
     def connection_made(self, transport):
         """Server ready."""
         self.transport = transport
 
     def datagram_received(self, data: bytes, addr):
         """Handle INVITE SIP messages."""
@@ -69,14 +69,15 @@
                 caller_ip,
                 caller_sip_port,
             )
 
             # Extract caller's RTP port from SDP.
             # See: https://datatracker.ietf.org/doc/html/rfc2327
             caller_rtp_port: Optional[int] = None
+            opus_payload_type = OPUS_PAYLOAD_TYPE
             body_lines = body.splitlines()
             for line in body_lines:
                 line = line.strip()
                 if line:
                     key, value = line.split("=", maxsplit=1)
                     if key == "m":
                         parts = value.split()
@@ -85,17 +86,17 @@
                     elif key == "a" and value.startswith("rtpmap:"):
                         # a=rtpmap:123 opus/48000/2
                         codec_str = value.split(":", maxsplit=1)[1]
                         codec_parts = codec_str.split()
                         if (len(codec_parts) > 1) and (
                             codec_parts[1].lower().startswith("opus")
                         ):
-                            self._opus_payload = codec_parts[0]
+                            opus_payload_type = int(codec_parts[0])
                             _LOGGER.debug(
-                                "Detected OPUS payload type as %s", self._opus_payload
+                                "Detected OPUS payload type as %s", opus_payload_type
                             )
 
             if caller_rtp_port is None:
                 raise VoipError("No caller RTP port")
 
             # Extract host from ruri
             # sip:user@123.123.123.123:1234
@@ -122,14 +123,15 @@
             self.on_call(
                 CallInfo(
                     caller_ip=caller_ip,
                     caller_sip_port=caller_sip_port,
                     caller_rtp_port=caller_rtp_port,
                     server_ip=server_ip,
                     headers=headers,
+                    opus_payload_type=opus_payload_type,
                 )
             )
         except Exception:
             _LOGGER.exception("Unexpected error handling SIP INVITE")
 
     @abstractmethod
     def on_call(self, call_info: CallInfo):
@@ -148,16 +150,16 @@
         # See: https://datatracker.ietf.org/doc/html/rfc2327
         body_lines = [
             "v=0",
             f"o={self.sdp_info.username} {self.sdp_info.id} 1 IN IP4 {call_info.server_ip}",
             f"s={self.sdp_info.session_name}",
             f"c=IN IP4 {call_info.server_ip}",
             "t=0 0",
-            f"m=audio {server_rtp_port} RTP/AVP {self._opus_payload}",
-            f"a=rtpmap:{_OPUS_PAYLOAD} opus/48000/2",
+            f"m=audio {server_rtp_port} RTP/AVP {call_info.opus_payload_type}",
+            f"a=rtpmap:{call_info.opus_payload_type} opus/48000/2",
             "a=ptime:20",
             "a=maxptime:150",
             "a=sendrecv",
             _CRLF,
         ]
         body = _CRLF.join(body_lines)
```

### Comparing `voip-utils-0.0.6/voip_utils/voip.py` & `voip-utils-0.0.7/voip_utils/voip.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import socket
 import time
 from abc import ABC, abstractmethod
 from functools import partial
 from typing import Any, Callable, Optional, Set
 
+from .const import OPUS_PAYLOAD_TYPE
 from .rtp_audio import RtpOpusInput, RtpOpusOutput
 from .sip import CallInfo, SdpInfo, SipDatagramProtocol
 
 _LOGGER = logging.getLogger(__name__)
 
 CallProtocolFactory = Callable[[CallInfo], asyncio.Protocol]
 
@@ -76,27 +77,28 @@
     """Handle RTP audio input/output for a VoIP call."""
 
     def __init__(
         self,
         rate: int = 16000,
         width: int = 2,
         channels: int = 1,
+        opus_payload_type: int = OPUS_PAYLOAD_TYPE,
     ) -> None:
         """Set up RTP server."""
         # Desired format for input audio
         self.rate = rate
         self.width = width
         self.channels = channels
 
         self.transport = None
         self.addr = None
 
         self._audio_queue: "asyncio.Queue[bytes]" = asyncio.Queue()
-        self._rtp_input = RtpOpusInput()
-        self._rtp_output = RtpOpusOutput()
+        self._rtp_input = RtpOpusInput(opus_payload_type=opus_payload_type)
+        self._rtp_output = RtpOpusOutput(opus_payload_type=opus_payload_type)
         self._is_connected: bool = False
 
     def disconnect(self):
         self._is_connected = False
         if self.transport is not None:
             self.transport.close()
             self.transport = None
```

### Comparing `voip-utils-0.0.6/voip_utils.egg-info/PKG-INFO` & `voip-utils-0.0.7/voip_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant-libs/voip-utils
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

