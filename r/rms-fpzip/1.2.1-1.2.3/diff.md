# Comparing `tmp/rms_fpzip-1.2.1-cp39-cp39-win_amd64.whl.zip` & `tmp/rms_fpzip-1.2.3-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 98741 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   299008 b- defN 23-May-02 03:40 fpzip.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      148 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/AUTHORS
--rw-rw-rw-  2.0 fat     1556 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3439 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      568 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/RECORD
-7 files, 304825 bytes uncompressed, 97735 bytes compressed:  67.9%
+Zip file size: 130547 bytes, number of entries: 7
+-rwxr-xr-x  2.0 unx   525840 b- defN 23-May-02 18:29 fpzip.cpython-310-darwin.so
+-rw-rw-r--  2.0 unx      578 b- defN 23-May-02 18:29 rms_fpzip-1.2.3.dist-info/RECORD
+-rw-r--r--  2.0 unx     1527 b- defN 23-May-02 18:29 rms_fpzip-1.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      145 b- defN 23-May-02 18:29 rms_fpzip-1.2.3.dist-info/AUTHORS
+-rw-r--r--  2.0 unx      111 b- defN 23-May-02 18:29 rms_fpzip-1.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-02 18:29 rms_fpzip-1.2.3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     3363 b- defN 23-May-02 18:29 rms_fpzip-1.2.3.dist-info/METADATA
+7 files, 531570 bytes uncompressed, 129535 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: fpzip.cp39-win_amd64.pyd
+Filename: fpzip.cpython-310-darwin.so
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/AUTHORS
+Filename: rms_fpzip-1.2.3.dist-info/RECORD
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/LICENSE
+Filename: rms_fpzip-1.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/METADATA
+Filename: rms_fpzip-1.2.3.dist-info/AUTHORS
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/WHEEL
+Filename: rms_fpzip-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/top_level.txt
+Filename: rms_fpzip-1.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/RECORD
+Filename: rms_fpzip-1.2.3.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## Comparing `rms_fpzip-1.2.1.dist-info/LICENSE` & `rms_fpzip-1.2.3.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, William Silversmith
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, William Silversmith
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

