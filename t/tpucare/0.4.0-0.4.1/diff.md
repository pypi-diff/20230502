# Comparing `tmp/tpucare-0.4.0.tar.gz` & `tmp/tpucare-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpucare-0.4.0.tar", last modified: Tue Nov 15 09:45:51 2022, max compression
+gzip compressed data, was "tpucare-0.4.1.tar", last modified: Tue May  2 17:46:46 2023, max compression
```

## Comparing `tpucare-0.4.0.tar` & `tpucare-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-15 09:45:51.667734 tpucare-0.4.0/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      137 2022-08-06 21:35:28.000000 tpucare-0.4.0/.deepsource.toml
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1928 2022-07-14 13:23:22.000000 tpucare-0.4.0/.gitignore
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1348 2022-07-14 13:23:22.000000 tpucare-0.4.0/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8385 2022-11-15 09:45:51.665732 tpucare-0.4.0/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7752 2022-07-17 14:38:00.000000 tpucare-0.4.0/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       68 2022-07-14 16:56:32.000000 tpucare-0.4.0/build.sh
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-15 09:45:51.600812 tpucare-0.4.0/examples/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4700 2022-07-17 14:36:34.000000 tpucare-0.4.0/examples/pod.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2711 2022-07-17 14:37:40.000000 tpucare-0.4.0/examples/sweep.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2022-11-15 09:45:51.668733 tpucare-0.4.0/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1139 2022-11-15 09:45:00.000000 tpucare-0.4.0/setup.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-15 09:45:51.611969 tpucare-0.4.0/tpucare/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10541 2022-11-15 09:43:49.000000 tpucare-0.4.0/tpucare/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-15 09:45:51.654612 tpucare-0.4.0/tpucare.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8385 2022-11-15 09:45:50.000000 tpucare-0.4.0/tpucare.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      241 2022-11-15 09:45:51.000000 tpucare-0.4.0/tpucare.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-15 09:45:51.000000 tpucare-0.4.0/tpucare.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        8 2022-11-15 09:45:51.000000 tpucare-0.4.0/tpucare.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-02 17:46:46.222448 tpucare-0.4.1/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-02 17:44:22.000000 tpucare-0.4.1/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-02 17:46:46.222448 tpucare-0.4.1/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7570 2023-05-02 17:44:22.000000 tpucare-0.4.1/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-02 17:46:46.222448 tpucare-0.4.1/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1106 2023-05-02 17:45:50.000000 tpucare-0.4.1/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-02 17:46:46.222448 tpucare-0.4.1/tpucare/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    10299 2023-05-02 17:45:28.000000 tpucare-0.4.1/tpucare/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-02 17:46:46.222448 tpucare-0.4.1/tpucare.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-02 17:46:46.000000 tpucare-0.4.1/tpucare.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      170 2023-05-02 17:46:46.000000 tpucare-0.4.1/tpucare.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-02 17:46:46.000000 tpucare-0.4.1/tpucare.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-02 17:46:46.000000 tpucare-0.4.1/tpucare.egg-info/top_level.txt
```

### Comparing `tpucare-0.4.0/LICENSE` & `tpucare-0.4.1/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-BSD 2-Clause License
-
-Copyright (c) 2022, Lucas Nestler
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
+BSD 2-Clause License
+
+Copyright (c) 2022, Lucas Nestler
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

### Comparing `tpucare-0.4.0/PKG-INFO` & `tpucare-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.0
+Version: 0.4.1
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
@@ -199,8 +198,7 @@
   month        = jul,
   year         = 2022,
   publisher    = {Zenodo},
   version      = {0.0.2},
   doi          = {10.5281/zenodo.6837312},
   url          = {https://doi.org/10.5281/zenodo.6837312}
 }```
-
```

