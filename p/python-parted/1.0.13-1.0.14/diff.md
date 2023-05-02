# Comparing `tmp/python-parted-1.0.13.tar.gz` & `tmp/python_parted-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-parted-1.0.13.tar", max compression
+gzip compressed data, was "python_parted-1.0.14.tar", max compression
```

## Comparing `python-parted-1.0.13.tar` & `python_parted-1.0.14.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1596 2022-09-03 22:30:15.668686 python-parted-1.0.13/LICENSE
--rw-r--r--   0        0        0      342 2022-09-20 17:11:56.991217 python-parted-1.0.13/README.md
--rw-r--r--   0        0        0    27877 2022-09-28 20:00:39.477913 python-parted-1.0.13/build.py
--rw-r--r--   0        0        0      672 2022-09-27 20:14:12.975319 python-parted-1.0.13/docs/Makefile
--rw-r--r--   0        0        0      804 2022-09-17 09:42:27.371559 python-parted-1.0.13/docs/make.bat
--rw-r--r--   0        0        0     1283 2022-09-27 20:19:01.809332 python-parted-1.0.13/docs/source/conf.py
--rw-r--r--   0        0        0      494 2022-09-17 21:22:29.390240 python-parted-1.0.13/docs/source/index.rst
--rw-r--r--   0        0        0      136 2022-09-17 18:05:18.932654 python-parted-1.0.13/docs/source/parted.alignment.rst
--rw-r--r--   0        0        0      139 2022-09-17 18:05:18.932654 python-parted-1.0.13/docs/source/parted.constraint.rst
--rw-r--r--   0        0        0      127 2022-09-17 18:05:18.932654 python-parted-1.0.13/docs/source/parted.device.rst
--rw-r--r--   0        0        0      121 2022-09-17 18:05:18.936654 python-parted-1.0.13/docs/source/parted.disk.rst
--rw-r--r--   0        0        0      139 2022-09-17 18:05:18.936654 python-parted-1.0.13/docs/source/parted.exceptions.rst
--rw-r--r--   0        0        0      124 2022-09-17 18:05:18.936654 python-parted-1.0.13/docs/source/parted.excpt.rst
--rw-r--r--   0        0        0      130 2022-09-17 18:05:18.940654 python-parted-1.0.13/docs/source/parted.filesys.rst
--rw-r--r--   0        0        0      121 2022-09-17 18:05:18.940654 python-parted-1.0.13/docs/source/parted.geom.rst
--rw-r--r--   0        0        0      336 2022-09-17 18:08:46.109657 python-parted-1.0.13/docs/source/parted.rst
--rw-r--r--   0        0        0      124 2022-09-17 18:05:18.940654 python-parted-1.0.13/docs/source/parted.timer.rst
--rw-r--r--   0        0        0      121 2022-09-17 18:05:18.944654 python-parted-1.0.13/docs/source/parted.util.rst
--rw-r--r--   0        0        0      155 2022-09-17 14:21:41.265355 python-parted-1.0.13/docs/source/usage.rst
--rw-r--r--   0        0        0     2668 2022-09-19 18:47:44.567750 python-parted-1.0.13/parted/__init__.py
--rw-r--r--   0        0        0    10518 2022-10-26 18:18:09.621120 python-parted-1.0.13/parted/alignment.py
--rw-r--r--   0        0        0    16370 2022-10-26 18:18:44.073349 python-parted-1.0.13/parted/constraint.py
--rw-r--r--   0        0        0    25120 2022-10-26 18:19:02.049469 python-parted-1.0.13/parted/device.py
--rw-r--r--   0        0        0    41410 2022-10-26 18:37:10.539204 python-parted-1.0.13/parted/disk.py
--rw-r--r--   0        0        0     3401 2022-09-18 21:37:06.415547 python-parted-1.0.13/parted/exceptions.py
--rw-r--r--   0        0        0     9382 2022-10-26 18:20:29.126140 python-parted-1.0.13/parted/excpt.py
--rw-r--r--   0        0        0     9611 2022-10-26 18:22:49.135650 python-parted-1.0.13/parted/filesys.py
--rw-r--r--   0        0        0    16661 2022-10-26 18:23:40.264171 python-parted-1.0.13/parted/geom.py
--rw-r--r--   0        0        0     8240 2022-10-26 18:23:59.928367 python-parted-1.0.13/parted/timer.py
--rw-r--r--   0        0        0     7146 2022-09-25 17:54:15.783686 python-parted-1.0.13/parted/util.py
--rw-r--r--   0        0        0     2056 2022-10-26 18:38:33.499853 python-parted-1.0.13/pyproject.toml
--rw-r--r--   0        0        0     1680 2022-09-03 20:03:48.168386 python-parted-1.0.13/tests/__init__.py
--rw-r--r--   0        0        0    14974 2022-09-18 17:54:08.282230 python-parted-1.0.13/tests/test_alignment.py
--rw-r--r--   0        0        0    13859 2022-10-26 18:29:25.099377 python-parted-1.0.13/tests/test_constraint.py
--rw-r--r--   0        0        0    15594 2022-10-26 18:25:53.057461 python-parted-1.0.13/tests/test_device.py
--rw-r--r--   0        0        0    14533 2022-10-26 18:37:37.823418 python-parted-1.0.13/tests/test_disk.py
--rw-r--r--   0        0        0     2045 2022-10-26 18:26:36.021862 python-parted-1.0.13/tests/test_exception.py
--rw-r--r--   0        0        0     4545 2022-10-26 18:27:07.714153 python-parted-1.0.13/tests/test_filesys.py
--rw-r--r--   0        0        0     8188 2022-10-26 18:27:18.326250 python-parted-1.0.13/tests/test_geometry.py
--rw-r--r--   0        0        0    14443 2022-10-26 18:27:28.174339 python-parted-1.0.13/tests/test_partition.py
--rw-r--r--   0        0        0     2032 2022-10-26 18:27:37.854427 python-parted-1.0.13/tests/test_timer.py
--rw-r--r--   0        0        0     7327 2022-09-11 22:05:37.643649 python-parted-1.0.13/tests/util/__init__.py
--rw-r--r--   0        0        0    17842 2022-09-05 14:21:05.125147 python-parted-1.0.13/tests/util/gptdsk.py
--rw-r--r--   0        0        0    18087 2022-09-05 14:21:05.125147 python-parted-1.0.13/tests/util/msdosdsk.py
--rw-r--r--   0        0        0     3440 2022-09-10 20:11:34.875465 python-parted-1.0.13/tests/util/partedtest.py
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 python-parted-1.0.13/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-02 15:06:52.033475 python_parted-1.0.14/LICENSE
+-rw-r--r--   0        0        0      342 2022-09-20 17:11:56.991217 python_parted-1.0.14/README.md
+-rw-r--r--   0        0        0    27877 2022-09-28 20:00:39.477913 python_parted-1.0.14/build.py
+-rw-r--r--   0        0        0      672 2022-09-27 20:14:12.975319 python_parted-1.0.14/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-09-17 09:42:27.371559 python_parted-1.0.14/docs/make.bat
+-rw-r--r--   0        0        0     1283 2022-09-27 20:19:01.809332 python_parted-1.0.14/docs/source/conf.py
+-rw-r--r--   0        0        0      494 2022-09-17 21:22:29.390240 python_parted-1.0.14/docs/source/index.rst
+-rw-r--r--   0        0        0      136 2022-09-17 18:05:18.932654 python_parted-1.0.14/docs/source/parted.alignment.rst
+-rw-r--r--   0        0        0      139 2022-09-17 18:05:18.932654 python_parted-1.0.14/docs/source/parted.constraint.rst
+-rw-r--r--   0        0        0      127 2022-09-17 18:05:18.932654 python_parted-1.0.14/docs/source/parted.device.rst
+-rw-r--r--   0        0        0      121 2022-09-17 18:05:18.936654 python_parted-1.0.14/docs/source/parted.disk.rst
+-rw-r--r--   0        0        0      139 2022-09-17 18:05:18.936654 python_parted-1.0.14/docs/source/parted.exceptions.rst
+-rw-r--r--   0        0        0      124 2022-09-17 18:05:18.936654 python_parted-1.0.14/docs/source/parted.excpt.rst
+-rw-r--r--   0        0        0      130 2022-09-17 18:05:18.940654 python_parted-1.0.14/docs/source/parted.filesys.rst
+-rw-r--r--   0        0        0      121 2022-09-17 18:05:18.940654 python_parted-1.0.14/docs/source/parted.geom.rst
+-rw-r--r--   0        0        0      336 2022-09-17 18:08:46.109657 python_parted-1.0.14/docs/source/parted.rst
+-rw-r--r--   0        0        0      124 2022-09-17 18:05:18.940654 python_parted-1.0.14/docs/source/parted.timer.rst
+-rw-r--r--   0        0        0      121 2022-09-17 18:05:18.944654 python_parted-1.0.14/docs/source/parted.util.rst
+-rw-r--r--   0        0        0      155 2022-09-17 14:21:41.265355 python_parted-1.0.14/docs/source/usage.rst
+-rw-r--r--   0        0        0     2668 2022-09-19 18:47:44.567750 python_parted-1.0.14/parted/__init__.py
+-rw-r--r--   0        0        0    10023 2023-05-02 15:27:59.676306 python_parted-1.0.14/parted/alignment.py
+-rw-r--r--   0        0        0    15841 2023-05-02 15:28:06.724366 python_parted-1.0.14/parted/constraint.py
+-rw-r--r--   0        0        0    24591 2023-05-02 15:28:13.632425 python_parted-1.0.14/parted/device.py
+-rw-r--r--   0        0        0    40881 2023-05-02 15:28:38.236635 python_parted-1.0.14/parted/disk.py
+-rw-r--r--   0        0        0     2872 2023-05-02 15:28:45.476697 python_parted-1.0.14/parted/exceptions.py
+-rw-r--r--   0        0        0     8853 2023-05-02 15:28:53.440765 python_parted-1.0.14/parted/excpt.py
+-rw-r--r--   0        0        0     9082 2023-05-02 15:29:02.672844 python_parted-1.0.14/parted/filesys.py
+-rw-r--r--   0        0        0    16132 2023-05-02 15:29:11.076916 python_parted-1.0.14/parted/geom.py
+-rw-r--r--   0        0        0     7711 2023-05-02 15:29:21.297003 python_parted-1.0.14/parted/timer.py
+-rw-r--r--   0        0        0     6615 2023-05-02 15:30:52.969789 python_parted-1.0.14/parted/util.py
+-rw-r--r--   0        0        0     2049 2023-05-02 15:32:02.834389 python_parted-1.0.14/pyproject.toml
+-rw-r--r--   0        0        0     1680 2022-09-03 20:03:48.168386 python_parted-1.0.14/tests/__init__.py
+-rw-r--r--   0        0        0    14445 2023-05-02 15:29:32.209097 python_parted-1.0.14/tests/test_alignment.py
+-rw-r--r--   0        0        0    13330 2023-05-02 15:29:39.353158 python_parted-1.0.14/tests/test_constraint.py
+-rw-r--r--   0        0        0    15065 2023-05-02 15:29:45.925214 python_parted-1.0.14/tests/test_device.py
+-rw-r--r--   0        0        0    14004 2023-05-02 15:29:54.417287 python_parted-1.0.14/tests/test_disk.py
+-rw-r--r--   0        0        0     1516 2023-05-02 15:30:00.637340 python_parted-1.0.14/tests/test_exception.py
+-rw-r--r--   0        0        0     4016 2023-05-02 15:30:07.001395 python_parted-1.0.14/tests/test_filesys.py
+-rw-r--r--   0        0        0     7659 2023-05-02 15:30:12.657443 python_parted-1.0.14/tests/test_geometry.py
+-rw-r--r--   0        0        0    13914 2023-05-02 15:30:18.573494 python_parted-1.0.14/tests/test_partition.py
+-rw-r--r--   0        0        0     1503 2023-05-02 15:30:24.701546 python_parted-1.0.14/tests/test_timer.py
+-rw-r--r--   0        0        0     7327 2022-09-11 22:05:37.643649 python_parted-1.0.14/tests/util/__init__.py
+-rw-r--r--   0        0        0    17842 2022-09-05 14:21:05.125147 python_parted-1.0.14/tests/util/gptdsk.py
+-rw-r--r--   0        0        0    18087 2022-09-05 14:21:05.125147 python_parted-1.0.14/tests/util/msdosdsk.py
+-rw-r--r--   0        0        0     2911 2023-05-02 15:30:50.137765 python_parted-1.0.14/tests/util/partedtest.py
+-rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 python_parted-1.0.14/PKG-INFO
```

### Comparing `python-parted-1.0.13/LICENSE` & `python_parted-1.0.14/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+#
 # Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #    * Redistributions of source code must retain the above copyright notice,