## Comparing `rms_fpzip-1.2.1.dist-info/METADATA` & `rms_fpzip-1.2.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 2.1
-Name: rms-fpzip
-Version: 1.2.1
-Summary: Numpy wrapper for fpzip algorithm (P. Lindstrom & M. Isenburg, 2006) RMS Fork
-Home-page: https://github.com/seung-lab/fpzip/
-Author: William Silversmith
-Author-email: ws9@princeton.edu
-Maintainer: Robert French
-Maintainer-email: rfrench@seti.org
-License: None
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Archiving :: Compression
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
-[![PyPI version](https://badge.fury.io/py/rms-fpzip.svg)](https://badge.fury.io/py/rms-fpzip)
-
-# Introduction
-
-This is a fork of https://github.com/seung-lab/fpzip with changes to allow it to work
-with Python 3.11 and also have a different PyPI deployment system.
-
-This fork is maintained by the Ring-Moon Systems Node of NASA's Planetary Data System.
-
-# fpzip
-
-fpzip is a compression algorithm supporting lossless and lossy encoding for up to 4 dimensional floating point data. This package contains Python C++ bindings for the fpzip algorithm (version 1.3.0). The version number for this package is independent. Python 3.7+ is supported.
-
-```python
-import fpzip
-import numpy as np
-
-data = np.array(..., dtype=np.float32) # up to 4d float or double array
-# Compress data losslessly, interpreting the underlying buffer in C (default) or F order.
-compressed_bytes = fpzip.compress(data, precision=0, order='C') # returns byte string
-# Back to 3d or 4d float or double array, decode as C (default) or F order.
-data_again = fpzip.decompress(compressed_bytes, order='C')
-```
-
-## Installation
-
-#### `pip` Binary Installation
-
-```bash
-pip install fpzip
-```
-
-If we have a precompiled binary available the above command should just work. However, if you have to compile from source, it's unfortunately necessary to install numpy first because of a quirk in the Python installation procedure that won't easily recognize when a numpy installation completes in the same process. There are some hacks, but I haven't gotten them to work.
-
-#### `pip` Source Installation
-
-*Requires C++ compiler.*
-
-```bash
-pip install numpy
-pip install fpzip
-```
-
-#### Direct Installation
-
-*Requires C++ compiler.*
-
-```bash
-$ pip install numpy
-$ python setup.py develop
-```
-
-## References
-
-Algorithm and C++ code by Peter Lindstrom and Martin Isenburg. Cython interface code by William Silversmith. Check out [Dr. Lindstrom's site](https://computing.llnl.gov/projects/fpzip) or the [fpzip Github page](https://github.com/LLNL/fpzip).
-
-1. Peter Lindstrom and Martin Isenburg, "[Fast and Efficient Compression of Floating-Point Data,](https://www.researchgate.net/publication/6715625_Fast_and_Efficient_Compression_of_Floating-Point_Data)" IEEE Transactions on Visualization and Computer Graphics, 12(5):1245-1250, September-October 2006, doi:[10.1109/TVCG.2006.143](http://dx.doi.org/10.1109/TVCG.2006.143).
+Metadata-Version: 2.1
+Name: rms-fpzip
+Version: 1.2.3
+Summary: Numpy wrapper for fpzip algorithm (P. Lindstrom & M. Isenburg, 2006) RMS Fork
+Home-page: https://github.com/SETI/pds-fpzip/
+Author: William Silversmith
+Author-email: ws9@princeton.edu
+Maintainer: Robert French
+Maintainer-email: rfrench@seti.org
+License: None
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Archiving :: Compression
+Requires-Python: ~=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+[![PyPI version](https://badge.fury.io/py/rms-fpzip.svg)](https://badge.fury.io/py/rms-fpzip)
+
+# Introduction
+
+This is a fork of https://github.com/seung-lab/fpzip with changes to allow it to work
+with Python 3.11 and also have a different PyPI deployment system.
+
+This fork is maintained by the Ring-Moon Systems Node of NASA's Planetary Data System.
+
+# fpzip
+
+fpzip is a compression algorithm supporting lossless and lossy encoding for up to 4 dimensional floating point data. This package contains Python C++ bindings for the fpzip algorithm (version 1.3.0). The version number for this package is independent. Python 3.7+ is supported.
+
+```python
+import fpzip
+import numpy as np
+
+data = np.array(..., dtype=np.float32) # up to 4d float or double array
+# Compress data losslessly, interpreting the underlying buffer in C (default) or F order.
+compressed_bytes = fpzip.compress(data, precision=0, order='C') # returns byte string
+# Back to 3d or 4d float or double array, decode as C (default) or F order.
+data_again = fpzip.decompress(compressed_bytes, order='C')
+```
+
+## Installation
+
+#### `pip` Binary Installation
+
+```bash
+pip install rms-fpzip
+```
+
+If we have a precompiled binary available the above command should just work. However, if you have to compile from source, it's unfortunately necessary to install numpy first because of a quirk in the Python installation procedure that won't easily recognize when a numpy installation completes in the same process. There are some hacks, but I haven't gotten them to work.
+
+#### `pip` Source Installation
+
+*Requires C++ compiler.*
+
+```bash
+pip install numpy
+pip install rms-fpzip
+```
+
+#### Direct Installation
+
+*Requires C++ compiler.*
+
+```bash
+$ pip install numpy
+$ python setup.py develop
+```
+
+## References
+
+Algorithm and C++ code by Peter Lindstrom and Martin Isenburg. Cython interface code by William Silversmith. Check out [Dr. Lindstrom's site](https://computing.llnl.gov/projects/fpzip) or the [fpzip Github page](https://github.com/LLNL/fpzip).
+
+1. Peter Lindstrom and Martin Isenburg, "[Fast and Efficient Compression of Floating-Point Data,](https://www.researchgate.net/publication/6715625_Fast_and_Efficient_Compression_of_Floating-Point_Data)" IEEE Transactions on Visualization and Computer Graphics, 12(5):1245-1250, September-October 2006, doi:[10.1109/TVCG.2006.143](http://dx.doi.org/10.1109/TVCG.2006.143).
```

## Comparing `rms_fpzip-1.2.1.dist-info/RECORD` & `rms_fpzip-1.2.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-fpzip.cp39-win_amd64.pyd,sha256=LrbvKPJo4IFZ-xUS22iqvae6fB3WHKrjjG6H8sUjhPA,299008
-rms_fpzip-1.2.1.dist-info/AUTHORS,sha256=DWcBA-LLUE0rjzUE8xVO4sA1KzwxWIja0Iu7M1XhvGo,148
-rms_fpzip-1.2.1.dist-info/LICENSE,sha256=8BpZRbaM_5v8SwQlwhblgue4osr-URIVpjiJ7R-Iec8,1556
-rms_fpzip-1.2.1.dist-info/METADATA,sha256=uIxx5qUZHq3FCYBpMlxXbygQ0SQOJ6gv4Wj1a7hJ41Q,3439
-rms_fpzip-1.2.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-rms_fpzip-1.2.1.dist-info/top_level.txt,sha256=FTQGjjMLAGhaiyzBJhAZTrMW7rzMdVpM-moiFbFZMVk,6
-rms_fpzip-1.2.1.dist-info/RECORD,,
+fpzip.cpython-310-darwin.so,sha256=ino7yKM2qRwgxiV_LXW1kSuWvUzvSBxNgiFkLLITat4,525840
+rms_fpzip-1.2.3.dist-info/RECORD,,
+rms_fpzip-1.2.3.dist-info/LICENSE,sha256=suvI3Zn_lBC4LsFTqRK6seDM6gSavT6CPkB6G8eqxxo,1527
+rms_fpzip-1.2.3.dist-info/AUTHORS,sha256=Vbo3Fw2d8ds_JA9eljQboB3gUG-kmtA41jU0e8YLoZw,145
+rms_fpzip-1.2.3.dist-info/WHEEL,sha256=doY7Ynwndq62v9G9yH4QQiKEI6qNEsMeVrkmo76vHLE,111
+rms_fpzip-1.2.3.dist-info/top_level.txt,sha256=FTQGjjMLAGhaiyzBJhAZTrMW7rzMdVpM-moiFbFZMVk,6
+rms_fpzip-1.2.3.dist-info/METADATA,sha256=tQObcwD7WlxsJSY2jOcP34o7Kk9xaJXoW5cgVOvCLT8,3363
```

