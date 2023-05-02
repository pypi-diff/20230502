# Comparing `tmp/algokit_utils-1.1.0b3-py3-none-any.whl.zip` & `tmp/algokit_utils-1.1.0b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 33086 bytes, number of entries: 15
+Zip file size: 33633 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     3697 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
--rw-r--r--  2.0 unx    29956 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx    32431 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/RECORD
-15 files, 125584 bytes uncompressed, 30994 bytes compressed:  75.3%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.1.0b4.dist-info/RECORD
+15 files, 128059 bytes uncompressed, 31541 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.1.0b3.dist-info/LICENSE
+Filename: algokit_utils-1.1.0b4.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.1.0b3.dist-info/METADATA
+Filename: algokit_utils-1.1.0b4.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.1.0b3.dist-info/WHEEL
+Filename: algokit_utils-1.1.0b4.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.1.0b3.dist-info/RECORD
+Filename: algokit_utils-1.1.0b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/deploy.py

```diff
@@ -1,12 +1,11 @@
 import base64
 import dataclasses
 import json
 import logging
-import re
 from collections.abc import Iterable, Mapping, Sequence
 from enum import Enum
 from typing import TYPE_CHECKING, TypeAlias, TypedDict
 
 from algosdk import transaction
 from algosdk.atomic_transaction_composer import AtomicTransactionComposer, TransactionSigner
 from algosdk.logic import get_application_address
@@ -275,69 +274,141 @@
     return AppChanges(
         app_updated=app_updated,
         schema_breaking_change=bool(schema_changes),
         schema_change_description=", ".join(schema_changes),
     )
 
 
+def _is_valid_token_character(char: str) -> bool:
+    return char.isalnum() or char == "_"
+
+
 def _replace_template_variable(program_lines: list[str], template_variable: str, value: str) -> tuple[list[str], int]:
     result: list[str] = []
     match_count = 0
-    pattern = re.compile(rf"(\b)TMPL_{template_variable}(\b|$)")
-
-    def replacement(m: re.Match) -> str:
-        return f"{m.group(1)}{value}{m.group(2)}"
-
+    token = f"TMPL_{template_variable}"
+    token_idx_offset = len(value) - len(token)
     for line in program_lines:
-        code_comment = line.split("//", maxsplit=1)
-        code = code_comment[0]
-        new_line, matches = re.subn(pattern, replacement, code)
-        match_count += matches
-        if len(code_comment) > 1:
-            new_line = f"{new_line}//{code_comment[1]}"
-        result.append(new_line)
+        comment_idx = _find_unquoted_string(line, "//")
+        if comment_idx is None:
+            comment_idx = len(line)
+        code = line[:comment_idx]
+        comment = line[comment_idx:]
+        trailing_idx = 0
+        while True:
+            token_idx = _find_template_token(code, token, trailing_idx)
+            if token_idx is None:
+                break
+
+            trailing_idx = token_idx + len(token)
+            prefix = code[:token_idx]
+            suffix = code[trailing_idx:]
+            code = f"{prefix}{value}{suffix}"
+            match_count += 1
+            trailing_idx += token_idx_offset
+        result.append(code + comment)
     return result, match_count
 
 
 def add_deploy_template_variables(
     template_values: TemplateValueDict, allow_update: bool | None, allow_delete: bool | None
 ) -> None:
     if allow_update is not None:
         template_values[_UPDATABLE] = int(allow_update)
     if allow_delete is not None:
         template_values[_DELETABLE] = int(allow_delete)
 
 
+def _find_unquoted_string(line: str, token: str, start: int = 0, end: int = -1) -> int | None:
+    """Find the first string within a line of TEAL. Only matches outside of quotes are returned.
+    Returns None if not found"""
+
+    if end < 0:
+        end = len(line)
+    idx = start
+    in_quotes = False
+    while idx < end:
+        current_char = line[idx]
+        match current_char:
+            case "\\":
+                if in_quotes:  # skip next character
+                    idx += 1
+            case '"':
+                in_quotes = not in_quotes
+            case _:
+                # only match if not in quotes and string matches
+                if not in_quotes and line.startswith(token, idx):
+                    return idx
+        idx += 1
+    return None
+
+
+def _find_template_token(line: str, token: str, start: int = 0, end: int = -1) -> int | None:
+    """Find the first template token within a line of TEAL. Only matches outside of quotes are returned.
+    Only full token matches are returned, i.e. TMPL_STR will not match against TMPL_STRING
+    Returns None if not found"""
+    if end < 0:
+        end = len(line)
+
+    idx = start
+    while idx < end:
+        token_idx = _find_unquoted_string(line, token, idx, end)
+        if token_idx is None:
+            break
+        trailing_idx = token_idx + len(token)
+        if (token_idx == 0 or not _is_valid_token_character(line[token_idx - 1])) and (  # word boundary at start
+            trailing_idx >= len(line) or not _is_valid_token_character(line[trailing_idx])  # word boundary at end
+        ):
+            return token_idx
+        idx = trailing_idx
+    return None
+
+
+def _strip_comment(line: str) -> str:
+    comment_idx = _find_unquoted_string(line, "//")
+    if comment_idx is None:
+        return line
+    return line[:comment_idx]
+
+
 def strip_comments(program: str) -> str:
-    lines = [line.split("//", maxsplit=1)[0] for line in program.splitlines()]
-    return "\n".join(lines)
+    return "\n".join(_strip_comment(line) for line in program.splitlines())
+
+
+def _has_token(program_without_comments: str, token: str) -> bool:
+    for line in program_without_comments.splitlines():
+        token_idx = _find_template_token(line, token)
+        if token_idx is not None:
+            return True
+    return False
 
 
 def check_template_variables(approval_program: str, template_values: TemplateValueDict) -> None:
     approval_program = strip_comments(approval_program)
-    if UPDATABLE_TEMPLATE_NAME in approval_program and _UPDATABLE not in template_values:
+    if _has_token(approval_program, UPDATABLE_TEMPLATE_NAME) and _UPDATABLE not in template_values:
         raise DeploymentFailedError(
             "allow_update must be specified if deploy time configuration of update is being used"
         )
-    if DELETABLE_TEMPLATE_NAME in approval_program and _DELETABLE not in template_values:
+    if _has_token(approval_program, DELETABLE_TEMPLATE_NAME) and _DELETABLE not in template_values:
         raise DeploymentFailedError(
             "allow_delete must be specified if deploy time configuration of delete is being used"
         )
 
     for template_variable_name in template_values:
-        if template_variable_name not in approval_program:
+        tmpl_variable = f"TMPL_{template_variable_name}"
+        if not _has_token(approval_program, tmpl_variable):
             if template_variable_name == _UPDATABLE:
                 raise DeploymentFailedError(
                     "allow_update must only be specified if deploy time configuration of update is being used"
                 )
             if template_variable_name == _DELETABLE:
                 raise DeploymentFailedError(
                     "allow_delete must only be specified if deploy time configuration of delete is being used"
                 )
-            logger.warning(f"{template_variable_name} not found in approval program, but variable was provided")
+            logger.warning(f"{tmpl_variable} not found in approval program, but variable was provided")
 
 
 def replace_template_variables(program: str, template_values: TemplateValueMapping) -> str:
     """Replaces `TMPL_*` variables in `program` with `template_values`
 
     ```{note}
     `template_values` keys should *NOT* be prefixed with `TMPL_`
