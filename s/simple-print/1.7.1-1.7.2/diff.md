# Comparing `tmp/simple_print-1.7.1-py3-none-any.whl.zip` & `tmp/simple_print-1.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7714 bytes, number of entries: 11
+Zip file size: 7742 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx       51 b- defN 23-Apr-28 06:49 simple_print/__init__.py
 -rw-rw-r--  2.0 unx     4467 b- defN 22-Dec-04 17:59 simple_print/broker.py
--rw-rw-r--  2.0 unx     4198 b- defN 23-Apr-28 06:49 simple_print/sprint.py
+-rw-rw-r--  2.0 unx     4392 b- defN 23-May-02 07:17 simple_print/sprint.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-21 11:16 test/__init__.py
 -rw-rw-r--  2.0 unx      220 b- defN 22-Dec-04 18:00 test/test_broker.py
 -rw-rw-r--  2.0 unx     1861 b- defN 23-Feb-27 07:48 test/test_print.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-Apr-28 06:55 simple_print-1.7.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2605 b- defN 23-Apr-28 06:55 simple_print-1.7.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 06:55 simple_print-1.7.1.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       18 b- defN 23-Apr-28 06:55 simple_print-1.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      868 b- defN 23-Apr-28 06:55 simple_print-1.7.1.dist-info/RECORD
-11 files, 15474 bytes uncompressed, 6246 bytes compressed:  59.6%
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2605 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       18 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      868 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/RECORD
+11 files, 15668 bytes uncompressed, 6274 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: test/test_broker.py
 Comment: 
 
 Filename: test/test_print.py
 Comment: 
 
-Filename: simple_print-1.7.1.dist-info/LICENSE
+Filename: simple_print-1.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: simple_print-1.7.1.dist-info/METADATA
+Filename: simple_print-1.7.2.dist-info/METADATA
 Comment: 
 
-Filename: simple_print-1.7.1.dist-info/WHEEL
+Filename: simple_print-1.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: simple_print-1.7.1.dist-info/top_level.txt
+Filename: simple_print-1.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_print-1.7.1.dist-info/RECORD
+Filename: simple_print-1.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_print/sprint.py

```diff
@@ -87,29 +87,33 @@
                 _colored_print(arg, arg_name, c, b, a, i, p, function_name, lineno, filename)
         
         if s:
             return ";".join(arg_names)
 
 
 @contextmanager
-def SprintErr():
+def SprintErr(DEBUG=True):
 
     def format_exception(ei) -> str:
         sio = io.StringIO()
         tb = ei[2]
         traceback.print_exception(ei[0], ei[1], tb, None, sio)
         s = sio.getvalue()
         sio.close()
         if s[-1:] == "\n":
             s = s[:-1]
         return s
 
-    cprint("\nSprintErr -> looking for errors [start ok]", color="green")
-    try:
-        yield 
-    except Exception as e:
-        ei = sys.exc_info()
-        print(format_exception(ei))
-    finally:
-        cprint("SprintErr -> looking for errors [finish ok]\n", color="green")
+    if DEBUG:
+        stack = traceback.extract_stack()
+        filename, lineno, function_name, code = stack[-3]
+
+        cprint(f"\nSprintErr. filename={filename} lineno={lineno} [ START OK ]", color="green")
+        try:
+            yield 
+        except Exception as e:
+            ei = sys.exc_info()
+            print(format_exception(ei))
+        finally:
+            cprint(f"SprintErr. filename={filename} lineno={lineno} [ FINISH OK ]\n", color="yellow")
```

## Comparing `simple_print-1.7.1.dist-info/LICENSE` & `simple_print-1.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simple_print-1.7.1.dist-info/METADATA` & `simple_print-1.7.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-print
-Version: 1.7.1
+Version: 1.7.2
 Summary: Powerful debugging tool for Python.
 Home-page: https://github.com/Sobolev5/simple-print/
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `simple_print-1.7.1.dist-info/RECORD` & `simple_print-1.7.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 simple_print/__init__.py,sha256=5PxZbGPVCHHFBkxb0qDKf-r13G5KKjlFbqNWXDnvWGA,51
 simple_print/broker.py,sha256=p1DDR4UjHBxH0BXqnw_O2dTes-H8rpV8UwzvvVKEh90,4467
-simple_print/sprint.py,sha256=ORK0-633_A18IAPIL8drsTSFcawvSGR5-kvXNPDdJMc,4198
+simple_print/sprint.py,sha256=TyPwIC0xskDGFmpzBxvUJEwqqcNWPudNeleO-fUyhLs,4392
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_broker.py,sha256=hdDXeNHlO9s2vd_pLlHdqypWgCMQIPa3mz9Ou9Md22c,220
 test/test_print.py,sha256=agnkk5AL5xtnG-4odW0Hr1ahM5iw-Ycv1I9DIwddJ_Y,1861
-simple_print-1.7.1.dist-info/LICENSE,sha256=D2EVTI_UztUmQIzfsNpaXSuKgHLnBVY9Y56G77ZBFv0,1094
-simple_print-1.7.1.dist-info/METADATA,sha256=nRceCCnfana9IOvkPkcXvmJKkSUa13nRZTX0fz6NZhg,2605
-simple_print-1.7.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-simple_print-1.7.1.dist-info/top_level.txt,sha256=Yhv0h31B2Z5Nu3_Zy3Y27TOagXhPb2VGQBI9Q6CxV3Q,18
-simple_print-1.7.1.dist-info/RECORD,,
+simple_print-1.7.2.dist-info/LICENSE,sha256=D2EVTI_UztUmQIzfsNpaXSuKgHLnBVY9Y56G77ZBFv0,1094
+simple_print-1.7.2.dist-info/METADATA,sha256=rM_YcYoG43adVNBtiD4brcDTdBy8Iv8wcNb1qty4lvM,2605
+simple_print-1.7.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+simple_print-1.7.2.dist-info/top_level.txt,sha256=Yhv0h31B2Z5Nu3_Zy3Y27TOagXhPb2VGQBI9Q6CxV3Q,18
+simple_print-1.7.2.dist-info/RECORD,,
```