@@ -19,7 +21,10 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+"""
+@author: Adolfo Gómez, dkmaster at dkmon dot com
+"""
```

### Comparing `python-parted-1.0.13/build.py` & `python_parted-1.0.14/build.py`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/docs/Makefile` & `python_parted-1.0.14/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/docs/make.bat` & `python_parted-1.0.14/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/docs/source/conf.py` & `python_parted-1.0.14/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/parted/__init__.py` & `python_parted-1.0.14/parted/__init__.py`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/parted/alignment.py` & `python_parted-1.0.14/parted/alignment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 This module contains the Alignment class.
 
 The alignment class is used to specify the alignment of a partition.
 It's a wrapper for the PedAlignment struct. and related functions.
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
@@ -52,15 +44,17 @@
 
     This class wraps the PedAlignment object, and provides a more pythonic interface to itself.
     """
 
     _alignment: typing.Any
     _destroyable: bool
 
-    def __init__(self, alignment_or_offset: typing.Union[int, 'cffi.FFI.CData', None], grain_size: int = 0) -> None:
+    def __init__(
+        self, alignment_or_offset: typing.Union[int, 'cffi.FFI.CData', None], grain_size: int = 0
+    ) -> None:
         """Creates an alignment object
 
         Args:
             alignment_or_offset (typing.Union[int, "cffi.FFI.CData"]): If an int, it's the offset, if a CData, it's the PedAlignment* object
             grain_size (int, optional): Grain size of the aligment. Defaults to 0. (Only used if offset is an int)
 
         Note:
@@ -160,15 +154,17 @@
 
         Returns:
             Alignment: The resulting alignment
 
         Raises:
             exceptions.InvalidObjectError: If the wrapped alignment is not valid
         """
-        return make_destroyable(Alignment(_parted.lib.ped_alignment_intersect(self._alignment, other._alignment)))
+        return make_destroyable(
+            Alignment(_parted.lib.ped_alignment_intersect(self._alignment, other._alignment))
+        )
 
     @ensure_obj
     def align_up(self, geometry: 'geom.Geometry', sector: int) -> int:
         """Returns the closest sector to sector that lies inside geom that satisfies self aligment.
 
         Args:
             geometry (geom.Geometry): The geometry that contains the sector to align
```

### Comparing `python-parted-1.0.13/parted/constraint.py` & `python_parted-1.0.14/parted/constraint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 This module contains the Constraint class, which is used to specify
 the constraints on a Partition.
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import logging
```

### Comparing `python-parted-1.0.13/parted/device.py` & `python_parted-1.0.14/parted/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 This module contains Device and Device related classes
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import typing
 import logging
```

### Comparing `python-parted-1.0.13/parted/disk.py` & `python_parted-1.0.14/parted/disk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 This module contains Disk and Partition related classes
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import enum
 import logging
```

### Comparing `python-parted-1.0.13/parted/exceptions.py` & `python_parted-1.0.14/parted/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 Parted exceptions
 
 This module contains all the exceptions that can be raised by python-parted
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
```

### Comparing `python-parted-1.0.13/parted/excpt.py` & `python_parted-1.0.14/parted/excpt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 Parted library exceptions control module.
 
 This modules contains the mechanism to control exceptions raised by parted
 library, and to threat them on a pythonic way.
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
```

### Comparing `python-parted-1.0.13/parted/filesys.py` & `python_parted-1.0.14/parted/filesys.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 This module contains Filesystem related classes and functions
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 
 from os import stat