```

## Comparing `algokit_utils-1.1.0b3.dist-info/LICENSE` & `algokit_utils-1.1.0b4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.1.0b3.dist-info/METADATA` & `algokit_utils-1.1.0b4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.1.0b3
+Version: 1.1.0b4
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.1.0b3.dist-info/RECORD` & `algokit_utils-1.1.0b4.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 algokit_utils/__init__.py,sha256=XFpWqRXQgnT9JCh6ZOlI2strJgbaZeaykfM2JZgBz9E,3697
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
-algokit_utils/deploy.py,sha256=Vg5K7xDSp7F8ImwT9FyboZDZFHeq_HeZgZyU26lvjE0,29956
+algokit_utils/deploy.py,sha256=Qdlfos3AcgkxoS69cx3TzTf210nn3dssKWwEjb_vJok,32431
 algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
 algokit_utils/models.py,sha256=46vPWFNMowMyNOhmlInq58gVtOg91xgPhQ0w-bIMacw,3930
 algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.1.0b3.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.1.0b3.dist-info/METADATA,sha256=SH2sU6iQlt4Avwa8dBD_4CM08vjl6VxEjN8e8eo8Z10,2037
-algokit_utils-1.1.0b3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.1.0b3.dist-info/RECORD,,
+algokit_utils-1.1.0b4.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.1.0b4.dist-info/METADATA,sha256=7stt4wjNUve0FaYO9OdMTkBhxJNFT57hVhPIztbp2Wo,2037
+algokit_utils-1.1.0b4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.1.0b4.dist-info/RECORD,,
```