### Comparing `tpucare-0.4.0/README.md` & `tpucare-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,485 +1,474 @@
-00000000: 2320 5450 5520 4361 7265 0d0a 0d0a 4175  # TPU Care....Au
-00000010: 746f 6d61 7469 6361 6c6c 7920 7461 6b65  tomatically take
-00000020: 2067 6f6f 6420 6361 7265 206f 6620 796f   good care of yo
-00000030: 7572 2070 7265 656d 7074 6962 6c65 2054  ur preemptible T
-00000040: 5055 730d 0a0d 0a23 2320 5461 626c 6520  PUs....## Table 
-00000050: 6f66 2043 6f6e 7465 6e74 730d 0a0d 0a2a  of Contents....*
-00000060: 205b 5450 5520 4361 7265 5d28 2374 7075   [TPU Care](#tpu
-00000070: 2d63 6172 6529 0d0a 2020 2020 2a20 5b54  -care)..    * [T
-00000080: 6162 6c65 206f 6620 436f 6e74 656e 7473  able of Contents
-00000090: 5d28 2374 6162 6c65 2d6f 662d 636f 6e74  ](#table-of-cont
-000000a0: 656e 7473 290d 0a20 2020 202a 205b 4665  ents)..    * [Fe
-000000b0: 6174 7572 6573 5d28 2366 6561 7475 7265  atures](#feature
-000000c0: 7329 0d0a 2020 2020 2a20 5b47 6574 7469  s)..    * [Getti
-000000d0: 6e67 2053 7461 7274 6564 5d28 2367 6574  ng Started](#get
-000000e0: 7469 6e67 2d73 7461 7274 6564 290d 0a20  ting-started).. 
-000000f0: 2020 2020 2020 202a 205b 496e 7374 616c         * [Instal
-00000100: 6c61 7469 6f6e 5d28 2369 6e73 7461 6c6c  lation](#install
-00000110: 6174 696f 6e29 0d0a 2020 2020 2a20 5b45  ation)..    * [E
-00000120: 7861 6d70 6c65 735d 2823 6578 616d 706c  xamples](#exampl
-00000130: 6573 290d 0a20 2020 2020 2020 202a 205b  es)..        * [
-00000140: 4c6f 6e67 2d72 756e 6e69 6e67 2070 7265  Long-running pre
-00000150: 656d 7074 6962 6c65 2074 7261 696e 696e  emptible trainin
-00000160: 675d 2823 6c6f 6e67 2d72 756e 6e69 6e67  g](#long-running
-00000170: 2d70 7265 656d 7074 6962 6c65 2d74 7261  -preemptible-tra
-00000180: 696e 696e 6729 0d0a 2020 2020 2020 2020  ining)..        
-00000190: 2a20 5b53 7765 6570 735d 2823 7377 6565  * [Sweeps](#swee
-000001a0: 7073 290d 0a20 2020 202a 205b 4369 7461  ps)..    * [Cita
-000001b0: 7469 6f6e 5d28 2363 6974 6174 696f 6e29  tion](#citation)
-000001c0: 0d0a 0d0a 2323 2046 6561 7475 7265 730d  ....## Features.
-000001d0: 0a0d 0a2a 202a 2a52 656c 6961 626c 6520  ...* **Reliable 
-000001e0: 636f 6465 2065 7865 6375 7469 6f6e 2a2a  code execution**
-000001f0: 3a20 5450 5520 4361 7265 2073 7461 7274  : TPU Care start
-00000200: 7320 6120 5450 552c 2065 6e73 7572 6573  s a TPU, ensures
-00000210: 2069 7427 7320 7365 7420 7570 2061 7320   it's set up as 
-00000220: 7370 6563 6966 6965 6420 616e 6420 636f  specified and co
-00000230: 6e74 696e 7565 7320 7468 6520 6578 7065  ntinues the expe
-00000240: 7269 6d65 6e74 0d0a 2020 7768 656e 6576  riment..  whenev
-00000250: 6572 2074 6865 206e 6f64 6520 6469 6573  er the node dies
-00000260: 2e20 5468 696e 6b20 6f66 2069 7420 6c69  . Think of it li
-00000270: 6b65 205b 5465 7272 6146 6f72 6d5d 2868  ke [TerraForm](h
-00000280: 7474 7073 3a2f 2f77 7777 2e74 6572 7261  ttps://www.terra
-00000290: 666f 726d 2e69 6f2f 2920 2b20 5b41 6e73  form.io/) + [Ans
-000002a0: 6962 6c65 5d28 6874 7470 733a 2f2f 7777  ible](https://ww
-000002b0: 772e 616e 7369 626c 652e 636f 6d2f 290d  w.ansible.com/).
-000002c0: 0a20 2066 6f72 206d 6163 6869 6e65 206c  .  for machine l
-000002d0: 6561 726e 696e 672e 0d0a 2a20 2a2a 4d61  earning...* **Ma
-000002e0: 696e 7465 6e61 6e63 6520 6f66 206c 6172  intenance of lar
-000002f0: 6765 2073 7761 726d 732a 2a3a 2057 6865  ge swarms**: Whe
-00000300: 6e20 7275 6e6e 696e 6720 6d75 6c74 6970  n running multip
-00000310: 6c65 206e 6f64 6573 2c20 5450 5520 4361  le nodes, TPU Ca
-00000320: 7265 2077 696c 6c20 6175 746f 6d61 7469  re will automati
-00000330: 6361 6c6c 7920 6465 6c65 7465 2064 6561  cally delete dea
-00000340: 6420 696e 7374 616e 6365 7320 7768 696c  d instances whil
-00000350: 650d 0a20 206b 6565 7069 6e67 2061 7320  e..  keeping as 
-00000360: 6d61 6e79 2061 6c69 7665 2061 7320 706f  many alive as po
-00000370: 7373 6962 6c65 2e0d 0a2a 202a 2a43 6f64  ssible...* **Cod
-00000380: 6520 6765 6e65 7261 7469 6f6e 2a2a 3a20  e generation**: 
-00000390: 546f 2073 696d 706c 6966 7920 7365 7475  To simplify setu
-000003a0: 702c 2054 5055 2043 6172 6520 6566 6669  p, TPU Care effi
-000003b0: 6369 656e 746c 7920 636c 6f6e 6573 2079  ciently clones y
-000003c0: 6f75 7220 6769 7420 7265 706f 7369 746f  our git reposito
-000003d0: 7279 2061 6e64 2065 6e73 7572 6573 2074  ry and ensures t
-000003e0: 7275 7374 6162 6c65 0d0a 2020 6578 6563  rustable..  exec
-000003f0: 7574 696f 6e20 6f66 2079 6f75 7220 6072  ution of your `r
-00000400: 756e 5f63 6f6d 6d61 6e64 6020 7468 6174  un_command` that
-00000410: 2063 6f6e 7469 6e75 6573 2065 7665 6e20   continues even 
-00000420: 6475 7269 6e67 206f 7574 6167 6573 2e0d  during outages..
-00000430: 0a2a 202a 2a4f 7074 696d 697a 6564 206d  .* **Optimized m
-00000440: 616e 6167 656d 656e 742a 2a3a 2057 6865  anagement**: Whe
-00000450: 6e20 6120 6e6f 6465 2064 6965 732c 2054  n a node dies, T
-00000460: 5055 2043 6172 6520 6465 6c65 7465 7320  PU Care deletes 
-00000470: 6974 2077 6974 6869 6e20 6669 7665 206d  it within five m
-00000480: 696e 7574 6573 2061 6e64 2063 7265 6174  inutes and creat
-00000490: 6573 2061 206e 6577 206f 6e65 2074 6865  es a new one the
-000004a0: 2073 6563 6f6e 640d 0a20 2074 6865 7265   second..  there
-000004b0: 2069 7320 6361 7061 6369 7479 2e0d 0a0d   is capacity....
-000004c0: 0a23 2320 4765 7474 696e 6720 5374 6172  .## Getting Star
-000004d0: 7465 640d 0a0d 0a23 2323 2049 6e73 7461  ted....### Insta
-000004e0: 6c6c 6174 696f 6e0d 0a0d 0a60 6060 4241  llation....```BA
-000004f0: 5348 0d0a 7079 7468 6f6e 3320 2d6d 2070  SH..python3 -m p
-00000500: 6970 2069 6e73 7461 6c6c 2074 7075 6361  ip install tpuca
-00000510: 7265 0d0a 6060 600d 0a0d 0a23 2320 4578  re..```....## Ex
-00000520: 616d 706c 6573 0d0a 0d0a 5765 2776 6520  amples....We've 
-00000530: 6265 656e 2075 7369 6e67 2054 5055 2043  been using TPU C
-00000540: 6172 6520 666f 7220 6120 7768 696c 6520  are for a while 
-00000550: 6174 205b 486f 6d65 6272 6577 4e4c 505d  at [HomebrewNLP]
-00000560: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000570: 636f 6d2f 486f 6d65 6272 6577 4e4c 502f  com/HomebrewNLP/
-00000580: 292e 2049 6e20 6661 6374 2c20 7468 6973  ). In fact, this
-00000590: 206c 6962 7261 7279 2069 7320 6a75 7374   library is just
-000005a0: 0d0a 7468 6520 6272 616e 6368 6564 206f  ..the branched o
-000005b0: 7574 2063 6f72 6520 6f66 2074 6865 206f  ut core of the o
-000005c0: 7269 6769 6e61 6c20 7072 6f64 7563 7469  riginal producti
-000005d0: 6f6e 2d72 6561 6479 2048 6f6d 6562 7265  on-ready Homebre
-000005e0: 774e 4c50 2063 6f64 652e 2041 7420 486f  wNLP code. At Ho
-000005f0: 6d65 6272 6577 4e4c 502c 2074 6865 7265  mebrewNLP, there
-00000600: 2077 6572 6520 7477 6f20 6d61 6a6f 7220   were two major 
-00000610: 7573 652d 6361 7365 730d 0a66 6f72 2074  use-cases..for t
-00000620: 6869 7320 6c69 6272 6172 792e 2057 6520  his library. We 
-00000630: 7374 6172 7465 6420 626f 7468 206d 6173  started both mas
-00000640: 7369 7665 2068 7970 6572 7061 7261 6d65  sive hyperparame
-00000650: 7465 7220 7377 6565 7073 2077 6869 6368  ter sweeps which
-00000660: 2063 6f6e 7375 6d65 6420 3930 302c 3030   consumed 900,00
-00000670: 3020 5450 552d 636f 7265 2068 6f75 7273  0 TPU-core hours
-00000680: 2077 6974 6869 6e20 7468 7265 650d 0a6d   within three..m
-00000690: 6f6e 7468 7320 616e 6420 7374 6162 6c65  onths and stable
-000006a0: 2074 7261 696e 696e 6720 6f6e 206c 6172   training on lar
-000006b0: 6765 2054 5055 2070 6f64 732e 2042 656c  ge TPU pods. Bel
-000006c0: 6f77 2c20 796f 7520 6361 6e20 7365 6520  ow, you can see 
-000006d0: 6120 6c69 7374 206f 6620 5450 5573 2077  a list of TPUs w
-000006e0: 6869 6368 2061 7265 206c 6172 6765 6c79  hich are largely
-000006f0: 206d 616e 6167 6564 2062 7920 5450 550d   managed by TPU.
-00000700: 0a43 6172 653a 2021 5b50 5520 4f75 7470  .Care: ![PU Outp
-00000710: 7574 5d28 6874 7470 733a 2f2f 692e 696d  ut](https://i.im
-00000720: 6775 722e 636f 6d2f 4c63 4f6d 3042 632e  gur.com/LcOm0Bc.
-00000730: 706e 6729 0d0a 3c70 2061 6c69 676e 3d22  png)..<p align="
-00000740: 6365 6e74 6572 223e 5363 7265 656e 7368  center">Screensh
-00000750: 6f74 2066 726f 6d20 3c61 2068 7265 663d  ot from <a href=
-00000760: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000770: 636f 6d2f 7368 6177 776e 2f74 7075 6e69  com/shawwn/tpuni
-00000780: 636f 726e 223e 5450 556e 6963 6f72 6e3c  corn">TPUnicorn<
-00000790: 2f61 3e2c 2061 2043 4c49 2d62 6173 6564  /a>, a CLI-based
-000007a0: 2054 5055 206d 616e 6167 6564 2073 6f66   TPU managed sof
-000007b0: 7477 6172 653c 2f70 3e0d 0a49 6e20 7468  tware</p>..In th
-000007c0: 6520 666f 6c6c 6f77 696e 6720 7365 6374  e following sect
-000007d0: 696f 6e73 2c20 796f 7527 6c6c 206c 6561  ions, you'll lea
-000007e0: 726e 2068 6f77 2077 6520 7573 6520 6174  rn how we use at
-000007f0: 206d 6173 7369 7665 2073 6361 6c65 2077   massive scale w
-00000800: 6974 6820 6d69 6e69 6d61 6c20 636f 6465  ith minimal code
-00000810: 2065 6666 6f72 742e 0d0a 0d0a 2323 2320   effort.....### 
-00000820: 4c6f 6e67 2d72 756e 6e69 6e67 2070 7265  Long-running pre
-00000830: 656d 7074 6962 6c65 2074 7261 696e 696e  emptible trainin
-00000840: 670d 0a0d 0a46 6f72 2065 7861 6d70 6c65  g....For example
-00000850: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
-00000860: 636f 6465 2063 616e 2062 6520 7573 6564  code can be used
-00000870: 2074 6f20 6372 6561 7465 2061 2070 726f   to create a pro
-00000880: 6475 6374 696f 6e2d 7265 6164 7920 7633  duction-ready v3
-00000890: 2d32 3536 2075 7369 6e67 0d0a 7468 6520  -256 using..the 
-000008a0: 5b48 6f6d 6562 7265 774e 4c50 2d4a 6178  [HomebrewNLP-Jax
-000008b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000008c0: 2e63 6f6d 2f48 6f6d 6562 7265 774e 4c50  .com/HomebrewNLP
-000008d0: 2f48 6f6d 6562 7265 774e 4c50 2d4a 6178  /HomebrewNLP-Jax
-000008e0: 2920 636f 6465 6261 7365 2028 0d0a 7365  ) codebase (..se
-000008f0: 6520 5b65 7861 6d70 6c65 732f 706f 642e  e [examples/pod.
-00000900: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-00000910: 7562 2e63 6f6d 2f63 6c61 7368 6c75 6b65  ub.com/clashluke
-00000920: 2f74 7075 6361 7265 2f62 6c6f 622f 6d61  /tpucare/blob/ma
-00000930: 696e 2f65 7861 6d70 6c65 732f 706f 642e  in/examples/pod.
-00000940: 7079 2920 666f 7220 616e 2065 7865 6375  py) for an execu
-00000950: 7461 626c 6520 7665 7273 696f 6e29 3a0d  table version):.
-00000960: 0a0d 0a60 6060 5059 5448 4f4e 0d0a 696d  ...```PYTHON..im
-00000970: 706f 7274 2064 6174 6163 6c61 7373 6573  port dataclasses
-00000980: 0d0a 696d 706f 7274 2074 7970 696e 670d  ..import typing.
-00000990: 0a66 726f 6d20 6e65 7472 6320 696d 706f  .from netrc impo
-000009a0: 7274 206e 6574 7263 0d0a 0d0a 696d 706f  rt netrc....impo
-000009b0: 7274 2079 616d 6c0d 0a0d 0a66 726f 6d20  rt yaml....from 
-000009c0: 7470 7563 6172 6520 696d 706f 7274 2065  tpucare import e
-000009d0: 7865 635f 636f 6d6d 616e 642c 2065 7865  xec_command, exe
-000009e0: 635f 6f6e 5f74 7075 2c20 7365 6e64 5f74  c_on_tpu, send_t
-000009f0: 6f5f 7470 752c 2073 7461 7274 5f73 696e  o_tpu, start_sin
-00000a00: 676c 650d 0a0d 0a0d 0a40 6461 7461 636c  gle......@datacl
-00000a10: 6173 7365 732e 6461 7461 636c 6173 730d  asses.dataclass.
-00000a20: 0a63 6c61 7373 2043 6f6e 7465 7874 3a0d  .class Context:.
-00000a30: 0a20 2020 2072 6574 7279 3a20 696e 740d  .    retry: int.
-00000a40: 0a0d 0a0d 0a5a 4f4e 4520 3d20 2265 7572  .....ZONE = "eur
-00000a50: 6f70 652d 7765 7374 342d 6122 0d0a 484f  ope-west4-a"..HO
-00000a60: 5354 203d 2022 6269 672d 706f 6422 0d0a  ST = "big-pod"..
-00000a70: 5255 4e5f 4e41 4d45 203d 2022 3235 362d  RUN_NAME = "256-
-00000a80: 636f 7265 2d74 7075 220d 0a0d 0a0d 0a64  core-tpu"......d
-00000a90: 6566 206c 6f61 645f 636f 6e66 6967 2863  ef load_config(c
-00000aa0: 7478 3a20 436f 6e74 6578 7429 3a0d 0a20  tx: Context):.. 
-00000ab0: 2020 2077 6974 6820 6f70 656e 2822 636f     with open("co
-00000ac0: 6e66 6967 2e79 616d 6c22 2c20 2772 2729  nfig.yaml", 'r')
-00000ad0: 2061 7320 663a 0d0a 2020 2020 2020 2020   as f:..        
-00000ae0: 636f 6e66 6967 203d 2066 2e72 6561 6428  config = f.read(
-00000af0: 290d 0a20 2020 2063 6f6e 6669 6720 3d20  )..    config = 
-00000b00: 7961 6d6c 2e73 6166 655f 6c6f 6164 2863  yaml.safe_load(c
-00000b10: 6f6e 6669 6729 0d0a 0d0a 2020 2020 7761  onfig)....    wa
-00000b20: 6e64 625f 6170 6920 3d20 7761 6e64 622e  ndb_api = wandb.
-00000b30: 4170 6928 290d 0a20 2020 2063 6f6e 6669  Api()..    confi
-00000b40: 675b 2274 7261 696e 696e 6722 5d5b 2264  g["training"]["d
-00000b50: 6f5f 6368 6563 6b70 6f69 6e74 225d 203d  o_checkpoint"] =
-00000b60: 2054 7275 650d 0a20 2020 2062 6173 655f   True..    base_
-00000b70: 6368 6563 6b70 6f69 6e74 5f70 6174 6820  checkpoint_path 
-00000b80: 3d20 636f 6e66 6967 5b22 7472 6169 6e69  = config["traini
-00000b90: 6e67 225d 5b22 6368 6563 6b70 6f69 6e74  ng"]["checkpoint
-00000ba0: 5f70 6174 6822 5d0d 0a0d 0a20 2020 2073  _path"]....    s
-00000bb0: 7461 7274 5f73 7465 7020 3d20 300d 0a20  tart_step = 0.. 
-00000bc0: 2020 2066 6f72 2072 756e 2069 6e20 7761     for run in wa
-00000bd0: 6e64 625f 6170 692e 7275 6e73 2866 227b  ndb_api.runs(f"{
+00000000: 2320 5450 5520 4361 7265 0a0a 4175 746f  # TPU Care..Auto
+00000010: 6d61 7469 6361 6c6c 7920 7461 6b65 2067  matically take g
+00000020: 6f6f 6420 6361 7265 206f 6620 796f 7572  ood care of your
+00000030: 2070 7265 656d 7074 6962 6c65 2054 5055   preemptible TPU
+00000040: 730a 0a23 2320 5461 626c 6520 6f66 2043  s..## Table of C
+00000050: 6f6e 7465 6e74 730a 0a2a 205b 5450 5520  ontents..* [TPU 
+00000060: 4361 7265 5d28 2374 7075 2d63 6172 6529  Care](#tpu-care)
+00000070: 0a20 2020 202a 205b 5461 626c 6520 6f66  .    * [Table of
+00000080: 2043 6f6e 7465 6e74 735d 2823 7461 626c   Contents](#tabl
+00000090: 652d 6f66 2d63 6f6e 7465 6e74 7329 0a20  e-of-contents). 
+000000a0: 2020 202a 205b 4665 6174 7572 6573 5d28     * [Features](
+000000b0: 2366 6561 7475 7265 7329 0a20 2020 202a  #features).    *
+000000c0: 205b 4765 7474 696e 6720 5374 6172 7465   [Getting Starte
+000000d0: 645d 2823 6765 7474 696e 672d 7374 6172  d](#getting-star
+000000e0: 7465 6429 0a20 2020 2020 2020 202a 205b  ted).        * [
+000000f0: 496e 7374 616c 6c61 7469 6f6e 5d28 2369  Installation](#i
+00000100: 6e73 7461 6c6c 6174 696f 6e29 0a20 2020  nstallation).   
+00000110: 202a 205b 4578 616d 706c 6573 5d28 2365   * [Examples](#e
+00000120: 7861 6d70 6c65 7329 0a20 2020 2020 2020  xamples).       
+00000130: 202a 205b 4c6f 6e67 2d72 756e 6e69 6e67   * [Long-running
+00000140: 2070 7265 656d 7074 6962 6c65 2074 7261   preemptible tra
+00000150: 696e 696e 675d 2823 6c6f 6e67 2d72 756e  ining](#long-run
+00000160: 6e69 6e67 2d70 7265 656d 7074 6962 6c65  ning-preemptible
+00000170: 2d74 7261 696e 696e 6729 0a20 2020 2020  -training).     
+00000180: 2020 202a 205b 5377 6565 7073 5d28 2373     * [Sweeps](#s
+00000190: 7765 6570 7329 0a20 2020 202a 205b 4369  weeps).    * [Ci
+000001a0: 7461 7469 6f6e 5d28 2363 6974 6174 696f  tation](#citatio
+000001b0: 6e29 0a0a 2323 2046 6561 7475 7265 730a  n)..## Features.
+000001c0: 0a2a 202a 2a52 656c 6961 626c 6520 636f  .* **Reliable co
+000001d0: 6465 2065 7865 6375 7469 6f6e 2a2a 3a20  de execution**: 
+000001e0: 5450 5520 4361 7265 2073 7461 7274 7320  TPU Care starts 
+000001f0: 6120 5450 552c 2065 6e73 7572 6573 2069  a TPU, ensures i
+00000200: 7427 7320 7365 7420 7570 2061 7320 7370  t's set up as sp
+00000210: 6563 6966 6965 6420 616e 6420 636f 6e74  ecified and cont
+00000220: 696e 7565 7320 7468 6520 6578 7065 7269  inues the experi
+00000230: 6d65 6e74 0a20 2077 6865 6e65 7665 7220  ment.  whenever 
+00000240: 7468 6520 6e6f 6465 2064 6965 732e 2054  the node dies. T
+00000250: 6869 6e6b 206f 6620 6974 206c 696b 6520  hink of it like 
+00000260: 5b54 6572 7261 466f 726d 5d28 6874 7470  [TerraForm](http
+00000270: 733a 2f2f 7777 772e 7465 7272 6166 6f72  s://www.terrafor
+00000280: 6d2e 696f 2f29 202b 205b 416e 7369 626c  m.io/) + [Ansibl
+00000290: 655d 2868 7474 7073 3a2f 2f77 7777 2e61  e](https://www.a
+000002a0: 6e73 6962 6c65 2e63 6f6d 2f29 0a20 2066  nsible.com/).  f
+000002b0: 6f72 206d 6163 6869 6e65 206c 6561 726e  or machine learn
+000002c0: 696e 672e 0a2a 202a 2a4d 6169 6e74 656e  ing..* **Mainten
+000002d0: 616e 6365 206f 6620 6c61 7267 6520 7377  ance of large sw
+000002e0: 6172 6d73 2a2a 3a20 5768 656e 2072 756e  arms**: When run
+000002f0: 6e69 6e67 206d 756c 7469 706c 6520 6e6f  ning multiple no
+00000300: 6465 732c 2054 5055 2043 6172 6520 7769  des, TPU Care wi
+00000310: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+00000320: 2064 656c 6574 6520 6465 6164 2069 6e73   delete dead ins
+00000330: 7461 6e63 6573 2077 6869 6c65 0a20 206b  tances while.  k
+00000340: 6565 7069 6e67 2061 7320 6d61 6e79 2061  eeping as many a
+00000350: 6c69 7665 2061 7320 706f 7373 6962 6c65  live as possible
+00000360: 2e0a 2a20 2a2a 436f 6465 2067 656e 6572  ..* **Code gener
+00000370: 6174 696f 6e2a 2a3a 2054 6f20 7369 6d70  ation**: To simp
+00000380: 6c69 6679 2073 6574 7570 2c20 5450 5520  lify setup, TPU 
+00000390: 4361 7265 2065 6666 6963 6965 6e74 6c79  Care efficiently
+000003a0: 2063 6c6f 6e65 7320 796f 7572 2067 6974   clones your git
+000003b0: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
+000003c0: 656e 7375 7265 7320 7472 7573 7461 626c  ensures trustabl
+000003d0: 650a 2020 6578 6563 7574 696f 6e20 6f66  e.  execution of
+000003e0: 2079 6f75 7220 6072 756e 5f63 6f6d 6d61   your `run_comma
+000003f0: 6e64 6020 7468 6174 2063 6f6e 7469 6e75  nd` that continu
+00000400: 6573 2065 7665 6e20 6475 7269 6e67 206f  es even during o
+00000410: 7574 6167 6573 2e0a 2a20 2a2a 4f70 7469  utages..* **Opti
+00000420: 6d69 7a65 6420 6d61 6e61 6765 6d65 6e74  mized management
+00000430: 2a2a 3a20 5768 656e 2061 206e 6f64 6520  **: When a node 
+00000440: 6469 6573 2c20 5450 5520 4361 7265 2064  dies, TPU Care d
+00000450: 656c 6574 6573 2069 7420 7769 7468 696e  eletes it within
+00000460: 2066 6976 6520 6d69 6e75 7465 7320 616e   five minutes an
+00000470: 6420 6372 6561 7465 7320 6120 6e65 7720  d creates a new 
+00000480: 6f6e 6520 7468 6520 7365 636f 6e64 0a20  one the second. 
+00000490: 2074 6865 7265 2069 7320 6361 7061 6369   there is capaci
+000004a0: 7479 2e0a 0a23 2320 4765 7474 696e 6720  ty...## Getting 
+000004b0: 5374 6172 7465 640a 0a23 2323 2049 6e73  Started..### Ins
+000004c0: 7461 6c6c 6174 696f 6e0a 0a60 6060 4241  tallation..```BA
+000004d0: 5348 0a70 7974 686f 6e33 202d 6d20 7069  SH.python3 -m pi
+000004e0: 7020 696e 7374 616c 6c20 7470 7563 6172  p install tpucar
+000004f0: 650a 6060 600a 0a23 2320 4578 616d 706c  e.```..## Exampl
+00000500: 6573 0a0a 5765 2776 6520 6265 656e 2075  es..We've been u
+00000510: 7369 6e67 2054 5055 2043 6172 6520 666f  sing TPU Care fo
+00000520: 7220 6120 7768 696c 6520 6174 205b 486f  r a while at [Ho
+00000530: 6d65 6272 6577 4e4c 505d 2868 7474 7073  mebrewNLP](https
+00000540: 3a2f 2f67 6974 6875 622e 636f 6d2f 486f  ://github.com/Ho
+00000550: 6d65 6272 6577 4e4c 502f 292e 2049 6e20  mebrewNLP/). In 
+00000560: 6661 6374 2c20 7468 6973 206c 6962 7261  fact, this libra
+00000570: 7279 2069 7320 6a75 7374 0a74 6865 2062  ry is just.the b
+00000580: 7261 6e63 6865 6420 6f75 7420 636f 7265  ranched out core
+00000590: 206f 6620 7468 6520 6f72 6967 696e 616c   of the original
+000005a0: 2070 726f 6475 6374 696f 6e2d 7265 6164   production-read
+000005b0: 7920 486f 6d65 6272 6577 4e4c 5020 636f  y HomebrewNLP co
+000005c0: 6465 2e20 4174 2048 6f6d 6562 7265 774e  de. At HomebrewN
+000005d0: 4c50 2c20 7468 6572 6520 7765 7265 2074  LP, there were t
+000005e0: 776f 206d 616a 6f72 2075 7365 2d63 6173  wo major use-cas
+000005f0: 6573 0a66 6f72 2074 6869 7320 6c69 6272  es.for this libr
+00000600: 6172 792e 2057 6520 7374 6172 7465 6420  ary. We started 
+00000610: 626f 7468 206d 6173 7369 7665 2068 7970  both massive hyp
+00000620: 6572 7061 7261 6d65 7465 7220 7377 6565  erparameter swee
+00000630: 7073 2077 6869 6368 2063 6f6e 7375 6d65  ps which consume
+00000640: 6420 3930 302c 3030 3020 5450 552d 636f  d 900,000 TPU-co
+00000650: 7265 2068 6f75 7273 2077 6974 6869 6e20  re hours within 
+00000660: 7468 7265 650a 6d6f 6e74 6873 2061 6e64  three.months and
+00000670: 2073 7461 626c 6520 7472 6169 6e69 6e67   stable training
+00000680: 206f 6e20 6c61 7267 6520 5450 5520 706f   on large TPU po
+00000690: 6473 2e20 4265 6c6f 772c 2079 6f75 2063  ds. Below, you c
+000006a0: 616e 2073 6565 2061 206c 6973 7420 6f66  an see a list of
+000006b0: 2054 5055 7320 7768 6963 6820 6172 6520   TPUs which are 
+000006c0: 6c61 7267 656c 7920 6d61 6e61 6765 6420  largely managed 
+000006d0: 6279 2054 5055 0a43 6172 653a 2021 5b50  by TPU.Care: ![P
+000006e0: 5520 4f75 7470 7574 5d28 6874 7470 733a  U Output](https:
+000006f0: 2f2f 692e 696d 6775 722e 636f 6d2f 4c63  //i.imgur.com/Lc
+00000700: 4f6d 3042 632e 706e 6729 0a3c 7020 616c  Om0Bc.png).<p al
+00000710: 6967 6e3d 2263 656e 7465 7222 3e53 6372  ign="center">Scr
+00000720: 6565 6e73 686f 7420 6672 6f6d 203c 6120  eenshot from <a 
+00000730: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000740: 7468 7562 2e63 6f6d 2f73 6861 7777 6e2f  thub.com/shawwn/
+00000750: 7470 756e 6963 6f72 6e22 3e54 5055 6e69  tpunicorn">TPUni
+00000760: 636f 726e 3c2f 613e 2c20 6120 434c 492d  corn</a>, a CLI-
+00000770: 6261 7365 6420 5450 5520 6d61 6e61 6765  based TPU manage
+00000780: 6420 736f 6674 7761 7265 3c2f 703e 0a49  d software</p>.I
+00000790: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+000007a0: 7365 6374 696f 6e73 2c20 796f 7527 6c6c  sections, you'll
+000007b0: 206c 6561 726e 2068 6f77 2077 6520 7573   learn how we us
+000007c0: 6520 6174 206d 6173 7369 7665 2073 6361  e at massive sca
+000007d0: 6c65 2077 6974 6820 6d69 6e69 6d61 6c20  le with minimal 
+000007e0: 636f 6465 2065 6666 6f72 742e 0a0a 2323  code effort...##
+000007f0: 2320 4c6f 6e67 2d72 756e 6e69 6e67 2070  # Long-running p
+00000800: 7265 656d 7074 6962 6c65 2074 7261 696e  reemptible train
+00000810: 696e 670a 0a46 6f72 2065 7861 6d70 6c65  ing..For example
+00000820: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
+00000830: 636f 6465 2063 616e 2062 6520 7573 6564  code can be used
+00000840: 2074 6f20 6372 6561 7465 2061 2070 726f   to create a pro
+00000850: 6475 6374 696f 6e2d 7265 6164 7920 7633  duction-ready v3
+00000860: 2d32 3536 2075 7369 6e67 0a74 6865 205b  -256 using.the [
+00000870: 486f 6d65 6272 6577 4e4c 502d 4a61 785d  HomebrewNLP-Jax]
+00000880: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000890: 636f 6d2f 486f 6d65 6272 6577 4e4c 502f  com/HomebrewNLP/
+000008a0: 486f 6d65 6272 6577 4e4c 502d 4a61 7829  HomebrewNLP-Jax)
+000008b0: 2063 6f64 6562 6173 6520 280a 7365 6520   codebase (.see 
+000008c0: 5b65 7861 6d70 6c65 732f 706f 642e 7079  [examples/pod.py
+000008d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008e0: 2e63 6f6d 2f63 6c61 7368 6c75 6b65 2f74  .com/clashluke/t
+000008f0: 7075 6361 7265 2f62 6c6f 622f 6d61 696e  pucare/blob/main
+00000900: 2f65 7861 6d70 6c65 732f 706f 642e 7079  /examples/pod.py
+00000910: 2920 666f 7220 616e 2065 7865 6375 7461  ) for an executa
+00000920: 626c 6520 7665 7273 696f 6e29 3a0a 0a60  ble version):..`
+00000930: 6060 5059 5448 4f4e 0a69 6d70 6f72 7420  ``PYTHON.import 
+00000940: 6461 7461 636c 6173 7365 730a 696d 706f  dataclasses.impo
+00000950: 7274 2074 7970 696e 670a 6672 6f6d 206e  rt typing.from n
+00000960: 6574 7263 2069 6d70 6f72 7420 6e65 7472  etrc import netr
+00000970: 630a 0a69 6d70 6f72 7420 7961 6d6c 0a0a  c..import yaml..
+00000980: 6672 6f6d 2074 7075 6361 7265 2069 6d70  from tpucare imp
+00000990: 6f72 7420 6578 6563 5f63 6f6d 6d61 6e64  ort exec_command
+000009a0: 2c20 6578 6563 5f6f 6e5f 7470 752c 2073  , exec_on_tpu, s
+000009b0: 656e 645f 746f 5f74 7075 2c20 7374 6172  end_to_tpu, star
+000009c0: 745f 7369 6e67 6c65 0a0a 0a40 6461 7461  t_single...@data
+000009d0: 636c 6173 7365 732e 6461 7461 636c 6173  classes.dataclas
+000009e0: 730a 636c 6173 7320 436f 6e74 6578 743a  s.class Context:
+000009f0: 0a20 2020 2072 6574 7279 3a20 696e 740a  .    retry: int.
+00000a00: 0a0a 5a4f 4e45 203d 2022 6575 726f 7065  ..ZONE = "europe
+00000a10: 2d77 6573 7434 2d61 220a 484f 5354 203d  -west4-a".HOST =
+00000a20: 2022 6269 672d 706f 6422 0a52 554e 5f4e   "big-pod".RUN_N
+00000a30: 414d 4520 3d20 2232 3536 2d63 6f72 652d  AME = "256-core-
+00000a40: 7470 7522 0a0a 0a64 6566 206c 6f61 645f  tpu"...def load_
+00000a50: 636f 6e66 6967 2863 7478 3a20 436f 6e74  config(ctx: Cont
+00000a60: 6578 7429 3a0a 2020 2020 7769 7468 206f  ext):.    with o
+00000a70: 7065 6e28 2263 6f6e 6669 672e 7961 6d6c  pen("config.yaml
+00000a80: 222c 2027 7227 2920 6173 2066 3a0a 2020  ", 'r') as f:.  
+00000a90: 2020 2020 2020 636f 6e66 6967 203d 2066        config = f
+00000aa0: 2e72 6561 6428 290a 2020 2020 636f 6e66  .read().    conf
+00000ab0: 6967 203d 2079 616d 6c2e 7361 6665 5f6c  ig = yaml.safe_l
+00000ac0: 6f61 6428 636f 6e66 6967 290a 0a20 2020  oad(config)..   
+00000ad0: 2077 616e 6462 5f61 7069 203d 2077 616e   wandb_api = wan
+00000ae0: 6462 2e41 7069 2829 0a20 2020 2063 6f6e  db.Api().    con
+00000af0: 6669 675b 2274 7261 696e 696e 6722 5d5b  fig["training"][
+00000b00: 2264 6f5f 6368 6563 6b70 6f69 6e74 225d  "do_checkpoint"]
+00000b10: 203d 2054 7275 650a 2020 2020 6261 7365   = True.    base
+00000b20: 5f63 6865 636b 706f 696e 745f 7061 7468  _checkpoint_path
+00000b30: 203d 2063 6f6e 6669 675b 2274 7261 696e   = config["train
+00000b40: 696e 6722 5d5b 2263 6865 636b 706f 696e  ing"]["checkpoin
+00000b50: 745f 7061 7468 225d 0a0a 2020 2020 7374  t_path"]..    st
+00000b60: 6172 745f 7374 6570 203d 2030 0a20 2020  art_step = 0.   
+00000b70: 2066 6f72 2072 756e 2069 6e20 7761 6e64   for run in wand
+00000b80: 625f 6170 692e 7275 6e73 2866 227b 636f  b_api.runs(f"{co
+00000b90: 6e66 6967 5b27 7761 6e64 6227 5d5b 2765  nfig['wandb']['e
+00000ba0: 6e74 6974 7927 5d7d 2f7b 636f 6e66 6967  ntity']}/{config
+00000bb0: 5b27 7761 6e64 6227 5d5b 2770 726f 6a65  ['wandb']['proje
+00000bc0: 6374 275d 7d22 293a 0a20 2020 2020 2020  ct']}"):.       
+00000bd0: 2069 6620 7275 6e2e 6e61 6d65 203d 3d20   if run.name == 
 00000be0: 636f 6e66 6967 5b27 7761 6e64 6227 5d5b  config['wandb'][
-00000bf0: 2765 6e74 6974 7927 5d7d 2f7b 636f 6e66  'entity']}/{conf
-00000c00: 6967 5b27 7761 6e64 6227 5d5b 2770 726f  ig['wandb']['pro
-00000c10: 6a65 6374 275d 7d22 293a 0d0a 2020 2020  ject']}"):..    
-00000c20: 2020 2020 6966 2072 756e 2e6e 616d 6520      if run.name 
-00000c30: 3d3d 2063 6f6e 6669 675b 2777 616e 6462  == config['wandb
-00000c40: 275d 5b27 6e61 6d65 275d 3a0d 0a20 2020  ']['name']:..   
-00000c50: 2020 2020 2020 2020 2073 7461 7274 5f73           start_s
-00000c60: 7465 7020 3d20 7275 6e2e 7375 6d6d 6172  tep = run.summar
-00000c70: 795b 225f 7374 6570 225d 0d0a 2020 2020  y["_step"]..    
-00000c80: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
-00000c90: 2020 2073 7461 7274 5f73 7465 7020 2d3d     start_step -=
-00000ca0: 2073 7461 7274 5f73 7465 7020 2520 636f   start_step % co
-00000cb0: 6e66 6967 5b22 7472 6169 6e69 6e67 225d  nfig["training"]
-00000cc0: 5b22 6368 6563 6b70 6f69 6e74 5f69 6e74  ["checkpoint_int
-00000cd0: 6572 7661 6c22 5d0d 0a0d 0a20 2020 2063  erval"]....    c
-00000ce0: 6f6e 6669 675b 2274 7261 696e 696e 6722  onfig["training"
-00000cf0: 5d5b 2273 7461 7274 5f73 7465 7022 5d20  ]["start_step"] 
-00000d00: 3d20 7374 6172 745f 7374 6570 0d0a 2020  = start_step..  
-00000d10: 2020 636f 6e66 6967 5b22 7761 6e64 6222    config["wandb"
-00000d20: 5d5b 226e 616d 6522 5d20 3d20 6622 7b52  ]["name"] = f"{R
-00000d30: 554e 5f4e 414d 457d 2d7b 6374 782e 7265  UN_NAME}-{ctx.re
-00000d40: 7472 797d 220d 0a20 2020 2069 6620 6374  try}"..    if ct
-00000d50: 782e 7265 7472 7920 3e20 303a 0d0a 2020  x.retry > 0:..  
-00000d60: 2020 2020 2020 636f 6e66 6967 5b22 7472        config["tr
-00000d70: 6169 6e69 6e67 225d 5b22 6368 6563 6b70  aining"]["checkp
-00000d80: 6f69 6e74 5f6c 6f61 645f 7061 7468 225d  oint_load_path"]
-00000d90: 203d 2063 6f6e 6669 675b 2274 7261 696e   = config["train
-00000da0: 696e 6722 5d5b 2263 6865 636b 706f 696e  ing"]["checkpoin
-00000db0: 745f 7061 7468 225d 0d0a 2020 2020 636f  t_path"]..    co
-00000dc0: 6e66 6967 5b22 7472 6169 6e69 6e67 225d  nfig["training"]
-00000dd0: 5b22 6368 6563 6b70 6f69 6e74 5f70 6174  ["checkpoint_pat
-00000de0: 6822 5d20 3d20 6622 7b62 6173 655f 6368  h"] = f"{base_ch
-00000df0: 6563 6b70 6f69 6e74 5f70 6174 687d 2d7b  eckpoint_path}-{
-00000e00: 6374 782e 7265 7472 797d 220d 0a20 2020  ctx.retry}"..   
-00000e10: 2072 6574 7572 6e20 7961 6d6c 2e64 756d   return yaml.dum
-00000e20: 7028 636f 6e66 6967 290d 0a0d 0a0d 0a64  p(config)......d
-00000e30: 6566 2073 7461 7274 5f66 6e28 6374 783a  ef start_fn(ctx:
-00000e40: 2043 6f6e 7465 7874 2c20 776f 726b 6572   Context, worker
-00000e50: 3a20 696e 7429 3a0d 0a20 2020 2022 2222  : int):..    """
-00000e60: 0d0a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
-00000e70: 696f 6e20 6765 7473 2065 7865 6375 7465  ion gets execute
-00000e80: 6420 696e 2074 6872 6561 6473 2074 6f20  d in threads to 
-00000e90: 7374 6172 7420 6120 7275 6e20 6f6e 2061  start a run on a
-00000ea0: 206e 6577 2054 5055 2e20 4974 2072 6563   new TPU. It rec
-00000eb0: 6569 7665 7320 7468 6520 636f 6e74 6578  eives the contex
-00000ec0: 7420 6f62 6a65 6374 2072 6574 7572 6e65  t object returne
-00000ed0: 6420 6279 200d 0a20 2020 2060 6372 6561  d by ..    `crea
-00000ee0: 7469 6f6e 5f63 616c 6c62 6163 6b60 2061  tion_callback` a
-00000ef0: 7320 7765 6c6c 2061 7320 7468 6520 776f  s well as the wo
-00000f00: 726b 6572 2069 6420 7768 6963 6820 636f  rker id which co
-00000f10: 7272 6573 706f 6e64 7320 746f 2074 6865  rresponds to the
-00000f20: 2073 6c69 6365 2069 6420 7468 6973 2063   slice id this c
-00000f30: 6f64 6520 7761 7320 6578 6563 7574 6564  ode was executed
-00000f40: 206f 6e20 696e 2061 200d 0a20 2020 206d   on in a ..    m
-00000f50: 756c 7469 2d68 6f73 7420 7365 7475 702e  ulti-host setup.
-00000f60: 2046 6f72 2073 696e 676c 652d 686f 7374   For single-host
-00000f70: 2073 6574 7570 732c 2073 7563 6820 6173   setups, such as
-00000f80: 2076 332d 3873 2c20 7468 6520 2277 6f72   v3-8s, the "wor
-00000f90: 6b65 7222 2077 696c 6c20 616c 7761 7973  ker" will always
-00000fa0: 2062 6520 7365 7420 746f 2030 2e0d 0a20   be set to 0... 
-00000fb0: 2020 2049 6465 616c 6c79 2c20 6974 2764     Ideally, it'd
-00000fc0: 2063 6f70 7920 6e65 6365 7373 6172 7920   copy necessary 
-00000fd0: 6669 6c65 7320 746f 2074 6865 2054 5055  files to the TPU
-00000fe0: 2061 6e64 2074 6865 6e20 7275 6e20 7468   and then run th
-00000ff0: 6f73 652e 2048 6572 652c 2060 6578 6563  ose. Here, `exec
-00001000: 5f63 6f6d 6d61 6e64 6020 6361 6e20 6265  _command` can be
-00001010: 2075 7365 6420 746f 2063 7265 6174 6520   used to create 
-00001020: 616e 200d 0a20 2020 2065 7865 6375 7469  an ..    executi
-00001030: 6f6e 2063 6f6d 6d61 6e64 2074 6861 7420  on command that 
-00001040: 6175 746f 6d61 7469 6361 6c6c 7920 7370  automatically sp
-00001050: 6177 6e73 2061 2060 7363 7265 656e 6020  awns a `screen` 
-00001060: 7365 7373 696f 6e20 7768 6963 6820 7065  session which pe
-00001070: 7273 6973 7473 2065 7665 6e20 7768 656e  rsists even when
-00001080: 2074 6865 2053 5348 2063 6f6e 6e65 6374   the SSH connect
-00001090: 696f 6e20 6765 7473 2063 7574 2e0d 0a20  ion gets cut... 
-000010a0: 2020 2022 2222 0d0a 2020 2020 7365 6e64     """..    send
-000010b0: 5f74 6f5f 7470 7528 484f 5354 2c20 5a4f  _to_tpu(HOST, ZO
-000010c0: 4e45 2c20 2263 6f6e 6669 672e 7961 6d6c  NE, "config.yaml
-000010d0: 222c 206c 6f61 645f 636f 6e66 6967 2863  ", load_config(c
-000010e0: 7478 292c 2077 6f72 6b65 7229 0d0a 2020  tx), worker)..  
-000010f0: 2020 636d 6420 3d20 6578 6563 5f63 6f6d    cmd = exec_com
-00001100: 6d61 6e64 2872 6570 6f73 6974 6f72 793d  mand(repository=
-00001110: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001120: 636f 6d2f 486f 6d65 6272 6577 4e4c 502f  com/HomebrewNLP/
-00001130: 486f 6d65 6272 6577 4e4c 502d 4a61 7822  HomebrewNLP-Jax"
-00001140: 2c20 7761 6e64 625f 6b65 793d 7761 6e64  , wandb_key=wand
-00001150: 625f 6b65 7929 0d0a 2020 2020 7365 6e64  b_key)..    send
-00001160: 5f74 6f5f 7470 7528 484f 5354 2c20 5a4f  _to_tpu(HOST, ZO
-00001170: 4e45 2c20 2273 6574 7570 2e73 6822 2c20  NE, "setup.sh", 
-00001180: 636d 642c 2077 6f72 6b65 7229 0d0a 2020  cmd, worker)..  
-00001190: 2020 6578 6563 5f6f 6e5f 7470 7528 484f    exec_on_tpu(HO
-000011a0: 5354 2c20 5a4f 4e45 2c20 2262 6173 6820  ST, ZONE, "bash 
-000011b0: 7365 7475 702e 7368 222c 2077 6f72 6b65  setup.sh", worke
-000011c0: 7229 0d0a 0d0a 0d0a 6465 6620 6372 6561  r)......def crea
-000011d0: 7469 6f6e 5f63 616c 6c62 6163 6b28 686f  tion_callback(ho
-000011e0: 7374 3a20 7374 722c 2063 7478 3a20 7479  st: str, ctx: ty
-000011f0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 436f  ping.Optional[Co
-00001200: 6e74 6578 745d 2920 2d3e 2043 6f6e 7465  ntext]) -> Conte
-00001210: 7874 3a0d 0a20 2020 2022 2222 0d0a 2020  xt:..    """..  
-00001220: 2020 5468 6520 6063 7265 6174 696f 6e5f    The `creation_
-00001230: 6361 6c6c 6261 636b 6020 6973 2063 616c  callback` is cal
-00001240: 6c65 6420 6f6e 6365 2077 6865 6e65 7665  led once wheneve
-00001250: 7220 6120 6e65 7720 5450 5520 6765 7473  r a new TPU gets
-00001260: 2063 7265 6174 6564 2061 6e64 2063 616e   created and can
-00001270: 2062 6520 7573 6564 2074 6f20 7065 7273   be used to pers
-00001280: 6973 7420 7374 6174 650d 0a20 2020 2028  ist state..    (
-00001290: 7375 6368 2061 7320 7265 7472 7920 636f  such as retry co
-000012a0: 756e 7465 7273 2920 6163 726f 7373 206d  unters) across m
-000012b0: 756c 7469 706c 6520 696e 766f 6361 7469  ultiple invocati
-000012c0: 6f6e 732e 0d0a 2020 2020 2222 220d 0a20  ons...    """.. 
-000012d0: 2020 2069 6620 6374 7820 6973 204e 6f6e     if ctx is Non
-000012e0: 653a 2020 2320 6669 7273 7420 696e 766f  e:  # first invo
-000012f0: 6361 7469 6f6e 0d0a 2020 2020 2020 2020  cation..        
-00001300: 7265 7475 726e 2043 6f6e 7465 7874 2830  return Context(0
-00001310: 290d 0a20 2020 2063 7478 2e72 6574 7279  )..    ctx.retry
-00001320: 202b 3d20 310d 0a20 2020 2072 6574 7572   += 1..    retur
-00001330: 6e20 6374 780d 0a0d 0a0d 0a64 6566 206d  n ctx......def m
-00001340: 6169 6e28 7365 7276 6963 655f 6163 636f  ain(service_acco
-00001350: 756e 743a 2073 7472 2c20 7470 755f 7665  unt: str, tpu_ve
-00001360: 7273 696f 6e3a 2069 6e74 203d 2033 2c20  rsion: int = 3, 
-00001370: 736c 6963 6573 3a20 696e 7420 3d20 3332  slices: int = 32
-00001380: 2c20 7072 6565 6d70 7469 626c 653a 2062  , preemptible: b
-00001390: 6f6f 6c20 3d20 5472 7565 293a 0d0a 2020  ool = True):..  
-000013a0: 2020 7374 6172 745f 7369 6e67 6c65 2868    start_single(h
-000013b0: 6f73 743d 484f 5354 2c20 7470 755f 7665  ost=HOST, tpu_ve
-000013c0: 7273 696f 6e3d 7470 755f 7665 7273 696f  rsion=tpu_versio
-000013d0: 6e2c 207a 6f6e 653d 5a4f 4e45 2c20 7072  n, zone=ZONE, pr
-000013e0: 6565 6d70 7469 626c 653d 7072 6565 6d70  eemptible=preemp
-000013f0: 7469 626c 652c 0d0a 2020 2020 2020 2020  tible,..        
-00001400: 2020 2020 2020 2020 2073 6572 7669 6365           service
-00001410: 5f61 6363 6f75 6e74 3d73 6572 7669 6365  _account=service
-00001420: 5f61 6363 6f75 6e74 2c20 736c 6963 6573  _account, slices
-00001430: 3d73 6c69 6365 732c 2073 7461 7274 5f66  =slices, start_f
-00001440: 6e3d 7374 6172 745f 666e 2c0d 0a20 2020  n=start_fn,..   
-00001450: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-00001460: 6561 7469 6f6e 5f63 616c 6c62 6163 6b3d  eation_callback=
-00001470: 6372 6561 7469 6f6e 5f63 616c 6c62 6163  creation_callbac
-00001480: 6b29 0d0a 6060 600d 0a0d 0a23 2323 2053  k)..```....### S
-00001490: 7765 6570 730d 0a0d 0a53 696d 696c 6172  weeps....Similar
-000014a0: 6c79 2c20 6c61 7267 6520 7377 6172 6d73  ly, large swarms
-000014b0: 206f 6620 696e 7374 616e 6365 7320 6361   of instances ca
-000014c0: 6e20 6265 206c 6175 6e63 6865 6420 7472  n be launched tr
-000014d0: 6976 6961 6c6c 7920 7573 696e 6720 7470  ivially using tp
-000014e0: 7563 6172 652e 2048 6572 652c 2077 6520  ucare. Here, we 
-000014f0: 6c61 7267 656c 7920 646f 2074 6865 2073  largely do the s
-00001500: 616d 6520 7365 7475 7020 6173 0d0a 6162  ame setup as..ab
-00001510: 6f76 652c 2062 7574 2063 616c 6c20 606c  ove, but call `l
-00001520: 6175 6e63 685f 6d75 6c74 6970 6c65 6020  aunch_multiple` 
-00001530: 696e 7374 6561 6420 6f66 2060 6c61 756e  instead of `laun
-00001540: 6368 5f73 696e 676c 6560 2077 6869 6368  ch_single` which
-00001550: 2074 616b 6573 2074 6865 2061 6464 6974   takes the addit
-00001560: 696f 6e61 6c20 6172 6775 6d65 6e74 2060  ional argument `
-00001570: 7470 7573 6020 7370 6563 6966 7969 6e67  tpus` specifying
-00001580: 2074 6865 0d0a 6e75 6d62 6572 206f 6620   the..number of 
-00001590: 5450 5573 2074 6861 7420 7368 6f75 6c64  TPUs that should
-000015a0: 2062 6520 6c61 756e 6368 6564 2061 6e64   be launched and
-000015b0: 2062 6162 7973 6974 2e20 4465 7065 6e64   babysit. Depend
-000015c0: 696e 6720 6f6e 2063 6170 6163 6974 7920  ing on capacity 
-000015d0: 616e 6420 7175 6f74 612c 2074 6865 2061  and quota, the a
-000015e0: 6374 7561 6c20 6e75 6d62 6572 206f 6620  ctual number of 
-000015f0: 5450 5573 2079 6f75 2067 6574 0d0a 6d69  TPUs you get..mi
-00001600: 6768 7420 6265 206c 6f77 6572 2074 6861  ght be lower tha
-00001610: 6e20 7468 6520 6e75 6d62 6572 206f 6620  n the number of 
-00001620: 5450 5573 2073 7065 6369 6669 6564 2e0d  TPUs specified..
-00001630: 0a0d 0a60 6060 5059 5448 4f4e 0d0a 6465  ...```PYTHON..de
-00001640: 6620 6d61 696e 2873 6572 7669 6365 5f61  f main(service_a
-00001650: 6363 6f75 6e74 3a20 7374 722c 2074 7075  ccount: str, tpu
-00001660: 733a 2069 6e74 2c20 7470 755f 7665 7273  s: int, tpu_vers
-00001670: 696f 6e3a 2069 6e74 203d 2033 2c20 736c  ion: int = 3, sl
-00001680: 6963 6573 3a20 696e 7420 3d20 3332 2c20  ices: int = 32, 
-00001690: 7072 6565 6d70 7469 626c 653a 2062 6f6f  preemptible: boo
-000016a0: 6c20 3d20 5472 7565 293a 0d0a 2020 2020  l = True):..    
-000016b0: 7374 6172 745f 6d75 6c74 6970 6c65 2870  start_multiple(p
-000016c0: 7265 6669 783d 484f 5354 2c20 7470 755f  refix=HOST, tpu_
-000016d0: 7665 7273 696f 6e3d 7470 755f 7665 7273  version=tpu_vers
-000016e0: 696f 6e2c 207a 6f6e 653d 5a4f 4e45 2c20  ion, zone=ZONE, 
-000016f0: 7072 6565 6d70 7469 626c 653d 7072 6565  preemptible=pree
-00001700: 6d70 7469 626c 652c 0d0a 2020 2020 2020  mptible,..      
-00001710: 2020 2020 2020 2020 2020 2020 2073 6572               ser
-00001720: 7669 6365 5f61 6363 6f75 6e74 3d73 6572  vice_account=ser
-00001730: 7669 6365 5f61 6363 6f75 6e74 2c20 736c  vice_account, sl
-00001740: 6963 6573 3d73 6c69 6365 732c 2073 7461  ices=slices, sta
-00001750: 7274 5f66 6e3d 7374 6172 745f 666e 2c0d  rt_fn=start_fn,.
-00001760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001770: 2020 2020 6372 6561 7469 6f6e 5f63 616c      creation_cal
-00001780: 6c62 6163 6b3d 6372 6561 7469 6f6e 5f63  lback=creation_c
-00001790: 616c 6c62 6163 6b2c 2074 7075 733d 7470  allback, tpus=tp
-000017a0: 7573 290d 0a60 6060 0d0a 0d0a 486f 7765  us)..```....Howe
-000017b0: 7665 722c 2074 6869 7320 776f 756c 6420  ver, this would 
-000017c0: 7369 6d70 6c79 206c 6175 6e63 6820 7468  simply launch th
-000017d0: 6520 7361 6d65 2072 756e 206d 616e 7920  e same run many 
-000017e0: 7469 6d65 732e 2049 6620 796f 7520 696e  times. If you in
-000017f0: 7374 6561 6420 706c 616e 2074 6f20 7265  stead plan to re
-00001800: 6769 7374 6572 2074 6865 6d20 7769 7468  gister them with
-00001810: 2061 0d0a 5b57 616e 6442 2053 7765 6570   a..[WandB Sweep
-00001820: 5d28 6874 7470 733a 2f2f 646f 6373 2e77  ](https://docs.w
-00001830: 616e 6462 2e61 692f 6775 6964 6573 2f73  andb.ai/guides/s
-00001840: 7765 6570 732f 636f 6e66 6967 7572 6174  weeps/configurat
-00001850: 696f 6e29 2c20 7765 206e 6565 6420 746f  ion), we need to
-00001860: 206d 6f64 6966 7920 7468 6520 6073 7461   modify the `sta
-00001870: 7274 5f66 6e60 2074 6f20 6a6f 696e 2074  rt_fn` to join t
-00001880: 6865 2077 616e 6462 0d0a 7377 6565 702e  he wandb..sweep.
-00001890: 5c0d 0a42 7920 7061 7463 6869 6e67 2069  \..By patching i
-000018a0: 6e20 7468 6520 636f 6465 2062 656c 6f77  n the code below
-000018b0: 2c20 7470 7563 6172 6520 7769 6c6c 2073  , tpucare will s
-000018c0: 7461 7274 2061 6e64 206d 6169 6e74 6169  tart and maintai
-000018d0: 6e20 6120 6c61 7267 6520 7377 6172 6d20  n a large swarm 
-000018e0: 6f66 2054 5055 7320 616c 6c20 776f 726b  of TPUs all work
-000018f0: 696e 6720 746f 7761 7264 7320 7468 6520  ing towards the 
-00001900: 7361 6d65 0d0a 6879 7065 7270 6172 616d  same..hyperparam
-00001910: 6574 6572 206f 7074 696d 697a 6174 696f  eter optimizatio
-00001920: 6e20 7072 6f62 6c65 6d2e 0d0a 0d0a 6060  n problem.....``
-00001930: 6050 5954 484f 4e0d 0a69 6d70 6f72 7420  `PYTHON..import 
-00001940: 7761 6e64 620d 0a0d 0a77 6974 6820 6f70  wandb....with op
-00001950: 656e 2822 7377 6565 702e 7961 6d6c 222c  en("sweep.yaml",
-00001960: 2027 7227 2920 6173 2066 3a20 2023 2073   'r') as f:  # s
-00001970: 7765 6570 2063 6f6e 6669 6720 7061 7373  weep config pass
-00001980: 6564 2073 7472 6169 6768 7420 746f 2077  ed straight to w
-00001990: 616e 6462 0d0a 2020 2020 636f 6e66 6967  andb..    config
-000019a0: 203d 2079 616d 6c2e 7361 6665 5f6c 6f61   = yaml.safe_loa
-000019b0: 6428 662e 7265 6164 2829 290d 0a73 7765  d(f.read())..swe
-000019c0: 6570 5f69 6420 3d20 7761 6e64 622e 7377  ep_id = wandb.sw
-000019d0: 6565 7028 636f 6e66 6967 2c20 656e 7469  eep(config, enti
-000019e0: 7479 3d22 686f 6d65 6272 6577 6e6c 7022  ty="homebrewnlp"
-000019f0: 2c20 7072 6f6a 6563 743d 2267 7074 2229  , project="gpt")
-00001a00: 0d0a 0d0a 0d0a 6465 6620 7374 6172 745f  ......def start_
-00001a10: 666e 2863 7478 3a20 436f 6e74 6578 742c  fn(ctx: Context,
-00001a20: 2077 6f72 6b65 723a 2069 6e74 293a 0d0a   worker: int):..
-00001a30: 2020 2020 636d 6420 3d20 6578 6563 5f63      cmd = exec_c
-00001a40: 6f6d 6d61 6e64 2872 6570 6f73 6974 6f72  ommand(repositor
-00001a50: 793d 2268 7474 7073 3a2f 2f67 6974 6875  y="https://githu
-00001a60: 622e 636f 6d2f 486f 6d65 6272 6577 4e4c  b.com/HomebrewNL
-00001a70: 502f 486f 6d65 6272 6577 4e4c 502d 4a61  P/HomebrewNLP-Ja
-00001a80: 7822 2c20 7761 6e64 625f 6b65 793d 7761  x", wandb_key=wa
-00001a90: 6e64 625f 6b65 792c 0d0a 2020 2020 2020  ndb_key,..      
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2072 756e 5f63 6f6d 6d61 6e64 3d66 222f   run_command=f"/
-00001ac0: 686f 6d65 2f75 6275 6e74 752f 2e6c 6f63  home/ubuntu/.loc
-00001ad0: 616c 2f62 696e 2f77 616e 6462 2061 6765  al/bin/wandb age
-00001ae0: 6e74 207b 7377 6565 705f 6964 7d22 290d  nt {sweep_id}").
-00001af0: 0a20 2020 2073 656e 645f 746f 5f74 7075  .    send_to_tpu
-00001b00: 2848 4f53 542c 205a 4f4e 452c 2022 7365  (HOST, ZONE, "se
-00001b10: 7475 702e 7368 222c 2063 6d64 2c20 776f  tup.sh", cmd, wo
-00001b20: 726b 6572 290d 0a20 2020 2065 7865 635f  rker)..    exec_
-00001b30: 6f6e 5f74 7075 2848 4f53 542c 205a 4f4e  on_tpu(HOST, ZON
-00001b40: 452c 2022 6261 7368 2073 6574 7570 2e73  E, "bash setup.s
-00001b50: 6822 2c20 776f 726b 6572 290d 0a60 6060  h", worker)..```
-00001b60: 0d0a 0d0a 5468 6520 6675 6c6c 2065 7865  ....The full exe
-00001b70: 6375 7461 626c 6520 636f 6465 2063 616e  cutable code can
-00001b80: 2062 6520 666f 756e 640d 0a69 6e20 5b65   be found..in [e
-00001b90: 7861 6d70 6c65 732f 7377 6565 702e 7079  xamples/sweep.py
-00001ba0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001bb0: 2e63 6f6d 2f63 6c61 7368 6c75 6b65 2f74  .com/clashluke/t
-00001bc0: 7075 6361 7265 2f62 6c6f 622f 6d61 696e  pucare/blob/main
-00001bd0: 2f65 7861 6d70 6c65 732f 7377 6565 702e  /examples/sweep.
-00001be0: 7079 292e 0d0a 0d0a 5369 6d69 6c61 726c  py).....Similarl
-00001bf0: 792c 2074 6865 2060 7374 6172 745f 666e  y, the `start_fn
-00001c00: 6020 636f 756c 6420 6265 2061 6461 7074  ` could be adapt
-00001c10: 6564 2074 6f20 7374 6172 7420 616e 2069  ed to start an i
-00001c20: 6e66 6572 656e 6365 2073 6572 7665 720d  nference server.
-00001c30: 0a66 6f72 205b 486f 6d65 6272 6577 4e4c  .for [HomebrewNL
-00001c40: 505d 2868 7474 7073 3a2f 2f67 6974 6875  P](https://githu
-00001c50: 622e 636f 6d2f 486f 6d65 6272 6577 4e4c  b.com/HomebrewNL
-00001c60: 502f 486f 6d65 6272 6577 4e4c 502d 4a61  P/HomebrewNLP-Ja
-00001c70: 782f 290d 0a6f 7220 5b43 7261 6979 6f6e  x/)..or [Craiyon
-00001c80: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00001c90: 6766 6163 652e 636f 2f73 7061 6365 732f  gface.co/spaces/
-00001ca0: 6461 6c6c 652d 6d69 6e69 2f64 616c 6c65  dalle-mini/dalle
-00001cb0: 2d6d 696e 6929 206f 7220 6576 656e 2065  -mini) or even e
-00001cc0: 7865 6375 7465 206d 6163 6869 6e65 206c  xecute machine l
-00001cd0: 6561 726e 696e 6720 756e 6974 2d74 6573  earning unit-tes
-00001ce0: 7473 2069 6e0d 0a70 6172 616c 6c65 6c2e  ts in..parallel.
-00001cf0: 0d0a 0d0a 2323 2043 6974 6174 696f 6e0d  ....## Citation.
-00001d00: 0a0d 0a60 6060 4249 4254 4558 0d0a 4073  ...```BIBTEX..@s
-00001d10: 6f66 7477 6172 657b 6e65 7374 6c65 725f  oftware{nestler_
-00001d20: 6c75 6361 735f 3230 3232 5f36 3833 3733  lucas_2022_68373
-00001d30: 3132 2c0d 0a20 2061 7574 686f 7220 2020  12,..  author   
-00001d40: 2020 2020 3d20 7b4e 6573 746c 6572 2c20      = {Nestler, 
-00001d50: 4c75 6361 737d 2c0d 0a20 2074 6974 6c65  Lucas},..  title
-00001d60: 2020 2020 2020 2020 3d20 7b54 5055 2043          = {TPU C
-00001d70: 6172 657d 2c0d 0a20 206d 6f6e 7468 2020  are},..  month  
-00001d80: 2020 2020 2020 3d20 6a75 6c2c 0d0a 2020        = jul,..  
-00001d90: 7965 6172 2020 2020 2020 2020 203d 2032  year         = 2
-00001da0: 3032 322c 0d0a 2020 7075 626c 6973 6865  022,..  publishe
-00001db0: 7220 2020 203d 207b 5a65 6e6f 646f 7d2c  r    = {Zenodo},
-00001dc0: 0d0a 2020 7665 7273 696f 6e20 2020 2020  ..  version     
-00001dd0: 203d 207b 302e 302e 327d 2c0d 0a20 2064   = {0.0.2},..  d
-00001de0: 6f69 2020 2020 2020 2020 2020 3d20 7b31  oi          = {1
-00001df0: 302e 3532 3831 2f7a 656e 6f64 6f2e 3638  0.5281/zenodo.68
-00001e00: 3337 3331 327d 2c0d 0a20 2075 726c 2020  37312},..  url  
-00001e10: 2020 2020 2020 2020 3d20 7b68 7474 7073          = {https
-00001e20: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3532  ://doi.org/10.52
-00001e30: 3831 2f7a 656e 6f64 6f2e 3638 3337 3331  81/zenodo.683731
-00001e40: 327d 0d0a 7d60 6060                      2}..}```
+00000bf0: 276e 616d 6527 5d3a 0a20 2020 2020 2020  'name']:.       
+00000c00: 2020 2020 2073 7461 7274 5f73 7465 7020       start_step 
+00000c10: 3d20 7275 6e2e 7375 6d6d 6172 795b 225f  = run.summary["_
+00000c20: 7374 6570 225d 0a20 2020 2020 2020 2020  step"].         
+00000c30: 2020 2062 7265 616b 0a20 2020 2073 7461     break.    sta
+00000c40: 7274 5f73 7465 7020 2d3d 2073 7461 7274  rt_step -= start
+00000c50: 5f73 7465 7020 2520 636f 6e66 6967 5b22  _step % config["
+00000c60: 7472 6169 6e69 6e67 225d 5b22 6368 6563  training"]["chec
+00000c70: 6b70 6f69 6e74 5f69 6e74 6572 7661 6c22  kpoint_interval"
+00000c80: 5d0a 0a20 2020 2063 6f6e 6669 675b 2274  ]..    config["t
+00000c90: 7261 696e 696e 6722 5d5b 2273 7461 7274  raining"]["start
+00000ca0: 5f73 7465 7022 5d20 3d20 7374 6172 745f  _step"] = start_
+00000cb0: 7374 6570 0a20 2020 2063 6f6e 6669 675b  step.    config[
+00000cc0: 2277 616e 6462 225d 5b22 6e61 6d65 225d  "wandb"]["name"]
+00000cd0: 203d 2066 227b 5255 4e5f 4e41 4d45 7d2d   = f"{RUN_NAME}-
+00000ce0: 7b63 7478 2e72 6574 7279 7d22 0a20 2020  {ctx.retry}".   
+00000cf0: 2069 6620 6374 782e 7265 7472 7920 3e20   if ctx.retry > 
+00000d00: 303a 0a20 2020 2020 2020 2063 6f6e 6669  0:.        confi
+00000d10: 675b 2274 7261 696e 696e 6722 5d5b 2263  g["training"]["c
+00000d20: 6865 636b 706f 696e 745f 6c6f 6164 5f70  heckpoint_load_p
+00000d30: 6174 6822 5d20 3d20 636f 6e66 6967 5b22  ath"] = config["
+00000d40: 7472 6169 6e69 6e67 225d 5b22 6368 6563  training"]["chec
+00000d50: 6b70 6f69 6e74 5f70 6174 6822 5d0a 2020  kpoint_path"].  
+00000d60: 2020 636f 6e66 6967 5b22 7472 6169 6e69    config["traini
+00000d70: 6e67 225d 5b22 6368 6563 6b70 6f69 6e74  ng"]["checkpoint
+00000d80: 5f70 6174 6822 5d20 3d20 6622 7b62 6173  _path"] = f"{bas
+00000d90: 655f 6368 6563 6b70 6f69 6e74 5f70 6174  e_checkpoint_pat
+00000da0: 687d 2d7b 6374 782e 7265 7472 797d 220a  h}-{ctx.retry}".
+00000db0: 2020 2020 7265 7475 726e 2079 616d 6c2e      return yaml.
+00000dc0: 6475 6d70 2863 6f6e 6669 6729 0a0a 0a64  dump(config)...d
+00000dd0: 6566 2073 7461 7274 5f66 6e28 6374 783a  ef start_fn(ctx:
+00000de0: 2043 6f6e 7465 7874 2c20 776f 726b 6572   Context, worker
+00000df0: 3a20 696e 7429 3a0a 2020 2020 2222 220a  : int):.    """.
+00000e00: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+00000e10: 6e20 6765 7473 2065 7865 6375 7465 6420  n gets executed 
+00000e20: 696e 2074 6872 6561 6473 2074 6f20 7374  in threads to st
+00000e30: 6172 7420 6120 7275 6e20 6f6e 2061 206e  art a run on a n
+00000e40: 6577 2054 5055 2e20 4974 2072 6563 6569  ew TPU. It recei
+00000e50: 7665 7320 7468 6520 636f 6e74 6578 7420  ves the context 
+00000e60: 6f62 6a65 6374 2072 6574 7572 6e65 6420  object returned 
+00000e70: 6279 200a 2020 2020 6063 7265 6174 696f  by .    `creatio
+00000e80: 6e5f 6361 6c6c 6261 636b 6020 6173 2077  n_callback` as w
+00000e90: 656c 6c20 6173 2074 6865 2077 6f72 6b65  ell as the worke
+00000ea0: 7220 6964 2077 6869 6368 2063 6f72 7265  r id which corre
+00000eb0: 7370 6f6e 6473 2074 6f20 7468 6520 736c  sponds to the sl
+00000ec0: 6963 6520 6964 2074 6869 7320 636f 6465  ice id this code
+00000ed0: 2077 6173 2065 7865 6375 7465 6420 6f6e   was executed on
+00000ee0: 2069 6e20 6120 0a20 2020 206d 756c 7469   in a .    multi
+00000ef0: 2d68 6f73 7420 7365 7475 702e 2046 6f72  -host setup. For
+00000f00: 2073 696e 676c 652d 686f 7374 2073 6574   single-host set
+00000f10: 7570 732c 2073 7563 6820 6173 2076 332d  ups, such as v3-
+00000f20: 3873 2c20 7468 6520 2277 6f72 6b65 7222  8s, the "worker"
+00000f30: 2077 696c 6c20 616c 7761 7973 2062 6520   will always be 
+00000f40: 7365 7420 746f 2030 2e0a 2020 2020 4964  set to 0..    Id
+00000f50: 6561 6c6c 792c 2069 7427 6420 636f 7079  eally, it'd copy
+00000f60: 206e 6563 6573 7361 7279 2066 696c 6573   necessary files
+00000f70: 2074 6f20 7468 6520 5450 5520 616e 6420   to the TPU and 
+00000f80: 7468 656e 2072 756e 2074 686f 7365 2e20  then run those. 
+00000f90: 4865 7265 2c20 6065 7865 635f 636f 6d6d  Here, `exec_comm
+00000fa0: 616e 6460 2063 616e 2062 6520 7573 6564  and` can be used
+00000fb0: 2074 6f20 6372 6561 7465 2061 6e20 0a20   to create an . 
+00000fc0: 2020 2065 7865 6375 7469 6f6e 2063 6f6d     execution com
+00000fd0: 6d61 6e64 2074 6861 7420 6175 746f 6d61  mand that automa
+00000fe0: 7469 6361 6c6c 7920 7370 6177 6e73 2061  tically spawns a
+00000ff0: 2060 7363 7265 656e 6020 7365 7373 696f   `screen` sessio
+00001000: 6e20 7768 6963 6820 7065 7273 6973 7473  n which persists
+00001010: 2065 7665 6e20 7768 656e 2074 6865 2053   even when the S
+00001020: 5348 2063 6f6e 6e65 6374 696f 6e20 6765  SH connection ge
+00001030: 7473 2063 7574 2e0a 2020 2020 2222 220a  ts cut..    """.
+00001040: 2020 2020 7365 6e64 5f74 6f5f 7470 7528      send_to_tpu(
+00001050: 484f 5354 2c20 5a4f 4e45 2c20 2263 6f6e  HOST, ZONE, "con
+00001060: 6669 672e 7961 6d6c 222c 206c 6f61 645f  fig.yaml", load_
+00001070: 636f 6e66 6967 2863 7478 292c 2077 6f72  config(ctx), wor
+00001080: 6b65 7229 0a20 2020 2063 6d64 203d 2065  ker).    cmd = e
+00001090: 7865 635f 636f 6d6d 616e 6428 7265 706f  xec_command(repo
+000010a0: 7369 746f 7279 3d22 6874 7470 733a 2f2f  sitory="https://
+000010b0: 6769 7468 7562 2e63 6f6d 2f48 6f6d 6562  github.com/Homeb
+000010c0: 7265 774e 4c50 2f48 6f6d 6562 7265 774e  rewNLP/HomebrewN
+000010d0: 4c50 2d4a 6178 222c 2077 616e 6462 5f6b  LP-Jax", wandb_k
+000010e0: 6579 3d77 616e 6462 5f6b 6579 290a 2020  ey=wandb_key).  
+000010f0: 2020 7365 6e64 5f74 6f5f 7470 7528 484f    send_to_tpu(HO
+00001100: 5354 2c20 5a4f 4e45 2c20 2273 6574 7570  ST, ZONE, "setup
+00001110: 2e73 6822 2c20 636d 642c 2077 6f72 6b65  .sh", cmd, worke
+00001120: 7229 0a20 2020 2065 7865 635f 6f6e 5f74  r).    exec_on_t
+00001130: 7075 2848 4f53 542c 205a 4f4e 452c 2022  pu(HOST, ZONE, "
+00001140: 6261 7368 2073 6574 7570 2e73 6822 2c20  bash setup.sh", 
+00001150: 776f 726b 6572 290a 0a0a 6465 6620 6372  worker)...def cr
+00001160: 6561 7469 6f6e 5f63 616c 6c62 6163 6b28  eation_callback(
+00001170: 686f 7374 3a20 7374 722c 2063 7478 3a20  host: str, ctx: 
+00001180: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001190: 436f 6e74 6578 745d 2920 2d3e 2043 6f6e  Context]) -> Con
+000011a0: 7465 7874 3a0a 2020 2020 2222 220a 2020  text:.    """.  
+000011b0: 2020 5468 6520 6063 7265 6174 696f 6e5f    The `creation_
+000011c0: 6361 6c6c 6261 636b 6020 6973 2063 616c  callback` is cal
+000011d0: 6c65 6420 6f6e 6365 2077 6865 6e65 7665  led once wheneve
+000011e0: 7220 6120 6e65 7720 5450 5520 6765 7473  r a new TPU gets
+000011f0: 2063 7265 6174 6564 2061 6e64 2063 616e   created and can
+00001200: 2062 6520 7573 6564 2074 6f20 7065 7273   be used to pers
+00001210: 6973 7420 7374 6174 650a 2020 2020 2873  ist state.    (s
+00001220: 7563 6820 6173 2072 6574 7279 2063 6f75  uch as retry cou
+00001230: 6e74 6572 7329 2061 6372 6f73 7320 6d75  nters) across mu
+00001240: 6c74 6970 6c65 2069 6e76 6f63 6174 696f  ltiple invocatio
+00001250: 6e73 2e0a 2020 2020 2222 220a 2020 2020  ns..    """.    
+00001260: 6966 2063 7478 2069 7320 4e6f 6e65 3a20  if ctx is None: 
+00001270: 2023 2066 6972 7374 2069 6e76 6f63 6174   # first invocat
+00001280: 696f 6e0a 2020 2020 2020 2020 7265 7475  ion.        retu
+00001290: 726e 2043 6f6e 7465 7874 2830 290a 2020  rn Context(0).  
+000012a0: 2020 6374 782e 7265 7472 7920 2b3d 2031    ctx.retry += 1
+000012b0: 0a20 2020 2072 6574 7572 6e20 6374 780a  .    return ctx.
+000012c0: 0a0a 6465 6620 6d61 696e 2873 6572 7669  ..def main(servi
+000012d0: 6365 5f61 6363 6f75 6e74 3a20 7374 722c  ce_account: str,
+000012e0: 2074 7075 5f76 6572 7369 6f6e 3a20 696e   tpu_version: in
+000012f0: 7420 3d20 332c 2073 6c69 6365 733a 2069  t = 3, slices: i
+00001300: 6e74 203d 2033 322c 2070 7265 656d 7074  nt = 32, preempt
+00001310: 6962 6c65 3a20 626f 6f6c 203d 2054 7275  ible: bool = Tru
+00001320: 6529 3a0a 2020 2020 7374 6172 745f 7369  e):.    start_si
+00001330: 6e67 6c65 2868 6f73 743d 484f 5354 2c20  ngle(host=HOST, 
+00001340: 7470 755f 7665 7273 696f 6e3d 7470 755f  tpu_version=tpu_
+00001350: 7665 7273 696f 6e2c 207a 6f6e 653d 5a4f  version, zone=ZO
+00001360: 4e45 2c20 7072 6565 6d70 7469 626c 653d  NE, preemptible=
+00001370: 7072 6565 6d70 7469 626c 652c 0a20 2020  preemptible,.   
+00001380: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001390: 7276 6963 655f 6163 636f 756e 743d 7365  rvice_account=se
+000013a0: 7276 6963 655f 6163 636f 756e 742c 2073  rvice_account, s
+000013b0: 6c69 6365 733d 736c 6963 6573 2c20 7374  lices=slices, st
+000013c0: 6172 745f 666e 3d73 7461 7274 5f66 6e2c  art_fn=start_fn,
+000013d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013e0: 2020 6372 6561 7469 6f6e 5f63 616c 6c62    creation_callb
+000013f0: 6163 6b3d 6372 6561 7469 6f6e 5f63 616c  ack=creation_cal
+00001400: 6c62 6163 6b29 0a60 6060 0a0a 2323 2320  lback).```..### 
+00001410: 5377 6565 7073 0a0a 5369 6d69 6c61 726c  Sweeps..Similarl
+00001420: 792c 206c 6172 6765 2073 7761 726d 7320  y, large swarms 
+00001430: 6f66 2069 6e73 7461 6e63 6573 2063 616e  of instances can
+00001440: 2062 6520 6c61 756e 6368 6564 2074 7269   be launched tri
+00001450: 7669 616c 6c79 2075 7369 6e67 2074 7075  vially using tpu
+00001460: 6361 7265 2e20 4865 7265 2c20 7765 206c  care. Here, we l
+00001470: 6172 6765 6c79 2064 6f20 7468 6520 7361  argely do the sa
+00001480: 6d65 2073 6574 7570 2061 730a 6162 6f76  me setup as.abov
+00001490: 652c 2062 7574 2063 616c 6c20 606c 6175  e, but call `lau
+000014a0: 6e63 685f 6d75 6c74 6970 6c65 6020 696e  nch_multiple` in
+000014b0: 7374 6561 6420 6f66 2060 6c61 756e 6368  stead of `launch
+000014c0: 5f73 696e 676c 6560 2077 6869 6368 2074  _single` which t
+000014d0: 616b 6573 2074 6865 2061 6464 6974 696f  akes the additio
+000014e0: 6e61 6c20 6172 6775 6d65 6e74 2060 7470  nal argument `tp
+000014f0: 7573 6020 7370 6563 6966 7969 6e67 2074  us` specifying t
+00001500: 6865 0a6e 756d 6265 7220 6f66 2054 5055  he.number of TPU
+00001510: 7320 7468 6174 2073 686f 756c 6420 6265  s that should be
+00001520: 206c 6175 6e63 6865 6420 616e 6420 6261   launched and ba
+00001530: 6279 7369 742e 2044 6570 656e 6469 6e67  bysit. Depending
+00001540: 206f 6e20 6361 7061 6369 7479 2061 6e64   on capacity and
+00001550: 2071 756f 7461 2c20 7468 6520 6163 7475   quota, the actu
+00001560: 616c 206e 756d 6265 7220 6f66 2054 5055  al number of TPU
+00001570: 7320 796f 7520 6765 740a 6d69 6768 7420  s you get.might 
+00001580: 6265 206c 6f77 6572 2074 6861 6e20 7468  be lower than th
+00001590: 6520 6e75 6d62 6572 206f 6620 5450 5573  e number of TPUs
+000015a0: 2073 7065 6369 6669 6564 2e0a 0a60 6060   specified...```
+000015b0: 5059 5448 4f4e 0a64 6566 206d 6169 6e28  PYTHON.def main(
+000015c0: 7365 7276 6963 655f 6163 636f 756e 743a  service_account:
+000015d0: 2073 7472 2c20 7470 7573 3a20 696e 742c   str, tpus: int,
+000015e0: 2074 7075 5f76 6572 7369 6f6e 3a20 696e   tpu_version: in
+000015f0: 7420 3d20 332c 2073 6c69 6365 733a 2069  t = 3, slices: i
+00001600: 6e74 203d 2033 322c 2070 7265 656d 7074  nt = 32, preempt
+00001610: 6962 6c65 3a20 626f 6f6c 203d 2054 7275  ible: bool = Tru
+00001620: 6529 3a0a 2020 2020 7374 6172 745f 6d75  e):.    start_mu
+00001630: 6c74 6970 6c65 2870 7265 6669 783d 484f  ltiple(prefix=HO
+00001640: 5354 2c20 7470 755f 7665 7273 696f 6e3d  ST, tpu_version=
+00001650: 7470 755f 7665 7273 696f 6e2c 207a 6f6e  tpu_version, zon
+00001660: 653d 5a4f 4e45 2c20 7072 6565 6d70 7469  e=ZONE, preempti
+00001670: 626c 653d 7072 6565 6d70 7469 626c 652c  ble=preemptible,
+00001680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001690: 2020 2020 7365 7276 6963 655f 6163 636f      service_acco
+000016a0: 756e 743d 7365 7276 6963 655f 6163 636f  unt=service_acco
+000016b0: 756e 742c 2073 6c69 6365 733d 736c 6963  unt, slices=slic
+000016c0: 6573 2c20 7374 6172 745f 666e 3d73 7461  es, start_fn=sta
+000016d0: 7274 5f66 6e2c 0a20 2020 2020 2020 2020  rt_fn,.         
+000016e0: 2020 2020 2020 2020 2020 6372 6561 7469            creati
+000016f0: 6f6e 5f63 616c 6c62 6163 6b3d 6372 6561  on_callback=crea
+00001700: 7469 6f6e 5f63 616c 6c62 6163 6b2c 2074  tion_callback, t
+00001710: 7075 733d 7470 7573 290a 6060 600a 0a48  pus=tpus).```..H
+00001720: 6f77 6576 6572 2c20 7468 6973 2077 6f75  owever, this wou
+00001730: 6c64 2073 696d 706c 7920 6c61 756e 6368  ld simply launch
+00001740: 2074 6865 2073 616d 6520 7275 6e20 6d61   the same run ma
+00001750: 6e79 2074 696d 6573 2e20 4966 2079 6f75  ny times. If you
+00001760: 2069 6e73 7465 6164 2070 6c61 6e20 746f   instead plan to
+00001770: 2072 6567 6973 7465 7220 7468 656d 2077   register them w
+00001780: 6974 6820 610a 5b57 616e 6442 2053 7765  ith a.[WandB Swe
+00001790: 6570 5d28 6874 7470 733a 2f2f 646f 6373  ep](https://docs
+000017a0: 2e77 616e 6462 2e61 692f 6775 6964 6573  .wandb.ai/guides
+000017b0: 2f73 7765 6570 732f 636f 6e66 6967 7572  /sweeps/configur
+000017c0: 6174 696f 6e29 2c20 7765 206e 6565 6420  ation), we need 
+000017d0: 746f 206d 6f64 6966 7920 7468 6520 6073  to modify the `s
+000017e0: 7461 7274 5f66 6e60 2074 6f20 6a6f 696e  tart_fn` to join
+000017f0: 2074 6865 2077 616e 6462 0a73 7765 6570   the wandb.sweep
+00001800: 2e5c 0a42 7920 7061 7463 6869 6e67 2069  .\.By patching i
+00001810: 6e20 7468 6520 636f 6465 2062 656c 6f77  n the code below
+00001820: 2c20 7470 7563 6172 6520 7769 6c6c 2073  , tpucare will s
+00001830: 7461 7274 2061 6e64 206d 6169 6e74 6169  tart and maintai
+00001840: 6e20 6120 6c61 7267 6520 7377 6172 6d20  n a large swarm 
+00001850: 6f66 2054 5055 7320 616c 6c20 776f 726b  of TPUs all work
+00001860: 696e 6720 746f 7761 7264 7320 7468 6520  ing towards the 
+00001870: 7361 6d65 0a68 7970 6572 7061 7261 6d65  same.hyperparame
+00001880: 7465 7220 6f70 7469 6d69 7a61 7469 6f6e  ter optimization
+00001890: 2070 726f 626c 656d 2e0a 0a60 6060 5059   problem...```PY
+000018a0: 5448 4f4e 0a69 6d70 6f72 7420 7761 6e64  THON.import wand
+000018b0: 620a 0a77 6974 6820 6f70 656e 2822 7377  b..with open("sw
+000018c0: 6565 702e 7961 6d6c 222c 2027 7227 2920  eep.yaml", 'r') 
+000018d0: 6173 2066 3a20 2023 2073 7765 6570 2063  as f:  # sweep c
+000018e0: 6f6e 6669 6720 7061 7373 6564 2073 7472  onfig passed str
+000018f0: 6169 6768 7420 746f 2077 616e 6462 0a20  aight to wandb. 
+00001900: 2020 2063 6f6e 6669 6720 3d20 7961 6d6c     config = yaml
+00001910: 2e73 6166 655f 6c6f 6164 2866 2e72 6561  .safe_load(f.rea
+00001920: 6428 2929 0a73 7765 6570 5f69 6420 3d20  d()).sweep_id = 
+00001930: 7761 6e64 622e 7377 6565 7028 636f 6e66  wandb.sweep(conf
+00001940: 6967 2c20 656e 7469 7479 3d22 686f 6d65  ig, entity="home
+00001950: 6272 6577 6e6c 7022 2c20 7072 6f6a 6563  brewnlp", projec
+00001960: 743d 2267 7074 2229 0a0a 0a64 6566 2073  t="gpt")...def s
+00001970: 7461 7274 5f66 6e28 6374 783a 2043 6f6e  tart_fn(ctx: Con
+00001980: 7465 7874 2c20 776f 726b 6572 3a20 696e  text, worker: in
+00001990: 7429 3a0a 2020 2020 636d 6420 3d20 6578  t):.    cmd = ex
+000019a0: 6563 5f63 6f6d 6d61 6e64 2872 6570 6f73  ec_command(repos
+000019b0: 6974 6f72 793d 2268 7474 7073 3a2f 2f67  itory="https://g
+000019c0: 6974 6875 622e 636f 6d2f 486f 6d65 6272  ithub.com/Homebr
+000019d0: 6577 4e4c 502f 486f 6d65 6272 6577 4e4c  ewNLP/HomebrewNL
+000019e0: 502d 4a61 7822 2c20 7761 6e64 625f 6b65  P-Jax", wandb_ke
+000019f0: 793d 7761 6e64 625f 6b65 792c 0a20 2020  y=wandb_key,.   
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 2020 2020 7275 6e5f 636f 6d6d 616e 643d      run_command=
+00001a20: 6622 2f68 6f6d 652f 7562 756e 7475 2f2e  f"/home/ubuntu/.
+00001a30: 6c6f 6361 6c2f 6269 6e2f 7761 6e64 6220  local/bin/wandb 
+00001a40: 6167 656e 7420 7b73 7765 6570 5f69 647d  agent {sweep_id}
+00001a50: 2229 0a20 2020 2073 656e 645f 746f 5f74  ").    send_to_t
+00001a60: 7075 2848 4f53 542c 205a 4f4e 452c 2022  pu(HOST, ZONE, "
+00001a70: 7365 7475 702e 7368 222c 2063 6d64 2c20  setup.sh", cmd, 
+00001a80: 776f 726b 6572 290a 2020 2020 6578 6563  worker).    exec
+00001a90: 5f6f 6e5f 7470 7528 484f 5354 2c20 5a4f  _on_tpu(HOST, ZO
+00001aa0: 4e45 2c20 2262 6173 6820 7365 7475 702e  NE, "bash setup.
+00001ab0: 7368 222c 2077 6f72 6b65 7229 0a60 6060  sh", worker).```
+00001ac0: 0a0a 5468 6520 6675 6c6c 2065 7865 6375  ..The full execu
+00001ad0: 7461 626c 6520 636f 6465 2063 616e 2062  table code can b
+00001ae0: 6520 666f 756e 640a 696e 205b 6578 616d  e found.in [exam
+00001af0: 706c 6573 2f73 7765 6570 2e70 795d 2868  ples/sweep.py](h
+00001b00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001b10: 6d2f 636c 6173 686c 756b 652f 7470 7563  m/clashluke/tpuc
+00001b20: 6172 652f 626c 6f62 2f6d 6169 6e2f 6578  are/blob/main/ex
+00001b30: 616d 706c 6573 2f73 7765 6570 2e70 7929  amples/sweep.py)
+00001b40: 2e0a 0a53 696d 696c 6172 6c79 2c20 7468  ...Similarly, th
+00001b50: 6520 6073 7461 7274 5f66 6e60 2063 6f75  e `start_fn` cou
+00001b60: 6c64 2062 6520 6164 6170 7465 6420 746f  ld be adapted to
+00001b70: 2073 7461 7274 2061 6e20 696e 6665 7265   start an infere
+00001b80: 6e63 6520 7365 7276 6572 0a66 6f72 205b  nce server.for [
+00001b90: 486f 6d65 6272 6577 4e4c 505d 2868 7474  HomebrewNLP](htt
+00001ba0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001bb0: 486f 6d65 6272 6577 4e4c 502f 486f 6d65  HomebrewNLP/Home
+00001bc0: 6272 6577 4e4c 502d 4a61 782f 290a 6f72  brewNLP-Jax/).or
+00001bd0: 205b 4372 6169 796f 6e5d 2868 7474 7073   [Craiyon](https
+00001be0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00001bf0: 6f2f 7370 6163 6573 2f64 616c 6c65 2d6d  o/spaces/dalle-m
+00001c00: 696e 692f 6461 6c6c 652d 6d69 6e69 2920  ini/dalle-mini) 
+00001c10: 6f72 2065 7665 6e20 6578 6563 7574 6520  or even execute 
+00001c20: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+00001c30: 2075 6e69 742d 7465 7374 7320 696e 0a70   unit-tests in.p
+00001c40: 6172 616c 6c65 6c2e 0a0a 2323 2043 6974  arallel...## Cit
+00001c50: 6174 696f 6e0a 0a60 6060 4249 4254 4558  ation..```BIBTEX
+00001c60: 0a40 736f 6674 7761 7265 7b6e 6573 746c  .@software{nestl
+00001c70: 6572 5f6c 7563 6173 5f32 3032 325f 3638  er_lucas_2022_68
+00001c80: 3337 3331 322c 0a20 2061 7574 686f 7220  37312,.  author 
+00001c90: 2020 2020 2020 3d20 7b4e 6573 746c 6572        = {Nestler
+00001ca0: 2c20 4c75 6361 737d 2c0a 2020 7469 746c  , Lucas},.  titl
+00001cb0: 6520 2020 2020 2020 203d 207b 5450 5520  e        = {TPU 
+00001cc0: 4361 7265 7d2c 0a20 206d 6f6e 7468 2020  Care},.  month  
+00001cd0: 2020 2020 2020 3d20 6a75 6c2c 0a20 2079        = jul,.  y
+00001ce0: 6561 7220 2020 2020 2020 2020 3d20 3230  ear         = 20
+00001cf0: 3232 2c0a 2020 7075 626c 6973 6865 7220  22,.  publisher 
+00001d00: 2020 203d 207b 5a65 6e6f 646f 7d2c 0a20     = {Zenodo},. 
+00001d10: 2076 6572 7369 6f6e 2020 2020 2020 3d20   version      = 
+00001d20: 7b30 2e30 2e32 7d2c 0a20 2064 6f69 2020  {0.0.2},.  doi  
+00001d30: 2020 2020 2020 2020 3d20 7b31 302e 3532          = {10.52
+00001d40: 3831 2f7a 656e 6f64 6f2e 3638 3337 3331  81/zenodo.683731
+00001d50: 327d 2c0a 2020 7572 6c20 2020 2020 2020  2},.  url       
+00001d60: 2020 203d 207b 6874 7470 733a 2f2f 646f     = {https://do
+00001d70: 692e 6f72 672f 3130 2e35 3238 312f 7a65  i.org/10.5281/ze
+00001d80: 6e6f 646f 2e36 3833 3733 3132 7d0a 7d60  nodo.6837312}.}`
+00001d90: 6060                                     ``
```

### Comparing `tpucare-0.4.0/setup.py` & `tpucare-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import setuptools
-
-
-with open('README.md') as f:
-    README = f.read()
-
-setuptools.setup(
-    author="Lucas Nestler",
-    author_email="github.tpucare@nestler.sh",
-    name='tpucare',
-    license='BSD',
-    description='Automatically take good care of your preemptible TPUs',
-    version='0.4.0',
-    long_description=README,
-    url='https://github.com/clashluke/tpucare',
-    packages=setuptools.find_packages(),
-    python_requires=">=3.7",
-    long_description_content_type="text/markdown",
-    install_requires=[],
-    classifiers=[
-        # Trove classifiers
-        # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Intended Audience :: Developers',
-    ],
-)
+import setuptools
+
+
+with open('README.md') as f:
+    README = f.read()
+
+setuptools.setup(
+    author="Lucas Nestler",
+    author_email="github.tpucare@nestler.sh",
+    name='tpucare',
+    license='BSD',
+    description='Automatically take good care of your preemptible TPUs',
+    version='0.4.1',
+    long_description=README,
+    url='https://github.com/clashluke/tpucare',
+    packages=setuptools.find_packages(),
+    python_requires=">=3.7",
+    long_description_content_type="text/markdown",
+    install_requires=[],
+    classifiers=[
+        # Trove classifiers
+        # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: BSD License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Intended Audience :: Developers',
+    ],
+)
```

### Comparing `tpucare-0.4.0/tpucare/__init__.py` & `tpucare-0.4.1/tpucare/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-import datetime
-import json
-import logging
-import multiprocessing
-import os
-import signal
-import subprocess
-import tempfile
-import threading
-import time
-import types
-import typing
-from contextlib import nullcontext
-
-
-def call(cmd: str) -> str:
-    return subprocess.check_output(cmd.split()).rstrip().decode()
-
-
-class CallReturnError(ValueError):
-    pass
-
-
-def retry_call(cmd: typing.List[str], retries: int = -2):
-    while retries != -1:
-        ret = subprocess.run(cmd, capture_output=True)
-        out = ret.stdout.rstrip().decode()
-        if not ret.returncode:
-            return out
-    raise ValueError
-
-
-PROJECT = call("gcloud config get project")
-TPU_CMD = "gcloud alpha compute tpus tpu-vm"
-GLOBAL_DICT = {}
-CACHE_TIME = 10
-LOG_LEVEL = logging.INFO
-Context = typing.TypeVar("Context")
-All = typing.Literal["all"]
-SliceIndex = typing.Union[All, int]
-
-
-def log(*message, log_level=1e9):
-    if log_level > LOG_LEVEL:
-        print(f'{datetime.datetime.now()} | {" ".join(map(str, message))}', flush=True)
-
-
-def exec_command(repository: str, wandb_key: typing.Optional[str] = None, branch: str = "main",
-                 setup_command: str = "(bash setup.sh; exit 0)", run_command: str = "bash run.sh",
-                 install_python: bool = True):
-    path = repository.split('/')[-1]
-    if path.endswith('.git'):
-        path = path[:-len('.git')]
-    script = []
-    if install_python:
-        script.append("sudo apt-get -o DPkg::Lock::Timeout=-1 update")
-        script.append("sudo apt-get -o DPkg::Lock::Timeout=-1 --fix-missing --fix-broken install -y git python3 "
-                      "python3-pip")
-    script.append(f"(rm -rf {path} ; pkill -f python3 ; exit 0)")
-    script.append(f"git clone --depth 1 --branch {branch} {repository}")
-    script.append(f"cd {path}")
-    if wandb_key is not None:
-        script.append("python3 -m pip install wandb")
-        script.append(f"/home/ubuntu/.local/bin/wandb login {wandb_key}")
-    script.extend([setup_command, f'screen -dmS model bash -c "cd {path} ; {run_command}"'])
-    return ' && '.join(script)
-
-
-def retry_delete(host: str, zone: str, cmd: typing.List[str], retries: int = -2):
-    try:
-        return retry_call(cmd, retries)
-    except CallReturnError:
-        delete_one_tpu(host, host, zone)
-        return ""
-
-
-def send_to_tpu(host: str, zone: str, filename_on_tpu: str, command: str, worker: SliceIndex = 0):
-    with tempfile.NamedTemporaryFile(mode='w+') as f:
-        f.write(command)
-        f.flush()
-        cmd = TPU_CMD.split(' ') + ["scp", f.name, f"ubuntu@{host}:~/{filename_on_tpu}", "--zone", zone, "--worker",
-                                    str(worker)]
-        retry_delete(host, zone, cmd, 4)
-
-
-def exec_on_tpu(host: str, zone: str, command: str, worker: SliceIndex = 0) -> str:
-    log(f"running '{command}' ...", log_level=logging.DEBUG)
-    start_time = time.time()
-    cmd = TPU_CMD.split(' ') + ["ssh", f"ubuntu@{host}", f"--zone", zone, "--command", command, "--worker", str(worker)]
-    out = retry_delete(host, zone, cmd, 2)
-    log(f"Finished running '{command}' after {time.time() - start_time:.1f}s", log_level=logging.DEBUG)
-    return out
-
-
-def all_tpus(zone: str):
-    zone = 'projects/' + PROJECT + '/locations/' + zone
-    if GLOBAL_DICT.get(f"last_write_{zone}", 0) < time.time() - CACHE_TIME:
-        GLOBAL_DICT[f"last_write_{zone}"] = time.time()
-        GLOBAL_DICT[f"tpus_{zone}"] = json.loads(call(f"{TPU_CMD} list --zone {zone} --format json"))
-    return GLOBAL_DICT[f"tpus_{zone}"]
-
-
-def valid_tpu(tpu: dict, preempted: bool = True, deleting: bool = False, unhealthy: bool = True) -> bool:
-    state = "state" in tpu and (deleting or tpu['state'] != "DELETING") and (preempted or tpu['state'] != "PREEMPTED")
-    state |= deleting and preempted
-    healthy = "health" in tpu and (unhealthy or tpu["health"] == "HEALTHY")
-    healthy |= unhealthy
-    return state and healthy
-
-
-def tpu_names(zone: str, preempted: bool = True, deleting: bool = False, unhealthy: bool = False,
-              no_filter: bool = False, prefix: str = ''):
-    while True:
-        try:
-            tpus = all_tpus(zone)
-            if no_filter:
-                tpus = [t['name'].split('/')[-1] for t in tpus]
-            else:
-                tpus = [t['name'].split('/')[-1] for t in tpus if valid_tpu(t, preempted, deleting, unhealthy)]
-            return [t for t in tpus if t.startswith(prefix)]
-        except KeyboardInterrupt as exc:
-            raise exc
-        except:
-            pass
-
-
-def delete_no_check(host: str, zone: str, asynchronous: bool):
-    os.system(f"echo y | {TPU_CMD} delete {host} --zone {zone} {'--async' * asynchronous}")
-
-
-def tpu_ips(host: str, zone: str) -> typing.List[str]:
-    out = call(f"{TPU_CMD} describe {host} --format json --zone {zone}")
-    return [host["accessConfig"]["externalIp"] for host in json.loads(out)["networkEndpoints"]]
-
-
-def delete_one_tpu(prefix: str, host: str, zone: str, asynchronous: bool = True):
-    if prefix not in host or host not in tpu_names(zone, no_filter=True):
-        return
-    log(f"\x1b[32;1m  DELETING {host}\x1b[0m", log_level=logging.INFO)
-    delete_no_check(host, zone, asynchronous)
-    while not asynchronous and host in tpu_names(zone, no_filter=True):
-        delete_no_check(host, zone, asynchronous)
-
-
-def delete_all(prefix: str, zone: str):
-    while tpu_names(zone, prefix=prefix, no_filter=True):
-        threads = [threading.Thread(target=delete_one_tpu, args=(prefix, host, zone, False), daemon=True) for host in
-                   tpu_names(zone, prefix=prefix)]
-        for t in threads:
-            t.start()
-        for t in threads:
-            t.join()
-
-
-def create_tpu(host: str, zone: str, tpu_version: int, preemptible: bool, service_account: str,
-               semaphore: typing.Optional[typing.ContextManager], slices: int = 1):
-    with semaphore:
-        os.system(f'while ! gcloud alpha compute tpus tpu-vm create {host} --service-account {service_account} '
-                  f'--zone {zone} --accelerator-type v{tpu_version}-{slices * 8} --version v2-alpha '
-                  f'{"--preemptible" * preemptible}; do echo; done')
-
-
-def recreate(host: str, zone: str, tpu_version: int, preemptible: bool, service_account: str, slices: int,
-             creation_semaphore: typing.Optional[typing.ContextManager] = None):
-    delete_one_tpu("", host, zone, False)
-    create_tpu(host, zone, tpu_version, preemptible, service_account, creation_semaphore, slices)
-
-
-def get_name(fn: typing.Callable, base: str):
-    if hasattr(fn, '__name__'):
-        return f"{base} ({fn.__name__})"
-    if not isinstance(fn, types.FunctionType):
-        return get_name(type(fn), base)
-    return base
-
-
-def start_single(host: str, tpu_version: int, zone: str, preemptible: bool, service_account: str, slices: int,
-                 start_fn: typing.Callable[[Context, SliceIndex], None],
-                 creation_callback: typing.Callable[[str, typing.Optional[Context]], Context],
-                 creation_semaphore: typing.Optional[typing.ContextManager] = None, all_workers: bool = False):
-    if creation_semaphore is None:
-        creation_semaphore = nullcontext()
-
-    ctx = None
-
-    creation_callback_name = get_name(creation_callback, "creation_callback")
-    start_fn_name = get_name(start_fn, "start_fn")
-
-    while True:
-        try:
-            log("Recreating TPU", log_level=logging.DEBUG)
-            recreate(host, zone, tpu_version, preemptible, service_account, slices, creation_semaphore)
-            log(f"TPU Created. Calling {creation_callback_name}.", log_level=logging.INFO)
-            ctx = creation_callback(host, ctx)
-            log(f"Callback returned. Launching {start_fn_name}", log_level=logging.DEBUG)
-            if all_workers:
-                threads = [multiprocessing.Process(target=start_fn, args=(ctx, "all"), daemon=True)]
-            else:
-                threads = [multiprocessing.Process(target=start_fn, args=(ctx, i), daemon=True) for i in range(slices)]
-            for t in threads:
-                t.start()
-            log("Started start_fn. Babysitting TPU..", log_level=logging.INFO)
-            unhealthy_timeout = 600 / CACHE_TIME  # sometimes "unhealthy" resolves itself. Let's wait up to 10 minutes
-            while host in tpu_names(zone, preempted=False, unhealthy=True):
-                if unhealthy_timeout <= 0:
-                    break
-                time.sleep(CACHE_TIME)
-                if host in tpu_names(zone, preempted=False, unhealthy=False):
-                    unhealthy_timeout = 600 / CACHE_TIME
-                else:
-                    unhealthy_timeout -= 1
-            log(f"TPU is {'unhealthy' if unhealthy_timeout <= 0 else 'preempted'}. Recreating it now.",
-                log_level=logging.INFO)
-            while any(t.is_alive() for t in threads):
-                for t in threads:
-                    if t.is_alive():
-                        os.kill(t.pid, signal.SIGINT)
-                time.sleep(0.1)
-            log("Sent SIGINT to all workers", log_level=logging.INFO)
-        except KeyboardInterrupt:
-            log(f"{host} - {datetime.datetime.now()}: KeyboardInterrupt received. Killing TPU, then self.",
-                log_level=logging.WARN)
-            delete_one_tpu("", host, zone, False)
-            return
-
-
-def start_multiple(prefix: str, tpu_version: int, zone: str, preemptible: bool, service_account: str, slices: int,
-                   start_fn: typing.Callable[[typing.Any, int], None],
-                   created_callback: typing.Callable[[typing.Any], typing.Any], tpus: int):
-    procs = []
-    creation_semaphore = threading.Semaphore(2)
-    for tpu_id in range(tpus):
-        proc = threading.Thread(target=start_single, daemon=True, args=(
-                f'{prefix}-{tpu_id}', tpu_version, zone, preemptible, service_account, slices, start_fn,
-                created_callback, creation_semaphore))
-        proc.start()
-        procs.append(proc)
-    while all(t.is_alive() for t in procs):
-        try:
-            time.sleep(10)
-        except KeyboardInterrupt:
-            log(f"MAIN - {datetime.datetime.now()}: KeyboardInterrupt received. Killing All TPUs, then self.",
-                logging.WARN)
-            delete_all(prefix, zone)
-            return
+import datetime
+import json
+import logging
+import multiprocessing
+import os
+import signal
+import subprocess
+import tempfile
+import threading
+import time
+import types
+import typing
+from contextlib import nullcontext
+
+
+def call(cmd: str) -> str:
+    return subprocess.check_output(cmd.split()).rstrip().decode()
+
+
+class CallReturnError(ValueError):
+    pass
+
+
+def retry_call(cmd: typing.List[str], retries: int = -2):
+    while retries != -1:
+        ret = subprocess.run(cmd, capture_output=True)
+        out = ret.stdout.rstrip().decode()
+        if not ret.returncode:
+            return out
+    raise ValueError
+
+
+PROJECT = call("gcloud config get project")
+TPU_CMD = "gcloud alpha compute tpus tpu-vm"
+GLOBAL_DICT = {}
+CACHE_TIME = 10
+LOG_LEVEL = logging.INFO
+Context = typing.TypeVar("Context")
+All = typing.Literal["all"]
+SliceIndex = typing.Union[All, int]
+
+
+def log(*message, log_level=1e9):
+    if log_level > LOG_LEVEL:
+        print(f'{datetime.datetime.now()} | {" ".join(map(str, message))}', flush=True)
+
+
+def exec_command(repository: str, wandb_key: typing.Optional[str] = None, branch: str = "main",
+                 setup_command: str = "(bash setup.sh; exit 0)", run_command: str = "bash run.sh",
+                 install_python: bool = True):
+    path = repository.split('/')[-1]
+    if path.endswith('.git'):
+        path = path[:-len('.git')]
+    script = []
+    if install_python:
+        script.append("sudo apt-get -o DPkg::Lock::Timeout=-1 update")
+        script.append("sudo apt-get -o DPkg::Lock::Timeout=-1 --fix-missing --fix-broken install -y git python3 "
+                      "python3-pip")
+    script.append(f"(rm -rf {path} ; pkill -f python3 ; exit 0)")
+    script.append(f"git clone --depth 1 --branch {branch} {repository}")
+    script.append(f"cd {path}")
+    if wandb_key is not None:
+        script.append("python3 -m pip install wandb")
+        script.append(f"/home/ubuntu/.local/bin/wandb login {wandb_key}")
+    script.extend([setup_command, f'screen -dmS model bash -c "cd {path} ; {run_command}"'])
+    return ' &&\\\n'.join(script)
+
+
+def retry_delete(host: str, zone: str, cmd: typing.List[str], retries: int = -2):
+    try:
+        return retry_call(cmd, retries)
+    except CallReturnError:
+        delete_one_tpu(host, host, zone)
+        return ""
+
+
+def send_to_tpu(host: str, zone: str, filename_on_tpu: str, command: str, worker: SliceIndex = 0):
+    with tempfile.NamedTemporaryFile(mode='w+') as f:
+        f.write(command)
+        f.flush()
+        cmd = TPU_CMD.split(' ') + ["scp", f.name, f"ubuntu@{host}:~/{filename_on_tpu}", "--zone", zone, "--worker",
+                                    str(worker)]
+        retry_delete(host, zone, cmd, 4)
+
+
+def exec_on_tpu(host: str, zone: str, command: str, worker: SliceIndex = 0) -> str:
+    log(f"running '{command}' ...", log_level=logging.DEBUG)
+    start_time = time.time()
+    cmd = TPU_CMD.split(' ') + ["ssh", f"ubuntu@{host}", f"--zone", zone, "--command", command, "--worker", str(worker)]
+    out = retry_delete(host, zone, cmd, 2)
+    log(f"Finished running '{command}' after {time.time() - start_time:.1f}s", log_level=logging.DEBUG)
+    return out
+
+
+def all_tpus(zone: str):
+    zone = 'projects/' + PROJECT + '/locations/' + zone
+    if GLOBAL_DICT.get(f"last_write_{zone}", 0) < time.time() - CACHE_TIME:
+        GLOBAL_DICT[f"last_write_{zone}"] = time.time()
+        GLOBAL_DICT[f"tpus_{zone}"] = json.loads(call(f"{TPU_CMD} list --zone {zone} --format json"))
+    return GLOBAL_DICT[f"tpus_{zone}"]
+
+
+def valid_tpu(tpu: dict, preempted: bool = True, deleting: bool = False, unhealthy: bool = True) -> bool:
+    state = "state" in tpu and (deleting or tpu['state'] != "DELETING") and (preempted or tpu['state'] != "PREEMPTED")
+    state |= deleting and preempted
+    healthy = "health" in tpu and (unhealthy or tpu["health"] == "HEALTHY")
+    healthy |= unhealthy
+    return state and healthy
+
+
+def tpu_names(zone: str, preempted: bool = True, deleting: bool = False, unhealthy: bool = False,
+              no_filter: bool = False, prefix: str = ''):
+    while True:
+        try:
+            tpus = all_tpus(zone)
+            if no_filter:
+                tpus = [t['name'].split('/')[-1] for t in tpus]
+            else:
+                tpus = [t['name'].split('/')[-1] for t in tpus if valid_tpu(t, preempted, deleting, unhealthy)]
+            return [t for t in tpus if t.startswith(prefix)]
+        except KeyboardInterrupt as exc:
+            raise exc
+        except:
+            pass
+
+
+def delete_no_check(host: str, zone: str, asynchronous: bool):
+    os.system(f"echo y | {TPU_CMD} delete {host} --zone {zone} {'--async' * asynchronous}")
+
+
+def tpu_ips(host: str, zone: str) -> typing.List[str]:
+    out = call(f"{TPU_CMD} describe {host} --format json --zone {zone}")
+    return [host["accessConfig"]["externalIp"] for host in json.loads(out)["networkEndpoints"]]
+
+
+def delete_one_tpu(prefix: str, host: str, zone: str, asynchronous: bool = True):
+    if prefix not in host or host not in tpu_names(zone, no_filter=True):
+        return
+    log(f"\x1b[32;1m  DELETING {host}\x1b[0m", log_level=logging.INFO)
+    delete_no_check(host, zone, asynchronous)
+    while not asynchronous and host in tpu_names(zone, no_filter=True):
+        delete_no_check(host, zone, asynchronous)
+
+
+def delete_all(prefix: str, zone: str):
+    while tpu_names(zone, prefix=prefix, no_filter=True):
+        threads = [threading.Thread(target=delete_one_tpu, args=(prefix, host, zone, False), daemon=True) for host in
+                   tpu_names(zone, prefix=prefix)]
+        for t in threads:
+            t.start()
+        for t in threads:
+            t.join()
+
+
+def create_tpu(host: str, zone: str, tpu_version: int, preemptible: bool, service_account: str,
+               semaphore: typing.Optional[typing.ContextManager], slices: int = 1):
+    with semaphore:
+        os.system(f'while ! gcloud alpha compute tpus tpu-vm create {host} --service-account {service_account} '
+                  f'--zone {zone} --accelerator-type v{tpu_version}-{slices * 8} --version v2-alpha '
+                  f'{"--preemptible" * preemptible}; do echo; done')
+
+
+def recreate(host: str, zone: str, tpu_version: int, preemptible: bool, service_account: str, slices: int,
+             creation_semaphore: typing.Optional[typing.ContextManager] = None):
+    delete_one_tpu("", host, zone, False)
+    create_tpu(host, zone, tpu_version, preemptible, service_account, creation_semaphore, slices)
+
+
+def get_name(fn: typing.Callable, base: str):
+    if hasattr(fn, '__name__'):
+        return f"{base} ({fn.__name__})"
+    if not isinstance(fn, types.FunctionType):
+        return get_name(type(fn), base)
+    return base
+
+
+def start_single(host: str, tpu_version: int, zone: str, preemptible: bool, service_account: str, slices: int,
+                 start_fn: typing.Callable[[Context, SliceIndex], None],
+                 creation_callback: typing.Callable[[str, typing.Optional[Context]], Context],
+                 creation_semaphore: typing.Optional[typing.ContextManager] = None, all_workers: bool = False):
+    if creation_semaphore is None:
+        creation_semaphore = nullcontext()
+
+    ctx = None
+
+    creation_callback_name = get_name(creation_callback, "creation_callback")
+    start_fn_name = get_name(start_fn, "start_fn")
+
+    while True:
+        try:
+            log("Recreating TPU", log_level=logging.DEBUG)
+            recreate(host, zone, tpu_version, preemptible, service_account, slices, creation_semaphore)
+            log(f"TPU Created. Calling {creation_callback_name}.", log_level=logging.INFO)
+            ctx = creation_callback(host, ctx)
+            log(f"Callback returned. Launching {start_fn_name}", log_level=logging.DEBUG)
+            if all_workers:
+                threads = [multiprocessing.Process(target=start_fn, args=(ctx, "all"), daemon=True)]
+            else:
+                threads = [multiprocessing.Process(target=start_fn, args=(ctx, i), daemon=True) for i in range(slices)]
+            for t in threads:
+                t.start()
+            log("Started start_fn. Babysitting TPU..", log_level=logging.INFO)
+            unhealthy_timeout = 600 / CACHE_TIME  # sometimes "unhealthy" resolves itself. Let's wait up to 10 minutes
+            while host in tpu_names(zone, preempted=False, unhealthy=True):
+                if unhealthy_timeout <= 0:
+                    break
+                time.sleep(CACHE_TIME)
+                if host in tpu_names(zone, preempted=False, unhealthy=False):
+                    unhealthy_timeout = 600 / CACHE_TIME
+                else:
+                    unhealthy_timeout -= 1
+            log(f"TPU is {'unhealthy' if unhealthy_timeout <= 0 else 'preempted'}. Recreating it now.",
+                log_level=logging.INFO)
+            while any(t.is_alive() for t in threads):
+                for t in threads:
+                    if t.is_alive():
+                        os.kill(t.pid, signal.SIGINT)
+                time.sleep(0.1)
+            log("Sent SIGINT to all workers", log_level=logging.INFO)
+        except KeyboardInterrupt:
+            log(f"{host} - {datetime.datetime.now()}: KeyboardInterrupt received. Killing TPU, then self.",
+                log_level=logging.WARN)
+            delete_one_tpu("", host, zone, False)
+            return
+
+
+def start_multiple(prefix: str, tpu_version: int, zone: str, preemptible: bool, service_account: str, slices: int,
+                   start_fn: typing.Callable[[typing.Any, int], None],
+                   created_callback: typing.Callable[[typing.Any], typing.Any], tpus: int):
+    procs = []
+    creation_semaphore = threading.Semaphore(2)
+    for tpu_id in range(tpus):
+        proc = threading.Thread(target=start_single, daemon=True, args=(
+                f'{prefix}-{tpu_id}', tpu_version, zone, preemptible, service_account, slices, start_fn,
+                created_callback, creation_semaphore))
+        proc.start()
+        procs.append(proc)
+    while all(t.is_alive() for t in procs):
+        try:
+            time.sleep(10)
+        except KeyboardInterrupt:
+            log(f"MAIN - {datetime.datetime.now()}: KeyboardInterrupt received. Killing All TPUs, then self.",
+                logging.WARN)
+            delete_all(prefix, zone)
+            return
```

### Comparing `tpucare-0.4.0/tpucare.egg-info/PKG-INFO` & `tpucare-0.4.1/tpucare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.0
+Version: 0.4.1
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
@@ -199,8 +198,7 @@
   month        = jul,
   year         = 2022,
   publisher    = {Zenodo},
   version      = {0.0.2},
   doi          = {10.5281/zenodo.6837312},
   url          = {https://doi.org/10.5281/zenodo.6837312}
 }```
-
```