```

### Comparing `python-parted-1.0.13/parted/geom.py` & `python_parted-1.0.14/parted/geom.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 
 import typing
 import logging
```

### Comparing `python-parted-1.0.13/parted/timer.py` & `python_parted-1.0.14/parted/timer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 Timer interface to "PedTimer" in parted
 
 :author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import typing
 import logging
```

### Comparing `python-parted-1.0.13/pyproject.toml` & `python_parted-1.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "python-parted"
-version = "1.0.13"
-license = "BSD-3-Clause"
+version = "1.0.14"
+license = "MIT"
 readme = "README.md"
 description = "Python interface to access the parted library"
 authors = ["Adolfo Gómez García <dkmaster@dkmon.com>"]
 packages = [
     {include = "parted"},
 ]
 include = [
@@ -27,15 +27,15 @@
 
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "build.py"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.7.2"
 cffi = ">=1.15.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.3"
 mypy = ">=0.971"
 black = ">=22.8.0"
 ipython = ">=7.0.0"
```

### Comparing `python-parted-1.0.13/tests/test_alignment.py` & `python_parted-1.0.14/tests/test_alignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import typing
 
 from parted import _parted  # type: ignore
 from parted import alignment, geom, exceptions, device
```

### Comparing `python-parted-1.0.13/tests/test_constraint.py` & `python_parted-1.0.14/tests/test_constraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 from hashlib import new
 from parted import _parted  # type: ignore
 from parted import constraint, alignment, geom, device, exceptions, disk
```

### Comparing `python-parted-1.0.13/tests/test_device.py` & `python_parted-1.0.14/tests/test_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 from curses import nonl
 import os
 
 from parted import _parted, constraint  # type: ignore
```

### Comparing `python-parted-1.0.13/tests/test_disk.py` & `python_parted-1.0.14/tests/test_disk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import logging
 
 from parted import _parted  # type: ignore
 from parted import disk, exceptions, excpt, device, constraint, geom, timer
```

### Comparing `python-parted-1.0.13/tests/test_exception.py` & `python_parted-1.0.14/tests/test_exception.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 from parted import _parted  # type: ignore
 from parted import constraint, excpt, device
 
 from tests.util import partedtest
```

### Comparing `python-parted-1.0.13/tests/test_filesys.py` & `python_parted-1.0.14/tests/test_filesys.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import logging
 
 from parted import _parted  # type: ignore
 from parted import filesys, exceptions, device, geom
```

### Comparing `python-parted-1.0.13/tests/test_geometry.py` & `python_parted-1.0.14/tests/test_geometry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import io
 import typing
 
 from parted import _parted  # type: ignore
```

### Comparing `python-parted-1.0.13/tests/test_partition.py` & `python_parted-1.0.14/tests/test_partition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Adolfo Gómez
 #
-# Copyright (c) 2022 Adolfo Gómez García <dkmaster at dkmon dot com>
-# All rights reserved.
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#    * Redistributions of source code must retain the above copyright notice,
-#      this list of conditions and the following disclaimer.
-#    * Redistributions in binary form must reproduce the above copyright notice,
-#      this list of conditions and the following disclaimer in the documentation
-#      and/or other materials provided with the distribution.
-#    * Neither the name of Adolfo Gómez García nor the names of its contributors
-#      may be used to endorse or promote products derived from this software
-#      without specific prior written permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 @author: Adolfo Gómez, dkmaster at dkmon dot com
 """
 import typing
 import logging
 
 from parted import _parted  # type: ignore
```

### Comparing `python-parted-1.0.13/tests/util/__init__.py` & `python_parted-1.0.14/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/tests/util/gptdsk.py` & `python_parted-1.0.14/tests/util/gptdsk.py`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/tests/util/msdosdsk.py` & `python_parted-1.0.14/tests/util/msdosdsk.py`

 * *Files identical despite different names*

### Comparing `python-parted-1.0.13/PKG-INFO` & `python_parted-1.0.14/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: python-parted
-Version: 1.0.13
+Version: 1.0.14
 Summary: Python interface to access the parted library
-License: BSD-3-Clause
+License: MIT
 Author: Adolfo Gómez García
 Author-email: dkmaster@dkmon.com
-Requires-Python: >=3.7
+Requires-Python: >=3.7.2
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Filesystems
 Requires-Dist: cffi (>=1.15.1)
 Description-Content-Type: text/markdown
 
 python-parted
 =============
```

