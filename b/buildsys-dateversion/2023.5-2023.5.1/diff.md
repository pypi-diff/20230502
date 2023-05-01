# Comparing `tmp/buildsys-dateversion-2023.5.tar.gz` & `tmp/buildsys-dateversion-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildsys-dateversion-2023.5.tar", last modified: Mon May  1 23:31:00 2023, max compression
+gzip compressed data, was "buildsys-dateversion-2023.5.1.tar", last modified: Mon May  1 23:41:31 2023, max compression
```

## Comparing `buildsys-dateversion-2023.5.tar` & `buildsys-dateversion-2023.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:31:00.892760 buildsys-dateversion-2023.5/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)    35149 2023-05-01 22:04:41.000000 buildsys-dateversion-2023.5/LICENSE
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       26 2023-05-01 23:30:19.000000 buildsys-dateversion-2023.5/MANIFEST.in
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       87 2023-05-01 23:31:00.892760 buildsys-dateversion-2023.5/PKG-INFO
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       72 2023-05-01 23:30:19.000000 buildsys-dateversion-2023.5/README.md
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      264 2023-05-01 23:28:43.000000 buildsys-dateversion-2023.5/pyproject.toml
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       38 2023-05-01 23:31:00.892760 buildsys-dateversion-2023.5/setup.cfg
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:31:00.890760 buildsys-dateversion-2023.5/src/
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:31:00.891760 buildsys-dateversion-2023.5/src/buildsys_dateversion/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      183 2023-05-01 23:31:00.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion/__init__.py
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:31:00.892760 buildsys-dateversion-2023.5/src/buildsys_dateversion/__pycache__/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      351 2023-05-01 23:30:59.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)    11912 2023-05-01 23:30:59.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)     8943 2023-05-01 23:30:19.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion/_hooks.py
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:31:00.891760 buildsys-dateversion-2023.5/src/buildsys_dateversion.egg-info/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       87 2023-05-01 23:31:00.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion.egg-info/PKG-INFO
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      430 2023-05-01 23:31:00.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion.egg-info/SOURCES.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)        1 2023-05-01 23:31:00.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion.egg-info/dependency_links.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       21 2023-05-01 23:31:00.000000 buildsys-dateversion-2023.5/src/buildsys_dateversion.egg-info/top_level.txt
+drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:41:31.234693 buildsys-dateversion-2023.5.1/
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)    35149 2023-05-01 22:04:41.000000 buildsys-dateversion-2023.5.1/LICENSE
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)       26 2023-05-01 23:30:19.000000 buildsys-dateversion-2023.5.1/MANIFEST.in
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)       89 2023-05-01 23:41:31.234693 buildsys-dateversion-2023.5.1/PKG-INFO
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)       72 2023-05-01 23:30:19.000000 buildsys-dateversion-2023.5.1/README.md
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)      264 2023-05-01 23:28:43.000000 buildsys-dateversion-2023.5.1/pyproject.toml
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)       38 2023-05-01 23:41:31.234693 buildsys-dateversion-2023.5.1/setup.cfg
+drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:41:31.232693 buildsys-dateversion-2023.5.1/src/
+drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:41:31.233693 buildsys-dateversion-2023.5.1/src/buildsys_dateversion/
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)      184 2023-05-01 23:41:31.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion/__init__.py
+drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:41:31.234693 buildsys-dateversion-2023.5.1/src/buildsys_dateversion/__pycache__/
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)      351 2023-05-01 23:41:30.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)    12518 2023-05-01 23:41:30.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)     9209 2023-05-01 23:39:13.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion/_hooks.py
+drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:41:31.233693 buildsys-dateversion-2023.5.1/src/buildsys_dateversion.egg-info/
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)       89 2023-05-01 23:41:31.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion.egg-info/PKG-INFO
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)      430 2023-05-01 23:41:31.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion.egg-info/SOURCES.txt
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)        1 2023-05-01 23:41:31.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion.egg-info/dependency_links.txt
+-rw-r--r--   0 rmcgover (20551) rmcgover (20551)       21 2023-05-01 23:41:31.000000 buildsys-dateversion-2023.5.1/src/buildsys_dateversion.egg-info/top_level.txt
```

### Comparing `buildsys-dateversion-2023.5/LICENSE` & `buildsys-dateversion-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc` & `buildsys-dateversion-2023.5.1/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8b4b5064 (Mon May  1 23:30:19 2023 UTC)
-files sz: 8943
+moddate:  0xa14d5064 (Mon May  1 23:39:13 2023 UTC)
+files sz: 9209
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -12,16 +12,17 @@
       076d085a080100640064016c095a09020065016a0a000000000000000064
       04a6010000ab0100000000000000005a0b650ba00c000000000000000000
       000000000000000000000065016a0d0000000000000000a6010000ab0100
       000000000000000100650ba00e0000000000000000000000000000000000
       000000020065016a0f00000000000000006405a6010000ab010000000000
       000000a6010000ab0100000000000000000100020065026a100000000000
       000000640665026a110000000000000000ac07a6020000ab020000000000
-      0000005a1202004700640884006409a6020000ab0200000000000000005a
-      13640d640a84015a14640e640b84015a15640d640c84015a1664015300
+      0000005a12640865136602640984045a1402004700640a8400640ba60200
+      00ab0200000000000000005a15640f640c84015a166410640d84015a1764
+      0f640e84015a1864015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -99,48 +100,127 @@
                244 LOAD_NAME                2 (re)
                246 LOAD_ATTR               17 (MULTILINE)
                256 KW_NAMES                 7
                258 PRECALL                  2
                262 CALL                     2
                272 STORE_NAME              18 (VERSION_PATTERN)
    
-    20         274 PUSH_NULL
-               276 LOAD_BUILD_CLASS
-               278 LOAD_CONST               8 (<code object DateVersion, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 20>)
-               280 MAKE_FUNCTION            0
-               282 LOAD_CONST               9 ('DateVersion')
-               284 PRECALL                  2
-               288 CALL                     2
-               298 STORE_NAME              19 (DateVersion)
+    20         274 LOAD_CONST               8 ('version')
+               276 LOAD_NAME               19 (str)
+               278 BUILD_TUPLE              2
+               280 LOAD_CONST               9 (<code object normalized, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 20>)
+               282 MAKE_FUNCTION            4 (annotations)
+               284 STORE_NAME              20 (normalized)
    
-   191         300 LOAD_CONST              13 ((None, None))
-               302 LOAD_CONST              10 (<code object build_wheel, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 191>)
-               304 MAKE_FUNCTION            1 (defaults)
-               306 STORE_NAME              20 (build_wheel)
+    28         286 PUSH_NULL
+               288 LOAD_BUILD_CLASS
+               290 LOAD_CONST              10 (<code object DateVersion, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 28>)
+               292 MAKE_FUNCTION            0
+               294 LOAD_CONST              11 ('DateVersion')
+               296 PRECALL                  2
+               300 CALL                     2
+               310 STORE_NAME              21 (DateVersion)
    
-   201         308 LOAD_CONST              14 ((None,))
-               310 LOAD_CONST              11 (<code object build_sdist, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 201>)
-               312 MAKE_FUNCTION            1 (defaults)
-               314 STORE_NAME              21 (build_sdist)
+   199         312 LOAD_CONST              15 ((None, None))
+               314 LOAD_CONST              12 (<code object build_wheel, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 199>)
+               316 MAKE_FUNCTION            1 (defaults)
+               318 STORE_NAME              22 (build_wheel)
    
-   221         316 LOAD_CONST              13 ((None, None))
-               318 LOAD_CONST              12 (<code object build_editable, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 221>)
-               320 MAKE_FUNCTION            1 (defaults)
-               322 STORE_NAME              22 (build_editable)
-               324 LOAD_CONST               1 (None)
-               326 RETURN_VALUE
+   209         320 LOAD_CONST              16 ((None,))
+               322 LOAD_CONST              13 (<code object build_sdist, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 209>)
+               324 MAKE_FUNCTION            1 (defaults)
+               326 STORE_NAME              23 (build_sdist)
+   
+   229         328 LOAD_CONST              15 ((None, None))
+               330 LOAD_CONST              14 (<code object build_editable, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 229>)
+               332 MAKE_FUNCTION            1 (defaults)
+               334 STORE_NAME              24 (build_editable)
+               336 LOAD_CONST               1 (None)
+               338 RETURN_VALUE
    consts
       0
       None
       ('datetime',)
       ('contextmanager',)
       'buildsys-dateversion'
       '/tmp/buildsys-dateversion.log'
       '^__version__ *=.*$'
       ('flags',)
