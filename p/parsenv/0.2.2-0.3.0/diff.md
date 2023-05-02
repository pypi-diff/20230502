# Comparing `tmp/parsenv-0.2.2.tar.gz` & `tmp/parsenv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsenv-0.2.2.tar", last modified: Sat Apr 29 17:14:06 2023, max compression
+gzip compressed data, was "parsenv-0.3.0.tar", last modified: Tue May  2 10:43:40 2023, max compression
```

## Comparing `parsenv-0.2.2.tar` & `parsenv-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      242 2023-04-29 16:54:02.050035 parsenv-0.2.2/env/__init__.py
--rw-r--r--   0        0        0      114 2023-04-29 16:54:02.080416 parsenv-0.2.2/env/core.py
--rw-r--r--   0        0        0     1379 2023-04-29 16:54:01.987250 parsenv-0.2.2/env/main.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.2.2/env/py.typed
--rw-r--r--   0        0        0      470 2023-04-29 17:14:06.875278 parsenv-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      952 2023-04-29 17:10:16.708983 parsenv-0.2.2/README.md
--rw-r--r--   0        0        0      778 2023-04-29 16:55:03.344368 parsenv-0.2.2/tests/__main__.py
--rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 parsenv-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-05-02 10:33:58.903078 parsenv-0.3.0/env/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-29 16:54:02.080416 parsenv-0.3.0/env/core.py
+-rw-r--r--   0        0        0     1446 2023-05-02 10:39:57.829703 parsenv-0.3.0/env/main.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.3.0/env/py.typed
+-rw-r--r--   0        0        0      470 2023-05-02 10:42:46.368242 parsenv-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      978 2023-05-02 10:42:29.286906 parsenv-0.3.0/README.md
+-rw-r--r--   0        0        0      804 2023-05-02 10:33:58.944876 parsenv-0.3.0/tests/__main__.py
+-rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 parsenv-0.3.0/PKG-INFO
```

### Comparing `parsenv-0.2.2/env/main.py` & `parsenv-0.3.0/env/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,7 +67,11 @@
 @overload
 def get_ints(name: str, default: list[int] | None) -> list[int] | None:
     ...
 
 
 def get_ints(name: str, default: list[int] | DEFAULT = UNDEFINED):
     return raw.list(name, default=default, subcast=int)
+
+
+def prefix(value: str):
+    return raw.prefixed(f"{value}_")
```

### Comparing `parsenv-0.2.2/README.md` & `parsenv-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", None) is None
 assert env.get_int("PORT") == 123
 assert env.get_strs("KEYS", []) == ["word1", "F402", "12"]
 assert env.get_ints("ADMIN_IDS") == [1, 2, 3]
 assert env.get_ints("X", [0]) == [0]
-assert env.get_bool("T_BOOL")
-assert not env.get_bool("F_BOOL")
+
+with env.prefix("BOOL"):
+    assert env.get_bool("T")
+    assert not env.get_bool("F")
 
 try:
     env.get("X")
 except Exception as e:
     assert str(e) == 'Mandatory environment variable "X" is missing'
 
 try:
```

### Comparing `parsenv-0.2.2/tests/__main__.py` & `parsenv-0.3.0/tests/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", None) is None
 assert env.get_int("PORT") == 123
 assert env.get_strs("KEYS", []) == ["word1", "F402", "12"]
 assert env.get_ints("ADMIN_IDS") == [1, 2, 3]
 assert env.get_ints("X", [0]) == [0]
-assert env.get_bool("T_BOOL")
-assert not env.get_bool("F_BOOL")
+
+with env.prefix("BOOL"):
+    assert env.get_bool("T")
+    assert not env.get_bool("F")
 
 try:
     env.get("X")
 except Exception as e:
     assert str(e) == 'Mandatory environment variable "X" is missing'
 
 try:
```

### Comparing `parsenv-0.2.2/PKG-INFO` & `parsenv-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsenv
-Version: 0.2.2
+Version: 0.3.0
 Summary: Typed dotenv parser
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ### Getting Started
@@ -20,16 +20,18 @@
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", None) is None
 assert env.get_int("PORT") == 123
 assert env.get_strs("KEYS", []) == ["word1", "F402", "12"]
 assert env.get_ints("ADMIN_IDS") == [1, 2, 3]
 assert env.get_ints("X", [0]) == [0]
-assert env.get_bool("T_BOOL")
-assert not env.get_bool("F_BOOL")
+
+with env.prefix("BOOL"):
+    assert env.get_bool("T")
+    assert not env.get_bool("F")
 
 try:
     env.get("X")
 except Exception as e:
     assert str(e) == 'Mandatory environment variable "X" is missing'
 
 try:
```