+      'version'
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 6
+         flags     : 3
+         code
+            0x97006401a0000000000000000000000000000000000000000000640284
+            007c00a00100000000000000000000000000000000000000006401a60100
+            00ab0100000000000000004400a6000000ab000000000000000000a60100
+            00ab0100000000000000005300
+          20           0 RESUME                   0
+         
+          25           2 LOAD_CONST               1 ('.')
+                       4 LOAD_METHOD              0 (join)
+                      26 LOAD_CONST               2 (<code object <listcomp>, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 25>)
+                      28 MAKE_FUNCTION            0
+                      30 LOAD_FAST                0 (version)
+                      32 LOAD_METHOD              1 (split)
+                      54 LOAD_CONST               1 ('.')
+                      56 PRECALL                  1
+                      60 CALL                     1
+                      70 GET_ITER
+                      72 PRECALL                  0
+                      76 CALL                     0
+                      86 PRECALL                  1
+                      90 CALL                     1
+                     100 RETURN_VALUE
+         consts
+            None
+            '.'
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 7
+               flags     : 19
+               code
+                  0x970067007c005d1e7d0174010000000000000000000074030000000000
+                  00000000007c01a6010000ab010000000000000000a6010000ab01000000
+                  000000000091028c1f5300
+                25           0 RESUME                   0
+                             2 BUILD_LIST               0
+                             4 LOAD_FAST                0 (.0)
+                       >>    6 FOR_ITER                30 (to 68)
+                             8 STORE_FAST               1 (x)
+                            10 LOAD_GLOBAL              1 (NULL + str)
+                            22 LOAD_GLOBAL              3 (NULL + int)
+                            34 LOAD_FAST                1 (x)
+                            36 PRECALL                  1
+                            40 CALL                     1
+                            50 PRECALL                  1
+                            54 CALL                     1
+                            64 LIST_APPEND              2
+                            66 JUMP_BACKWARD           31 (to 6)
+                       >>   68 RETURN_VALUE
+               consts
+               names      ('str', 'int')
+               varnames   ('.0', 'x')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       '<listcomp>'
+               firstlineno 25
+               lnotab 0x
+         names      ('join', 'split')
+         varnames   ('version',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         name       'normalized'
+         firstlineno 20
+         lnotab 0x0205
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a026412640284015a036504640365056602640484
@@ -148,142 +228,142 @@
             0464036505660264068404a6000000ab0000000000000000005a08650464
             078400a6000000ab0000000000000000005a096504640365056602640884
             04a6000000ab0000000000000000005a0a650464036505660264098404a6
             000000ab0000000000000000005a0b6504640365056602640a8404a60000
             00ab0000000000000000005a0c640365056602640b84045a0d640c650564
             03650e6604640d84045a0f6510640e8400a6000000ab0000000000000000
             005a11640f84005a12641084005a13641184005a1464015300
-          20           0 RESUME                   0
+          28           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DateVersion')
                        8 STORE_NAME               2 (__qualname__)
          
-          21          10 LOAD_CONST              18 ((None,))
-                      12 LOAD_CONST               2 (<code object __init__, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 21>)
+          29          10 LOAD_CONST              18 ((None,))
+                      12 LOAD_CONST               2 (<code object __init__, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 29>)
                       14 MAKE_FUNCTION            1 (defaults)
                       16 STORE_NAME               3 (__init__)
          
-          26          18 LOAD_NAME                4 (property)
+          34          18 LOAD_NAME                4 (property)
          
-          27          20 LOAD_CONST               3 ('return')
+          35          20 LOAD_CONST               3 ('return')
                       22 LOAD_NAME                5 (str)
                       24 BUILD_TUPLE              2
-                      26 LOAD_CONST               4 (<code object marker, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 26>)
+                      26 LOAD_CONST               4 (<code object marker, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 34>)
                       28 MAKE_FUNCTION            4 (annotations)
          
-          26          30 PRECALL                  0
+          34          30 PRECALL                  0
                       34 CALL                     0
          
-          27          44 STORE_NAME               6 (marker)
+          35          44 STORE_NAME               6 (marker)
          
-          30          46 LOAD_CONST               3 ('return')
+          38          46 LOAD_CONST               3 ('return')
                       48 LOAD_NAME                5 (str)
                       50 BUILD_TUPLE              2
-                      52 LOAD_CONST               5 (<code object _find_version_path, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 30>)
+                      52 LOAD_CONST               5 (<code object _find_version_path, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 38>)
                       54 MAKE_FUNCTION            4 (annotations)
                       56 STORE_NAME               7 (_find_version_path)
          
-          45          58 LOAD_NAME                4 (property)
+          53          58 LOAD_NAME                4 (property)
          
-          46          60 LOAD_CONST               3 ('return')
+          54          60 LOAD_CONST               3 ('return')
                       62 LOAD_NAME                5 (str)
                       64 BUILD_TUPLE              2
-                      66 LOAD_CONST               6 (<code object version_path, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 45>)
+                      66 LOAD_CONST               6 (<code object version_path, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 53>)
                       68 MAKE_FUNCTION            4 (annotations)
          
-          45          70 PRECALL                  0
+          53          70 PRECALL                  0
                       74 CALL                     0
          
-          46          84 STORE_NAME               8 (version_path)
+          54          84 STORE_NAME               8 (version_path)
          
-          51          86 LOAD_NAME                4 (property)
+          59          86 LOAD_NAME                4 (property)
          
-          52          88 LOAD_CONST               7 (<code object build_backend, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 51>)
+          60          88 LOAD_CONST               7 (<code object build_backend, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 59>)
                       90 MAKE_FUNCTION            0
          
-          51          92 PRECALL                  0
+          59          92 PRECALL                  0
                       96 CALL                     0
          
-          52         106 STORE_NAME               9 (build_backend)
+          60         106 STORE_NAME               9 (build_backend)
          
-          69         108 LOAD_NAME                4 (property)
+          77         108 LOAD_NAME                4 (property)
          
-          70         110 LOAD_CONST               3 ('return')
+          78         110 LOAD_CONST               3 ('return')
                      112 LOAD_NAME                5 (str)
                      114 BUILD_TUPLE              2
-                     116 LOAD_CONST               8 (<code object index_url, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 69>)
+                     116 LOAD_CONST               8 (<code object index_url, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 77>)
                      118 MAKE_FUNCTION            4 (annotations)
          
-          69         120 PRECALL                  0
+          77         120 PRECALL                  0
                      124 CALL                     0
          
-          70         134 STORE_NAME              10 (index_url)
+          78         134 STORE_NAME              10 (index_url)
          
-          79         136 LOAD_NAME                4 (property)
+          87         136 LOAD_NAME                4 (property)
          
-          80         138 LOAD_CONST               3 ('return')
+          88         138 LOAD_CONST               3 ('return')
                      140 LOAD_NAME                5 (str)
                      142 BUILD_TUPLE              2
-                     144 LOAD_CONST               9 (<code object distribution_name, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 79>)
+                     144 LOAD_CONST               9 (<code object distribution_name, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 87>)
                      146 MAKE_FUNCTION            4 (annotations)
          
-          79         148 PRECALL                  0
+          87         148 PRECALL                  0
                      152 CALL                     0
          
-          80         162 STORE_NAME              11 (distribution_name)
+          88         162 STORE_NAME              11 (distribution_name)
          
-         101         164 LOAD_NAME                4 (property)
+         109         164 LOAD_NAME                4 (property)
          
-         102         166 LOAD_CONST               3 ('return')
+         110         166 LOAD_CONST               3 ('return')
                      168 LOAD_NAME                5 (str)
                      170 BUILD_TUPLE              2
-                     172 LOAD_CONST              10 (<code object version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 101>)
+                     172 LOAD_CONST              10 (<code object version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 109>)
                      174 MAKE_FUNCTION            4 (annotations)
          
-         101         176 PRECALL                  0
+         109         176 PRECALL                  0
                      180 CALL                     0
          
-         102         190 STORE_NAME              12 (version)
+         110         190 STORE_NAME              12 (version)
          
-         109         192 LOAD_CONST               3 ('return')
+         117         192 LOAD_CONST               3 ('return')
                      194 LOAD_NAME                5 (str)
                      196 BUILD_TUPLE              2
-                     198 LOAD_CONST              11 (<code object _get_version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 109>)
+                     198 LOAD_CONST              11 (<code object _get_version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 117>)
                      200 MAKE_FUNCTION            4 (annotations)
                      202 STORE_NAME              13 (_get_version)
          
-         130         204 LOAD_CONST              12 ('candidate_version')
+         138         204 LOAD_CONST              12 ('candidate_version')
                      206 LOAD_NAME                5 (str)
                      208 LOAD_CONST               3 ('return')
                      210 LOAD_NAME               14 (bool)
                      212 BUILD_TUPLE              4
-                     214 LOAD_CONST              13 (<code object version_in_repository, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 130>)
+                     214 LOAD_CONST              13 (<code object version_in_repository, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 138>)
                      216 MAKE_FUNCTION            4 (annotations)
                      218 STORE_NAME              15 (version_in_repository)
          
-         155         220 LOAD_NAME               16 (contextmanager)
+         163         220 LOAD_NAME               16 (contextmanager)
          
-         156         222 LOAD_CONST              14 (<code object patched_version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 155>)
+         164         222 LOAD_CONST              14 (<code object patched_version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 163>)
                      224 MAKE_FUNCTION            0
          
-         155         226 PRECALL                  0
+         163         226 PRECALL                  0
                      230 CALL                     0
          
-         156         240 STORE_NAME              17 (patched_version)
+         164         240 STORE_NAME              17 (patched_version)
          
-         181         242 LOAD_CONST              15 (<code object delegate_build_wheel, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 181>)
+         189         242 LOAD_CONST              15 (<code object delegate_build_wheel, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 189>)
                      244 MAKE_FUNCTION            0
                      246 STORE_NAME              18 (delegate_build_wheel)
          
-         184         248 LOAD_CONST              16 (<code object delegate_build_sdist, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 184>)
+         192         248 LOAD_CONST              16 (<code object delegate_build_sdist, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 192>)
                      250 MAKE_FUNCTION            0
                      252 STORE_NAME              19 (delegate_build_sdist)
          
-         187         254 LOAD_CONST              17 (<code object delegate_build_editable, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 187>)
+         195         254 LOAD_CONST              17 (<code object delegate_build_editable, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 195>)
                      256 MAKE_FUNCTION            0
                      258 STORE_NAME              20 (delegate_build_editable)
                      260 LOAD_CONST               1 (None)
                      262 RETURN_VALUE
          consts
             'DateVersion'
             None
@@ -295,33 +375,33 @@
                code
                   0x97007c0170016900a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007c005f010000000000000000740500
                   0000000000000000006a030000000000000000a6000000ab000000000000
                   0000007c005f020000000000000000740800000000000000000000a00500
                   0000000000000000000000000000000000000064017c006a020000000000
                   000000a6020000ab020000000000000000010064005300
-                21           0 RESUME                   0
+                29           0 RESUME                   0
                
-                22           2 LOAD_FAST                1 (config_settings)
+                30           2 LOAD_FAST                1 (config_settings)
                              4 JUMP_IF_TRUE_OR_POP      1 (to 8)
                              6 BUILD_MAP                0
                        >>    8 LOAD_METHOD              0 (copy)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (config_settings)
                
-                23          56 LOAD_GLOBAL              5 (NULL + datetime)
+                31          56 LOAD_GLOBAL              5 (NULL + datetime)
                             68 LOAD_ATTR                3 (utcnow)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               2 (datetime)
                
-                24         104 LOAD_GLOBAL              8 (LOG)
+                32         104 LOAD_GLOBAL              8 (LOG)
                            116 LOAD_METHOD              5 (debug)
                            138 LOAD_CONST               1 ('operating with datetime = %s')
                            140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                2 (datetime)
                            152 PRECALL                  2
                            156 CALL                     2
                            166 POP_TOP
@@ -332,28 +412,28 @@
                   'operating with datetime = %s'
                names      ('copy', 'config_settings', 'datetime', 'utcnow', 'LOG', 'debug')
                varnames   ('self', 'config_settings')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       '__init__'
-               firstlineno 21
+               firstlineno 29
                lnotab 0x020136013001
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000700164025300
-                26           0 RESUME                   0
+                34           0 RESUME                   0
                
-                28           2 LOAD_FAST                0 (self)
+                36           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (config_settings)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('dateversion-version-marker')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 JUMP_IF_TRUE_OR_POP      1 (to 56)
                             54 LOAD_CONST               2 ('generated by buildsys-dateversion')
@@ -364,15 +444,15 @@
                   'generated by buildsys-dateversion'
                names      ('config_settings', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'marker'
-               firstlineno 26
+               firstlineno 34
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 7
                flags     : 3
                code
@@ -387,92 +467,92 @@
                   000000000000000000000000000000000000007413000000000000000000
                   007c05a6010000ab010000000000000000a00a0000000000000000000000
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   000000000000007221740a00000000000000000000a00b00000000000000
                   0000000000000000000000000064047c05a6020000ab0200000000000000
                   0001007c05630201006302010053008cae8cb77419000000000000000000
                   006405a6010000ab0100000000000000008201
-                30           0 RESUME                   0
+                38           0 RESUME                   0
                
-                31           2 LOAD_GLOBAL              1 (NULL + os)
+                39           2 LOAD_GLOBAL              1 (NULL + os)
                             14 LOAD_ATTR                1 (walk)
                             24 LOAD_CONST               1 ('.')
                             26 PRECALL                  1
                             30 CALL                     1
                             40 GET_ITER
                        >>   42 FOR_ITER               182 (to 408)
                             44 UNPACK_SEQUENCE          3
                             48 STORE_FAST               1 (dirpath)
                             50 STORE_FAST               2 (_)
                             52 STORE_FAST               3 (files)
                
-                32          54 LOAD_FAST                3 (files)
+                40          54 LOAD_FAST                3 (files)
                             56 GET_ITER
                        >>   58 FOR_ITER               173 (to 406)
                             60 STORE_FAST               4 (file)
                
-                33          62 LOAD_FAST                4 (file)
+                41          62 LOAD_FAST                4 (file)
                             64 LOAD_METHOD              2 (endswith)
                             86 LOAD_CONST               2 ('.py')
                             88 PRECALL                  1
                             92 CALL                     1
                            102 POP_JUMP_FORWARD_IF_TRUE     1 (to 106)
                
-                34         104 JUMP_BACKWARD           24 (to 58)
+                42         104 JUMP_BACKWARD           24 (to 58)
                
-                36     >>  106 LOAD_GLOBAL              0 (os)
+                44     >>  106 LOAD_GLOBAL              0 (os)
                            118 LOAD_ATTR                3 (path)
                            128 LOAD_METHOD              4 (join)
                            150 LOAD_FAST                1 (dirpath)
                            152 LOAD_FAST                4 (file)
                            154 PRECALL                  2
                            158 CALL                     2
                            168 STORE_FAST               5 (path)
                
-                37         170 LOAD_GLOBAL             10 (LOG)
+                45         170 LOAD_GLOBAL             10 (LOG)
                            182 LOAD_METHOD              6 (debug)
                            204 LOAD_CONST               3 ('Checking file %s')
                            206 LOAD_FAST                5 (path)
                            208 PRECALL                  2
                            212 CALL                     2
                            222 POP_TOP
                
-                38         224 LOAD_GLOBAL             14 (VERSION_PATTERN)
+                46         224 LOAD_GLOBAL             14 (VERSION_PATTERN)
                            236 LOAD_METHOD              8 (search)
                            258 LOAD_GLOBAL             19 (NULL + open)
                            270 LOAD_FAST                5 (path)
                            272 PRECALL                  1
                            276 CALL                     1
                            286 LOAD_METHOD             10 (read)
                            308 PRECALL                  0
                            312 CALL                     0
                            322 PRECALL                  1
                            326 CALL                     1
                            336 POP_JUMP_FORWARD_IF_FALSE    33 (to 404)
                
-                39         338 LOAD_GLOBAL             10 (LOG)
+                47         338 LOAD_GLOBAL             10 (LOG)
                            350 LOAD_METHOD             11 (info)
                            372 LOAD_CONST               4 ('detected __version__ in %s')
                            374 LOAD_FAST                5 (path)
                            376 PRECALL                  2
                            380 CALL                     2
                            390 POP_TOP
                
-                40         392 LOAD_FAST                5 (path)
+                48         392 LOAD_FAST                5 (path)
                            394 SWAP                     2
                            396 POP_TOP
                            398 SWAP                     2
                            400 POP_TOP
                            402 RETURN_VALUE
                
-                38     >>  404 JUMP_BACKWARD          174 (to 58)
+                46     >>  404 JUMP_BACKWARD          174 (to 58)
                
-                32     >>  406 JUMP_BACKWARD          183 (to 42)
+                40     >>  406 JUMP_BACKWARD          183 (to 42)
                
-                43     >>  408 LOAD_GLOBAL             25 (NULL + RuntimeError)
+                51     >>  408 LOAD_GLOBAL             25 (NULL + RuntimeError)
                            420 LOAD_CONST               5 ('Could not locate a file in the source tree defining `__version__`')
                            422 PRECALL                  1
                            426 CALL                     1
                            436 RAISE_VARARGS            1
                consts
                   None
                   '.'
@@ -482,58 +562,58 @@
                   'Could not locate a file in the source tree defining `__version__`'
                names      ('os', 'walk', 'endswith', 'path', 'join', 'LOG', 'debug', 'VERSION_PATTERN', 'search', 'open', 'read', 'info', 'RuntimeError')
                varnames   ('self', 'dirpath', '_', 'files', 'file', 'path')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       '_find_version_path'
-               firstlineno 30
+               firstlineno 38
                lnotab 0x0201340108012a01020240013601720136010cfe02fa020b
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x970064017c006a0000000000000000007601721c7c00a0010000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
                   006a00000000000000000064013c0000007c006a00000000000000000064
                   01190000000000000000005300
-                45           0 RESUME                   0
+                53           0 RESUME                   0
                
-                47           2 LOAD_CONST               1 ('dateversion-version-path')
+                55           2 LOAD_CONST               1 ('dateversion-version-path')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (config_settings)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE    28 (to 76)
                
-                48          20 LOAD_FAST                0 (self)
+                56          20 LOAD_FAST                0 (self)
                             22 LOAD_METHOD              1 (_find_version_path)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                0 (config_settings)
                             70 LOAD_CONST               1 ('dateversion-version-path')
                             72 STORE_SUBSCR
                
-                49     >>   76 LOAD_FAST                0 (self)
+                57     >>   76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                0 (config_settings)
                             88 LOAD_CONST               1 ('dateversion-version-path')
                             90 BINARY_SUBSCR
                            100 RETURN_VALUE
                consts
                   None
                   'dateversion-version-path'
                names      ('config_settings', '_find_version_path')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'version_path'
-               firstlineno 45
+               firstlineno 53
                lnotab 0x020212013801
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
@@ -545,84 +625,84 @@
                   0000000000a6010000ab0100000000000000007d037c037d04740b000000
                   000000000000007c02a6010000ab01000000000000000064066b02000000
                   007216740d000000000000000000007c037c026407190000000000000000
                   00a6020000ab0200000000000000007d04740e00000000000000000000a0
                   08000000000000000000000000000000000000000064087c017c04a60300
                   00ab03000000000000000001007c047c006a00000000000000000064013c
                   0000007c006a0000000000000000006401190000000000000000005300
-                51           0 RESUME                   0
+                59           0 RESUME                   0
                
-                53           2 LOAD_CONST               1 ('dateversion-build-backend-object')
+                61           2 LOAD_CONST               1 ('dateversion-build-backend-object')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (config_settings)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE   156 (to 332)
                
-                54          20 LOAD_FAST                0 (self)
+                62          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (config_settings)
                             32 LOAD_METHOD              1 (get)
                             54 LOAD_CONST               2 ('dateversion-build-backend')
                             56 PRECALL                  1
                             60 CALL                     1
                             70 JUMP_IF_TRUE_OR_POP      1 (to 74)
                             72 LOAD_CONST               3 ('setuptools.build_meta:__legacy__')
                        >>   74 STORE_FAST               1 (backend_name)
                
-                56          76 LOAD_FAST                1 (backend_name)
+                64          76 LOAD_FAST                1 (backend_name)
                             78 LOAD_METHOD              2 (split)
                            100 LOAD_CONST               4 (':')
                            102 PRECALL                  1
                            106 CALL                     1
                            116 STORE_FAST               2 (components)
                
-                57         118 LOAD_GLOBAL              7 (NULL + importlib)
+                65         118 LOAD_GLOBAL              7 (NULL + importlib)
                            130 LOAD_ATTR                4 (import_module)
                            140 LOAD_FAST                2 (components)
                            142 LOAD_CONST               5 (0)
                            144 BINARY_SUBSCR
                            154 PRECALL                  1
                            158 CALL                     1
                            168 STORE_FAST               3 (module)
                
-                58         170 LOAD_FAST                3 (module)
+                66         170 LOAD_FAST                3 (module)
                            172 STORE_FAST               4 (backend)
                
-                60         174 LOAD_GLOBAL             11 (NULL + len)
+                68         174 LOAD_GLOBAL             11 (NULL + len)
                            186 LOAD_FAST                2 (components)
                            188 PRECALL                  1
                            192 CALL                     1
                            202 LOAD_CONST               6 (2)
                            204 COMPARE_OP               2 (==)
                            210 POP_JUMP_FORWARD_IF_FALSE    22 (to 256)
                
-                61         212 LOAD_GLOBAL             13 (NULL + getattr)
+                69         212 LOAD_GLOBAL             13 (NULL + getattr)
                            224 LOAD_FAST                3 (module)
                            226 LOAD_FAST                2 (components)
                            228 LOAD_CONST               7 (1)
                            230 BINARY_SUBSCR
                            240 PRECALL                  2
                            244 CALL                     2
                            254 STORE_FAST               4 (backend)
                
-                63     >>  256 LOAD_GLOBAL             14 (LOG)
+                71     >>  256 LOAD_GLOBAL             14 (LOG)
                            268 LOAD_METHOD              8 (debug)
                            290 LOAD_CONST               8 ('using build backend %s (%s)')
                            292 LOAD_FAST                1 (backend_name)
                            294 LOAD_FAST                4 (backend)
                            296 PRECALL                  3
                            300 CALL                     3
                            310 POP_TOP
                
-                65         312 LOAD_FAST                4 (backend)
+                73         312 LOAD_FAST                4 (backend)
                            314 LOAD_FAST                0 (self)
                            316 LOAD_ATTR                0 (config_settings)
                            326 LOAD_CONST               1 ('dateversion-build-backend-object')
                            328 STORE_SUBSCR
                
-                67     >>  332 LOAD_FAST                0 (self)
+                75     >>  332 LOAD_FAST                0 (self)
                            334 LOAD_ATTR                0 (config_settings)
                            344 LOAD_CONST               1 ('dateversion-build-backend-object')
                            346 BINARY_SUBSCR
                            356 RETURN_VALUE
                consts
                   None
                   'dateversion-build-backend-object'
@@ -635,78 +715,78 @@
                   'using build backend %s (%s)'
                names      ('config_settings', 'get', 'split', 'importlib', 'import_module', 'len', 'getattr', 'LOG', 'debug')
                varnames   ('self', 'backend_name', 'components', 'module', 'backend')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'build_backend'
-               firstlineno 51
+               firstlineno 59
                lnotab 0x0202120138022a013401040226012c0238021402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000700164027d017c
                   01a00200000000000000000000000000000000000000006403a6010000ab
                   010000000000000000721f7c01640064048502190000000000000000007d
                   017c01a00200000000000000000000000000000000000000006403a60100
                   00ab010000000000000000b01f7c015300
-                69           0 RESUME                   0
+                77           0 RESUME                   0
                
-                72           2 LOAD_FAST                0 (self)
+                80           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (config_settings)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('dateversion-index-url')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 JUMP_IF_TRUE_OR_POP      1 (to 56)
                
-                73          54 LOAD_CONST               2 ('https://pypi.org/simple')
+                81          54 LOAD_CONST               2 ('https://pypi.org/simple')
                
-                71     >>   56 STORE_FAST               1 (out)
+                79     >>   56 STORE_FAST               1 (out)
                
-                75          58 LOAD_FAST                1 (out)
+                83          58 LOAD_FAST                1 (out)
                             60 LOAD_METHOD              2 (endswith)
                             82 LOAD_CONST               3 ('/')
                             84 PRECALL                  1
                             88 CALL                     1
                             98 POP_JUMP_FORWARD_IF_FALSE    31 (to 162)
                
-                76     >>  100 LOAD_FAST                1 (out)
+                84     >>  100 LOAD_FAST                1 (out)
                            102 LOAD_CONST               0 (None)
                            104 LOAD_CONST               4 (-1)
                            106 BUILD_SLICE              2
                            108 BINARY_SUBSCR
                            118 STORE_FAST               1 (out)
                
-                75         120 LOAD_FAST                1 (out)
+                83         120 LOAD_FAST                1 (out)
                            122 LOAD_METHOD              2 (endswith)
                            144 LOAD_CONST               3 ('/')
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_JUMP_BACKWARD_IF_TRUE    31 (to 100)
                
-                77     >>  162 LOAD_FAST                1 (out)
+                85     >>  162 LOAD_FAST                1 (out)
                            164 RETURN_VALUE
                consts
                   None
                   'dateversion-index-url'
                   'https://pypi.org/simple'
                   '/'
                   -1
                names      ('config_settings', 'get', 'endswith')
                varnames   ('self', 'out')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'index_url'
-               firstlineno 69
+               firstlineno 77
                lnotab 0x0203340102fe02042a0114ff2a02
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
@@ -717,59 +797,59 @@
                   0100000000000000007d03640064006400a6020000ab0200000000000000
                   0001006e0b23003100730477027803590077010100590001000100740a00
                   000000000000000000a00600000000000000000000000000000000000000
                   0064057c03a6020000ab02000000000000000001007c0364061900000000
                   00000000006407190000000000000000007c006a00000000000000000064
                   013c0000007c006a00000000000000000064011900000000000000000053
                   00
-                79           0 RESUME                   0
+                87           0 RESUME                   0
                
-                81           2 LOAD_CONST               1 ('dateversion-distribution-name')
+                89           2 LOAD_CONST               1 ('dateversion-distribution-name')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (config_settings)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE   127 (to 274)
                
-                83          20 NOP
+                91          20 NOP
                
-                84          22 LOAD_CONST               2 (0)
+                92          22 LOAD_CONST               2 (0)
                             24 LOAD_CONST               0 (None)
                             26 IMPORT_NAME              1 (tomllib)
                             28 STORE_FAST               1 (tomllib)
                             30 JUMP_FORWARD            11 (to 54)
                        >>   32 PUSH_EXC_INFO
                
-                85          34 POP_TOP
+                93          34 POP_TOP
                
-                87          36 LOAD_CONST               2 (0)
+                95          36 LOAD_CONST               2 (0)
                             38 LOAD_CONST               0 (None)
                             40 IMPORT_NAME              2 (tomli)
                             42 STORE_FAST               1 (tomllib)
                             44 POP_EXCEPT
                             46 JUMP_FORWARD             3 (to 54)
                        >>   48 COPY                     3
                             50 POP_EXCEPT
                             52 RERAISE                  1
                
-                89     >>   54 LOAD_GLOBAL              7 (NULL + open)
+                97     >>   54 LOAD_GLOBAL              7 (NULL + open)
                             66 LOAD_CONST               3 ('pyproject.toml')
                             68 LOAD_CONST               4 ('rb')
                             70 PRECALL                  2
                             74 CALL                     2
                             84 BEFORE_WITH
                             86 STORE_FAST               2 (f)
                
-                90          88 LOAD_FAST                1 (tomllib)
+                98          88 LOAD_FAST                1 (tomllib)
                             90 LOAD_METHOD              4 (load)
                            112 LOAD_FAST                2 (f)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 STORE_FAST               3 (data)
                
-                89         130 LOAD_CONST               0 (None)
+                97         130 LOAD_CONST               0 (None)
                            132 LOAD_CONST               0 (None)
                            134 LOAD_CONST               0 (None)
                            136 PRECALL                  2
                            140 CALL                     2
                            150 POP_TOP
                            152 JUMP_FORWARD            11 (to 176)
                        >>  154 PUSH_EXC_INFO
@@ -780,36 +860,36 @@
                            164 POP_EXCEPT
                            166 RERAISE                  1
                        >>  168 POP_TOP
                            170 POP_EXCEPT
                            172 POP_TOP
                            174 POP_TOP
                
-                92     >>  176 LOAD_GLOBAL             10 (LOG)
+               100     >>  176 LOAD_GLOBAL             10 (LOG)
                            188 LOAD_METHOD              6 (info)
                            210 LOAD_CONST               5 ('Loaded project metadata: %s')
                            212 LOAD_FAST                3 (data)
                            214 PRECALL                  2
                            218 CALL                     2
                            228 POP_TOP
                
-                97         230 LOAD_FAST                3 (data)
+               105         230 LOAD_FAST                3 (data)
                            232 LOAD_CONST               6 ('project')
                            234 BINARY_SUBSCR
                            244 LOAD_CONST               7 ('name')
                            246 BINARY_SUBSCR
                
-                95         256 LOAD_FAST                0 (self)
+               103         256 LOAD_FAST                0 (self)
                            258 LOAD_ATTR                0 (config_settings)
                
-                96         268 LOAD_CONST               1 ('dateversion-distribution-name')
+               104         268 LOAD_CONST               1 ('dateversion-distribution-name')
                
-                95         270 STORE_SUBSCR
+               103         270 STORE_SUBSCR
                
-                99     >>  274 LOAD_FAST                0 (self)
+               107     >>  274 LOAD_FAST                0 (self)
                            276 LOAD_ATTR                0 (config_settings)
                            286 LOAD_CONST               1 ('dateversion-distribution-name')
                            288 BINARY_SUBSCR
                            298 RETURN_VALUE
                ExceptionTable:
                  22 to 28 -> 32 [0]
                  32 to 42 -> 48 [1] lasti
@@ -827,142 +907,150 @@
                   'name'
                names      ('config_settings', 'tomllib', 'tomli', 'open', 'load', 'LOG', 'info')
                varnames   ('self', 'tomllib', 'f', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'distribution_name'
-               firstlineno 79
+               firstlineno 87
                lnotab 0x0202120202010c010202120222012aff2e0336051afe0c0102ff0404
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x970064017c006a0000000000000000007601721c7c00a0010000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
                   006a00000000000000000064013c0000007c006a00000000000000000064
                   01190000000000000000005300
-               101           0 RESUME                   0
+               109           0 RESUME                   0
                
-               103           2 LOAD_CONST               1 ('dateversion-distribution-version')
+               111           2 LOAD_CONST               1 ('dateversion-distribution-version')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (config_settings)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE    28 (to 76)
                
-               106          20 LOAD_FAST                0 (self)
+               114          20 LOAD_FAST                0 (self)
                             22 LOAD_METHOD              1 (_get_version)
                             44 PRECALL                  0
                             48 CALL                     0
                
-               104          58 LOAD_FAST                0 (self)
+               112          58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                0 (config_settings)
                
-               105          70 LOAD_CONST               1 ('dateversion-distribution-version')
+               113          70 LOAD_CONST               1 ('dateversion-distribution-version')
                
-               104          72 STORE_SUBSCR
+               112          72 STORE_SUBSCR
                
-               107     >>   76 LOAD_FAST                0 (self)
+               115     >>   76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                0 (config_settings)
                             88 LOAD_CONST               1 ('dateversion-distribution-version')
                             90 BINARY_SUBSCR
                            100 RETURN_VALUE
                consts
                   None
                   'dateversion-distribution-version'
                names      ('config_settings', '_get_version')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'version'
-               firstlineno 101
+               firstlineno 109
                lnotab 0x0202120326fe0c0102ff0403
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
-                  0x970067006401a2017d017c0144005d567d027c006a0000000000000000
-                  00a00100000000000000000000000000000000000000007c02a6010000ab
-                  0100000000000000007d037c00a002000000000000000000000000000000
-                  00000000007c03a6010000ab01000000000000000073047c036302010053
-                  00740600000000000000000000a004000000000000000000000000000000
-                  000000000064027c006a0500000000000000007c03a6030000ab03000000
-                  000000000001008c577401000000000000000000006a0100000000000000
-                  006403a6010000ab0100000000000000005300
-               109           0 RESUME                   0
+                  0x970067006401a2017d017c0144005d637d027401000000000000000000
+                  007c006a010000000000000000a002000000000000000000000000000000
+                  00000000007c02a6010000ab010000000000000000a6010000ab01000000
+                  00000000007d037c00a00300000000000000000000000000000000000000
+                  007c03a6010000ab01000000000000000073047c03630201005300740800
+                  000000000000000000a00500000000000000000000000000000000000000
+                  0064027c006a0600000000000000007c03a6030000ab0300000000000000
+                  0001008c647401000000000000000000007403000000000000000000006a
+                  0200000000000000006403a6010000ab010000000000000000a6010000ab
+                  0100000000000000005300
+               117           0 RESUME                   0
                
-               110           2 BUILD_LIST               0
+               118           2 BUILD_LIST               0
                              4 LOAD_CONST               1 (('%Y.%m', '%Y.%m.%d', '%Y.%m.%d.%H', '%Y.%m.%d.%H.%M'))
                              6 LIST_EXTEND              1
                              8 STORE_FAST               1 (formats)
                
-               117          10 LOAD_FAST                1 (formats)
+               125          10 LOAD_FAST                1 (formats)
                             12 GET_ITER
-                       >>   14 FOR_ITER                86 (to 188)
+                       >>   14 FOR_ITER                99 (to 214)
                             16 STORE_FAST               2 (format)
                
-               118          18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                0 (datetime)
-                            30 LOAD_METHOD              1 (strftime)
-                            52 LOAD_FAST                2 (format)
-                            54 PRECALL                  1
-                            58 CALL                     1
-                            68 STORE_FAST               3 (candidate)
-               
-               119          70 LOAD_FAST                0 (self)
-                            72 LOAD_METHOD              2 (version_in_repository)
-                            94 LOAD_FAST                3 (candidate)
-                            96 PRECALL                  1
-                           100 CALL                     1
-                           110 POP_JUMP_FORWARD_IF_TRUE     4 (to 120)
-               
-               120         112 LOAD_FAST                3 (candidate)
-                           114 SWAP                     2
-                           116 POP_TOP
-                           118 RETURN_VALUE
-               
-               121     >>  120 LOAD_GLOBAL              6 (LOG)
-                           132 LOAD_METHOD              4 (info)
-               
-               122         154 LOAD_CONST               2 ('%s-%s is already released, trying next...')
-               
-               123         156 LOAD_FAST                0 (self)
-                           158 LOAD_ATTR                5 (distribution_name)
-               
-               124         168 LOAD_FAST                3 (candidate)
-               
-               121         170 PRECALL                  3
-                           174 CALL                     3
-                           184 POP_TOP
-                           186 JUMP_BACKWARD           87 (to 14)
-               
-               128     >>  188 LOAD_GLOBAL              1 (NULL + datetime)
-                           200 LOAD_ATTR                1 (strftime)
-                           210 LOAD_CONST               3 ('%Y.%m.%d.%H.%M.%S')
-                           212 PRECALL                  1
-                           216 CALL                     1
-                           226 RETURN_VALUE
+               126          18 LOAD_GLOBAL              1 (NULL + normalized)
+                            30 LOAD_FAST                0 (self)
+                            32 LOAD_ATTR                1 (datetime)
+                            42 LOAD_METHOD              2 (strftime)
+                            64 LOAD_FAST                2 (format)
+                            66 PRECALL                  1
+                            70 CALL                     1
+                            80 PRECALL                  1
+                            84 CALL                     1
+                            94 STORE_FAST               3 (candidate)
+               
+               127          96 LOAD_FAST                0 (self)
+                            98 LOAD_METHOD              3 (version_in_repository)
+                           120 LOAD_FAST                3 (candidate)
+                           122 PRECALL                  1
+                           126 CALL                     1
+                           136 POP_JUMP_FORWARD_IF_TRUE     4 (to 146)
+               
+               128         138 LOAD_FAST                3 (candidate)
+                           140 SWAP                     2
+                           142 POP_TOP
+                           144 RETURN_VALUE
+               
+               129     >>  146 LOAD_GLOBAL              8 (LOG)
+                           158 LOAD_METHOD              5 (info)
+               
+               130         180 LOAD_CONST               2 ('%s-%s is already released, trying next...')
+               
+               131         182 LOAD_FAST                0 (self)
+                           184 LOAD_ATTR                6 (distribution_name)
+               
+               132         194 LOAD_FAST                3 (candidate)
+               
+               129         196 PRECALL                  3
+                           200 CALL                     3
+                           210 POP_TOP
+                           212 JUMP_BACKWARD          100 (to 14)
+               
+               136     >>  214 LOAD_GLOBAL              1 (NULL + normalized)
+                           226 LOAD_GLOBAL              3 (NULL + datetime)
+                           238 LOAD_ATTR                2 (strftime)
+                           248 LOAD_CONST               3 ('%Y.%m.%d.%H.%M.%S')
+                           250 PRECALL                  1
+                           254 CALL                     1
+                           264 PRECALL                  1
+                           268 CALL                     1
+                           278 RETURN_VALUE
                consts
                   None
                   ('%Y.%m', '%Y.%m.%d', '%Y.%m.%d.%H', '%Y.%m.%d.%H.%M')
                   '%s-%s is already released, trying next...'
                   '%Y.%m.%d.%H.%M.%S'
-               names      ('datetime', 'strftime', 'version_in_repository', 'LOG', 'info', 'distribution_name')
+               names      ('normalized', 'datetime', 'strftime', 'version_in_repository', 'LOG', 'info', 'distribution_name')
                varnames   ('self', 'formats', 'format', 'candidate')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       '_get_version'
-               firstlineno 109
-               lnotab 0x02010807080134012a010801220102010c0102fd1207
+               firstlineno 117
+               lnotab 0x0201080708014e012a010801220102010c0102fd1207
             'candidate_version'
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 6
                flags     : 3
                code
@@ -983,84 +1071,84 @@
                   00000000007c0476006302640064006400a6020000ab0200000000000000
                   000100530023003100730477027803590077010100590001000100640053
                   002300740e000000000000000000006a0e00000000000000006a0f000000
                   0000000000240072257d057c05a010000000000000000000000000000000
                   0000000000a6000000ab00000000000000000064056b0200000000720659
                   0064007d057e05640653007c05820164007d057e05770177007803590077
                   01
-               130           0 RESUME                   0
+               138           0 RESUME                   0
                
-               131           2 LOAD_GLOBAL              0 (os)
+               139           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (path)
                             24 LOAD_METHOD              2 (join)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (index_url)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                4 (distribution_name)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 STORE_FAST               2 (repo_url)
                
-               133          86 LOAD_GLOBAL             10 (LOG)
+               141          86 LOAD_GLOBAL             10 (LOG)
                             98 LOAD_METHOD              6 (info)
                            120 LOAD_CONST               1 ('looking for %s in %s ...')
                            122 LOAD_FAST                1 (candidate_version)
                            124 LOAD_FAST                2 (repo_url)
                            126 PRECALL                  3
                            130 CALL                     3
                            140 POP_TOP
                
-               136         142 NOP
+               144         142 NOP
                
-               137         144 LOAD_GLOBAL             14 (urllib)
+               145         144 LOAD_GLOBAL             14 (urllib)
                            156 LOAD_ATTR                8 (request)
                            166 LOAD_METHOD              9 (urlopen)
                            188 LOAD_FAST                2 (repo_url)
                            190 PRECALL                  1
                            194 CALL                     1
                            204 BEFORE_WITH
                            206 STORE_FAST               3 (response)
                
-               138         208 LOAD_GLOBAL             10 (LOG)
+               146         208 LOAD_GLOBAL             10 (LOG)
                            220 LOAD_METHOD             10 (debug)
                            242 LOAD_CONST               2 ('Response status: %s')
                            244 LOAD_FAST                3 (response)
                            246 LOAD_ATTR               11 (status)
                            256 PRECALL                  2
                            260 CALL                     2
                            270 POP_TOP
                
-               140         272 LOAD_FAST                3 (response)
+               148         272 LOAD_FAST                3 (response)
                            274 LOAD_METHOD             12 (read)
                            296 PRECALL                  0
                            300 CALL                     0
                            310 STORE_FAST               4 (body)
                
-               141         312 LOAD_GLOBAL             10 (LOG)
+               149         312 LOAD_GLOBAL             10 (LOG)
                            324 LOAD_METHOD             10 (debug)
                            346 LOAD_CONST               3 ('Response body: %s')
                            348 LOAD_FAST                4 (body)
                            350 PRECALL                  2
                            354 CALL                     2
                            364 POP_TOP
                
-               145         366 LOAD_FAST                0 (self)
+               153         366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR                4 (distribution_name)
                            378 FORMAT_VALUE             0
                            380 LOAD_CONST               4 ('-')
                            382 LOAD_FAST                1 (candidate_version)
                            384 FORMAT_VALUE             0
                            386 BUILD_STRING             3
                            388 LOAD_METHOD             13 (encode)
                            410 PRECALL                  0
                            414 CALL                     0
                            424 LOAD_FAST                4 (body)
                            426 CONTAINS_OP              0
                
-               137         428 SWAP                     2
+               145         428 SWAP                     2
                            430 LOAD_CONST               0 (None)
                            432 LOAD_CONST               0 (None)
                            434 LOAD_CONST               0 (None)
                            436 PRECALL                  2
                            440 CALL                     2
                            450 POP_TOP
                            452 RETURN_VALUE
@@ -1075,44 +1163,44 @@
                            470 POP_EXCEPT
                            472 POP_TOP
                            474 POP_TOP
                            476 LOAD_CONST               0 (None)
                            478 RETURN_VALUE
                        >>  480 PUSH_EXC_INFO
                
-               147         482 LOAD_GLOBAL             14 (urllib)
+               155         482 LOAD_GLOBAL             14 (urllib)
                            494 LOAD_ATTR               14 (error)
                            504 LOAD_ATTR               15 (HTTPError)
                            514 CHECK_EXC_MATCH
                            516 POP_JUMP_FORWARD_IF_FALSE    37 (to 592)
                            518 STORE_FAST               5 (error)
                
-               148         520 LOAD_FAST                5 (error)
+               156         520 LOAD_FAST                5 (error)
                            522 LOAD_METHOD             16 (getcode)
                            544 PRECALL                  0
                            548 CALL                     0
                            558 LOAD_CONST               5 (404)
                            560 COMPARE_OP               2 (==)
                            566 POP_JUMP_FORWARD_IF_FALSE     6 (to 580)
                
-               152         568 POP_EXCEPT
+               160         568 POP_EXCEPT
                            570 LOAD_CONST               0 (None)
                            572 STORE_FAST               5 (error)
                            574 DELETE_FAST              5 (error)
                            576 LOAD_CONST               6 (False)
                            578 RETURN_VALUE
                
-               153     >>  580 LOAD_FAST                5 (error)
+               161     >>  580 LOAD_FAST                5 (error)
                            582 RAISE_VARARGS            1
                        >>  584 LOAD_CONST               0 (None)
                            586 STORE_FAST               5 (error)
                            588 DELETE_FAST              5 (error)
                            590 RERAISE                  1
                
-               147     >>  592 RERAISE                  0
+               155     >>  592 RERAISE                  0
                        >>  594 COPY                     3
                            596 POP_EXCEPT
                            598 RERAISE                  1
                ExceptionTable:
                  144 to 204 -> 480 [0]
                  206 to 426 -> 454 [1] lasti
                  428 to 450 -> 480 [0]
@@ -1134,15 +1222,15 @@
                   False
                names      ('os', 'path', 'join', 'index_url', 'distribution_name', 'LOG', 'info', 'urllib', 'request', 'urlopen', 'debug', 'status', 'read', 'encode', 'error', 'HTTPError', 'getcode')
                varnames   ('self', 'candidate_version', 'repo_url', 'response', 'body', 'error')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'version_in_repository'
-               firstlineno 130
+               firstlineno 138
                lnotab 0x020154023803020140014002280136043ef8360a260130040c010cfa
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 35
                code
@@ -1160,124 +1248,124 @@
                   2a7401000000000000000000007c006a0100000000000000006403a60200
                   00ab020000000000000000a0080000000000000000000000000000000000
                   0000007c01a6010000ab0100000000000000000100640053006400530023
                   007c027c016b030000000072297401000000000000000000007c006a0100
                   000000000000006403a6020000ab020000000000000000a0080000000000
                   0000000000000000000000000000007c01a6010000ab0100000000000000
                   00010077007700780359007701
-               155           0 RETURN_GENERATOR
+               163           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               157           6 LOAD_GLOBAL              1 (NULL + open)
+               165           6 LOAD_GLOBAL              1 (NULL + open)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (version_path)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 LOAD_METHOD              2 (read)
                             66 PRECALL                  0
                             70 CALL                     0
                             80 STORE_FAST               1 (old_version_content)
                
-               158          82 LOAD_FAST                1 (old_version_content)
+               166          82 LOAD_FAST                1 (old_version_content)
                             84 STORE_FAST               2 (new_version_content)
                
-               165          86 LOAD_FAST                0 (self)
+               173          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                3 (marker)
                             98 LOAD_FAST                1 (old_version_content)
                            100 CONTAINS_OP              1
                            102 POP_JUMP_FORWARD_IF_FALSE    56 (to 216)
                
-               166         104 LOAD_GLOBAL              8 (VERSION_PATTERN)
+               174         104 LOAD_GLOBAL              8 (VERSION_PATTERN)
                            116 LOAD_METHOD              5 (sub)
                
-               167         138 LOAD_CONST               1 ('__version__ = ')
+               175         138 LOAD_CONST               1 ('__version__ = ')
                            140 LOAD_GLOBAL             13 (NULL + repr)
                            152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR                7 (version)
                            164 PRECALL                  1
                            168 CALL                     1
                            178 FORMAT_VALUE             0
                            180 LOAD_CONST               2 ('  # ')
                            182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                3 (marker)
                            194 FORMAT_VALUE             0
                            196 BUILD_STRING             4
                
-               168         198 LOAD_FAST                1 (old_version_content)
+               176         198 LOAD_FAST                1 (old_version_content)
                
-               166         200 PRECALL                  2
+               174         200 PRECALL                  2
                            204 CALL                     2
                            214 STORE_FAST               2 (new_version_content)
                
-               170     >>  216 NOP
+               178     >>  216 NOP
                
-               173         218 LOAD_FAST                2 (new_version_content)
+               181         218 LOAD_FAST                2 (new_version_content)
                            220 LOAD_FAST                1 (old_version_content)
                            222 COMPARE_OP               3 (!=)
                            228 POP_JUMP_FORWARD_IF_FALSE    40 (to 310)
                
-               174         230 LOAD_GLOBAL              1 (NULL + open)
+               182         230 LOAD_GLOBAL              1 (NULL + open)
                            242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                1 (version_path)
                            254 LOAD_CONST               3 ('w')
                            256 PRECALL                  2
                            260 CALL                     2
                            270 LOAD_METHOD              8 (write)
                            292 LOAD_FAST                2 (new_version_content)
                            294 PRECALL                  1
                            298 CALL                     1
                            308 POP_TOP
                
-               175     >>  310 LOAD_CONST               0 (None)
+               183     >>  310 LOAD_CONST               0 (None)
                            312 YIELD_VALUE
                            314 RESUME                   1
                            316 POP_TOP
                
-               177         318 LOAD_FAST                2 (new_version_content)
+               185         318 LOAD_FAST                2 (new_version_content)
                            320 LOAD_FAST                1 (old_version_content)
                            322 COMPARE_OP               3 (!=)
                            328 POP_JUMP_FORWARD_IF_FALSE    42 (to 414)
                
-               179         330 LOAD_GLOBAL              1 (NULL + open)
+               187         330 LOAD_GLOBAL              1 (NULL + open)
                            342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR                1 (version_path)
                            354 LOAD_CONST               3 ('w')
                            356 PRECALL                  2
                            360 CALL                     2
                            370 LOAD_METHOD              8 (write)
                            392 LOAD_FAST                1 (old_version_content)
                            394 PRECALL                  1
                            398 CALL                     1
                            408 POP_TOP
                            410 LOAD_CONST               0 (None)
                            412 RETURN_VALUE
                
-               177     >>  414 LOAD_CONST               0 (None)
+               185     >>  414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                        >>  418 PUSH_EXC_INFO
                            420 LOAD_FAST                2 (new_version_content)
                            422 LOAD_FAST                1 (old_version_content)
                            424 COMPARE_OP               3 (!=)
                            430 POP_JUMP_FORWARD_IF_FALSE    41 (to 514)
                
-               179         432 LOAD_GLOBAL              1 (NULL + open)
+               187         432 LOAD_GLOBAL              1 (NULL + open)
                            444 LOAD_FAST                0 (self)
                            446 LOAD_ATTR                1 (version_path)
                            456 LOAD_CONST               3 ('w')
                            458 PRECALL                  2
                            462 CALL                     2
                            472 LOAD_METHOD              8 (write)
                            494 LOAD_FAST                1 (old_version_content)
                            496 PRECALL                  1
                            500 CALL                     1
                            510 POP_TOP
                            512 RERAISE                  0
                
-               177     >>  514 RERAISE                  0
+               185     >>  514 RERAISE                  0
                        >>  516 COPY                     3
                            518 POP_EXCEPT
                            520 RERAISE                  1
                ExceptionTable:
                  218 to 316 -> 418 [0]
                  418 to 514 -> 516 [1] lasti
                consts
@@ -1287,30 +1375,30 @@
                   'w'
                names      ('open', 'version_path', 'read', 'marker', 'VERSION_PATTERN', 'sub', 'repr', 'version', 'write')
                varnames   ('self', 'old_version_content', 'new_version_content')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'patched_version'
-               firstlineno 155
+               firstlineno 163
                lnotab
                   0x06024c010407120122013c0102fe100402030c01500108020c0254fe12
                   0252fe
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c027c03ac01a6030000ab03000000000000000053
                   00
-               181           0 RESUME                   0
+               189           0 RESUME                   0
                
-               182           2 LOAD_FAST                0 (self)
+               190           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (build_backend)
                             14 LOAD_METHOD              1 (build_wheel)
                             36 LOAD_FAST                1 (wheel_directory)
                             38 LOAD_FAST                2 (config_settings)
                             40 LOAD_FAST                3 (metadata_directory)
                             42 KW_NAMES                 1
                             44 PRECALL                  3
@@ -1321,27 +1409,27 @@
                   ('config_settings', 'metadata_directory')
                names      ('build_backend', 'build_wheel')
                varnames   ('self', 'wheel_directory', 'config_settings', 'metadata_directory')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'delegate_build_wheel'
-               firstlineno 181
+               firstlineno 189
                lnotab 0x0201
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c02ac01a6020000ab0200000000000000005300
-               184           0 RESUME                   0
+               192           0 RESUME                   0
                
-               185           2 LOAD_FAST                0 (self)
+               193           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (build_backend)
                             14 LOAD_METHOD              1 (build_sdist)
                             36 LOAD_FAST                1 (sdist_directory)
                             38 LOAD_FAST                2 (config_settings)
                             40 KW_NAMES                 1
                             42 PRECALL                  2
                             46 CALL                     2
@@ -1351,28 +1439,28 @@
                   ('sdist_directory', 'config_settings')
                names      ('build_backend', 'build_sdist')
                varnames   ('self', 'sdist_directory', 'config_settings')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'delegate_build_sdist'
-               firstlineno 184
+               firstlineno 192
                lnotab 0x0201
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c027c03ac01a6030000ab03000000000000000053
                   00
-               187           0 RESUME                   0
+               195           0 RESUME                   0
                
-               188           2 LOAD_FAST                0 (self)
+               196           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (build_backend)
                             14 LOAD_METHOD              1 (build_editable)
                             36 LOAD_FAST                1 (wheel_directory)
                             38 LOAD_FAST                2 (config_settings)
                             40 LOAD_FAST                3 (metadata_directory)
                             42 KW_NAMES                 1
                             44 PRECALL                  3
@@ -1383,24 +1471,24 @@
                   ('config_settings', 'metadata_directory')
                names      ('build_backend', 'build_editable')
                varnames   ('self', 'wheel_directory', 'config_settings', 'metadata_directory')
                freevars   ()
                cellvars   ()
                filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'delegate_build_editable'
-               firstlineno 187
+               firstlineno 195
                lnotab 0x0201
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'property', 'str', 'marker', '_find_version_path', 'version_path', 'build_backend', 'index_url', 'distribution_name', 'version', '_get_version', 'bool', 'version_in_repository', 'contextmanager', 'patched_version', 'delegate_build_wheel', 'delegate_build_sdist', 'delegate_build_editable')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'DateVersion'
-         firstlineno 20
+         firstlineno 28
          lnotab
             0x0a01080502010aff0e0102030c0f02010aff0e010205020104ff0e0102
             1102010aff0e01020902010aff0e01021502010aff0e0102070c15101902
             0104ff0e01021906030603
       'DateVersion'
       code
          argcount  : 3
@@ -1410,44 +1498,44 @@
          code
             0x97007401000000000000000000007c01ac01a6010000ab010000000000
             0000007d037c03a0010000000000000000000000000000000000000000a6
             000000ab000000000000000000350001007c03a002000000000000000000
             00000000000000000000007c007c017c02ac02a6030000ab030000000000
             0000006302640064006400a6020000ab0200000000000000000100530023
             00310073047702780359007701010059000100010064005300
-         191           0 RESUME                   0
+         199           0 RESUME                   0
          
-         192           2 LOAD_GLOBAL              1 (NULL + DateVersion)
+         200           2 LOAD_GLOBAL              1 (NULL + DateVersion)
                       14 LOAD_FAST                1 (config_settings)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               3 (helper)
          
-         193          34 LOAD_FAST                3 (helper)
+         201          34 LOAD_FAST                3 (helper)
                       36 LOAD_METHOD              1 (patched_version)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 BEFORE_WITH
                       74 POP_TOP
          
-         194          76 LOAD_FAST                3 (helper)
+         202          76 LOAD_FAST                3 (helper)
                       78 LOAD_METHOD              2 (delegate_build_wheel)
          
-         195         100 LOAD_FAST                0 (wheel_directory)
+         203         100 LOAD_FAST                0 (wheel_directory)
          
-         196         102 LOAD_FAST                1 (config_settings)
+         204         102 LOAD_FAST                1 (config_settings)
          
-         197         104 LOAD_FAST                2 (metadata_directory)
+         205         104 LOAD_FAST                2 (metadata_directory)
          
-         194         106 KW_NAMES                 2
+         202         106 KW_NAMES                 2
                      108 PRECALL                  3
                      112 CALL                     3
          
-         193         122 SWAP                     2
+         201         122 SWAP                     2
                      124 LOAD_CONST               0 (None)
                      126 LOAD_CONST               0 (None)
                      128 LOAD_CONST               0 (None)
                      130 PRECALL                  2
                      134 CALL                     2
                      144 POP_TOP
                      146 RETURN_VALUE
@@ -1474,52 +1562,52 @@
             ('config_settings', 'metadata_directory')
          names      ('DateVersion', 'patched_version', 'delegate_build_wheel')
          varnames   ('wheel_directory', 'config_settings', 'metadata_directory', 'helper')
          freevars   ()
          cellvars   ()
          filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'build_wheel'
-         firstlineno 191
+         firstlineno 199
          lnotab 0x020120012a0118010201020102fd10ff
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c01ac01a6010000ab010000000000
             0000007d027c02a0010000000000000000000000000000000000000000a6
             000000ab000000000000000000350001007c02a002000000000000000000
             00000000000000000000007c007c01a6020000ab02000000000000000063
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         201           0 RESUME                   0
+         209           0 RESUME                   0
          
-         202           2 LOAD_GLOBAL              1 (NULL + DateVersion)
+         210           2 LOAD_GLOBAL              1 (NULL + DateVersion)
                       14 LOAD_FAST                1 (config_settings)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               2 (helper)
          
-         203          34 LOAD_FAST                2 (helper)
+         211          34 LOAD_FAST                2 (helper)
                       36 LOAD_METHOD              1 (patched_version)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 BEFORE_WITH
                       74 POP_TOP
          
-         204          76 LOAD_FAST                2 (helper)
+         212          76 LOAD_FAST                2 (helper)
                       78 LOAD_METHOD              2 (delegate_build_sdist)
                      100 LOAD_FAST                0 (sdist_directory)
                      102 LOAD_FAST                1 (config_settings)
                      104 PRECALL                  2
                      108 CALL                     2
          
-         203         118 SWAP                     2
+         211         118 SWAP                     2
                      120 LOAD_CONST               0 (None)
                      122 LOAD_CONST               0 (None)
                      124 LOAD_CONST               0 (None)
                      126 PRECALL                  2
                      130 CALL                     2
                      140 POP_TOP
                      142 RETURN_VALUE
@@ -1545,53 +1633,53 @@
             ('config_settings',)
          names      ('DateVersion', 'patched_version', 'delegate_build_sdist')
          varnames   ('sdist_directory', 'config_settings', 'helper')
          freevars   ()
          cellvars   ()
          filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'build_sdist'
-         firstlineno 201
+         firstlineno 209
          lnotab 0x020120012a012aff
       code
          argcount  : 3
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c01ac01a6010000ab010000000000
             0000007d037c03a0010000000000000000000000000000000000000000a6
             000000ab000000000000000000350001007c03a002000000000000000000
             00000000000000000000007c007c017c02a6030000ab0300000000000000
             006302640064006400a6020000ab02000000000000000001005300230031
             0073047702780359007701010059000100010064005300
-         221           0 RESUME                   0
+         229           0 RESUME                   0
          
-         222           2 LOAD_GLOBAL              1 (NULL + DateVersion)
+         230           2 LOAD_GLOBAL              1 (NULL + DateVersion)
                       14 LOAD_FAST                1 (config_settings)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               3 (helper)
          
-         224          34 LOAD_FAST                3 (helper)
+         232          34 LOAD_FAST                3 (helper)
                       36 LOAD_METHOD              1 (patched_version)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 BEFORE_WITH
                       74 POP_TOP
          
-         225          76 LOAD_FAST                3 (helper)
+         233          76 LOAD_FAST                3 (helper)
                       78 LOAD_METHOD              2 (delegate_build_editable)
                      100 LOAD_FAST                0 (wheel_directory)
                      102 LOAD_FAST                1 (config_settings)
                      104 LOAD_FAST                2 (metadata_directory)
                      106 PRECALL                  3
                      110 CALL                     3
          
-         224         120 SWAP                     2
+         232         120 SWAP                     2
                      122 LOAD_CONST               0 (None)
                      124 LOAD_CONST               0 (None)
                      126 LOAD_CONST               0 (None)
                      128 PRECALL                  2
                      132 CALL                     2
                      142 POP_TOP
                      144 RETURN_VALUE
@@ -1617,21 +1705,21 @@
             ('config_settings',)
          names      ('DateVersion', 'patched_version', 'delegate_build_editable')
          varnames   ('wheel_directory', 'config_settings', 'metadata_directory', 'helper')
          freevars   ()
          cellvars   ()
          filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'build_editable'
-         firstlineno 221
+         firstlineno 229
          lnotab 0x020120022a012cff
       (None, None)
       (None,)
-   names      ('os', 'logging', 're', 'urllib.request', 'urllib', 'urllib.error', 'datetime', 'contextlib', 'contextmanager', 'importlib', 'getLogger', 'LOG', 'setLevel', 'DEBUG', 'addHandler', 'FileHandler', 'compile', 'MULTILINE', 'VERSION_PATTERN', 'DateVersion', 'build_wheel', 'build_sdist', 'build_editable')
+   names      ('os', 'logging', 're', 'urllib.request', 'urllib', 'urllib.error', 'datetime', 'contextlib', 'contextmanager', 'importlib', 'getLogger', 'LOG', 'setLevel', 'DEBUG', 'addHandler', 'FileHandler', 'compile', 'MULTILINE', 'VERSION_PATTERN', 'str', 'normalized', 'DateVersion', 'build_wheel', 'build_sdist', 'build_editable')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010801080108010c010c0108022002340346022e031a
-      7f002c080a0814
+      0x00ff0201080108010801080108010c010c0108022002340346022e030c
+      081a7f002c080a0814
```

### Comparing `buildsys-dateversion-2023.5/src/buildsys_dateversion/_hooks.py` & `buildsys-dateversion-2023.5.1/src/buildsys_dateversion/_hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 
 # FIXME: make configurable
 LOG.addHandler(logging.FileHandler("/tmp/buildsys-dateversion.log"))
 
 VERSION_PATTERN = re.compile(r"^__version__ *=.*$", flags=re.MULTILINE)
 
 
+def normalized(version: str):
+    # PEP 440 version string normalization.
+    #
+    # (Not a generic function, just 'good enough' to work on our
+    # known strftime templates)
+    return '.'.join([str(int(x)) for x in version.split('.')])
+
+
 class DateVersion:
     def __init__(self, config_settings=None):
         self.config_settings: dict = (config_settings or {}).copy()
         self.datetime = datetime.utcnow()
         LOG.debug("operating with datetime = %s", self.datetime)
 
     @property
@@ -111,25 +119,25 @@
             "%Y.%m",
             "%Y.%m.%d",
             "%Y.%m.%d.%H",
             "%Y.%m.%d.%H.%M",
         ]
 
         for format in formats:
-            candidate = self.datetime.strftime(format)
+            candidate = normalized(self.datetime.strftime(format))
             if not self.version_in_repository(candidate):
                 return candidate
             LOG.info(
                 "%s-%s is already released, trying next...",
                 self.distribution_name,
                 candidate,
             )
 
         # Final fallback
-        return datetime.strftime("%Y.%m.%d.%H.%M.%S")
+        return normalized(datetime.strftime("%Y.%m.%d.%H.%M.%S"))
 
     def version_in_repository(self, candidate_version: str) -> bool:
         repo_url = os.path.join(self.index_url, self.distribution_name)
 
         LOG.info("looking for %s in %s ...", candidate_version, repo_url)
 
         # TODO: might we need to support custom CA bundles here?
```

