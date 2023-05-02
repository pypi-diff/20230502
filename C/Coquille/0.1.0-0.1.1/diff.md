# Comparing `tmp/Coquille-0.1.0.tar.gz` & `tmp/Coquille-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-0.1.0.tar", last modified: Tue May  2 19:24:31 2023, max compression
+gzip compressed data, was "Coquille-0.1.1.tar", last modified: Tue May  2 20:56:59 2023, max compression
```

## Comparing `Coquille-0.1.0.tar` & `Coquille-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:24:31.110359 Coquille-0.1.0/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.0/.gitignore
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.0/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1460 2023-05-02 19:24:31.110359 Coquille-0.1.0/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1103 2023-05-02 19:24:02.000000 Coquille-0.1.0/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:24:31.107026 Coquille-0.1.0/examples/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:24:31.110359 Coquille-0.1.0/examples/coquille_context/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.0/examples/coquille_context/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.0/examples/coquille_context/screenshot.png
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-02 19:24:20.000000 Coquille-0.1.0/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-02 19:24:31.110359 Coquille-0.1.0/setup.cfg
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:24:31.107026 Coquille-0.1.0/src/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:24:31.110359 Coquille-0.1.0/src/Coquille.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1460 2023-05-02 19:24:31.000000 Coquille-0.1.0/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      391 2023-05-02 19:24:31.000000 Coquille-0.1.0/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-02 19:24:31.000000 Coquille-0.1.0/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-02 19:24:31.000000 Coquille-0.1.0/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:24:31.110359 Coquille-0.1.0/src/coquille/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.0/src/coquille/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5584 2023-05-02 19:09:12.000000 Coquille-0.1.0/src/coquille/coquille.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10609 2023-05-02 18:53:58.000000 Coquille-0.1.0/src/coquille/sequences.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.0/src/coquille/typeshed.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.1/.gitignore
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.1/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1480 2023-05-02 20:56:59.689721 Coquille-0.1.1/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1103 2023-05-02 19:24:02.000000 Coquille-0.1.1/README.md
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.686388 Coquille-0.1.1/examples/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/examples/coquille_context/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.1/examples/coquille_context/__main__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.1/examples/coquille_context/screenshot.png
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-02 20:56:46.000000 Coquille-0.1.1/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-02 20:56:59.689721 Coquille-0.1.1/setup.cfg
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 20:03:01.000000 Coquille-0.1.1/setup.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.686388 Coquille-0.1.1/src/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/src/Coquille.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1480 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      500 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/src/coquille/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.1/src/coquille/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5735 2023-05-02 20:49:56.000000 Coquille-0.1.1/src/coquille/coquille.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 20:27:12.000000 Coquille-0.1.1/src/coquille/sequences.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.1/src/coquille/typeshed.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/tests/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:55:01.000000 Coquille-0.1.1/tests/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 20:50:32.000000 Coquille-0.1.1/tests/coquille_test.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 20:30:32.000000 Coquille-0.1.1/tests/sequences_test.py
```

### Comparing `Coquille-0.1.0/.gitignore` & `Coquille-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.0/.pre-commit-config.yaml` & `Coquille-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.0/LICENSE` & `Coquille-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.0/PKG-INFO` & `Coquille-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 0.1.0
+Version: 0.1.1
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Coquille
 
 Coquille (IPA: `/kɔ.kij/`, english: 'shell' or 'typo') is a library that wraps terminal escape sequences to easily apply them to a stream.
 
 ## Notes
```

### Comparing `Coquille-0.1.0/README.md` & `Coquille-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.0/examples/coquille_context/screenshot.png` & `Coquille-0.1.1/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.0/src/Coquille.egg-info/PKG-INFO` & `Coquille-0.1.1/src/Coquille.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 0.1.0
+Version: 0.1.1
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Coquille
 
 Coquille (IPA: `/kɔ.kij/`, english: 'shell' or 'typo') is a library that wraps terminal escape sequences to easily apply them to a stream.
 
 ## Notes
```

### Comparing `Coquille-0.1.0/src/coquille/coquille.py` & `Coquille-0.1.1/src/coquille/coquille.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 from coquille.sequences import EscapeSequence
 from coquille.sequences import soft_reset
 
 __all__ = ["apply", "Coquille", "EscapeSequence", "prepare"]
 
 # ... don't say anything.
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     if sys.version_info >= (3, 10):
         from typing import ParamSpec
 
         P = ParamSpec("P")
 
     from coquille.typeshed import Self
     from coquille.typeshed import SupportsWrite
 
 
 @overload
-def prepare(sequence: EscapeSequence) -> EscapeSequence:
+def prepare(sequence: EscapeSequence) -> EscapeSequence:  # pragma: no cover
     pass
 
 
 @overload
 def prepare(
     sequence: Callable[P, EscapeSequence],
     *args: P.args,
     **kwargs: P.kwargs,
-) -> EscapeSequence:
+) -> EscapeSequence:  # pragma: no cover
     pass
 
 
 def prepare(
     sequence: EscapeSequence | Callable[P, EscapeSequence],
     *args: P.args,
     **kwargs: P.kwargs,
@@ -51,25 +51,28 @@
     if isinstance(sequence, str):
         return sequence
 
     return sequence(*args, **kwargs)
 
 
 @overload
-def apply(sequence: EscapeSequence, file: SupportsWrite[str] | None = None) -> None:
+def apply(
+    sequence: EscapeSequence,
+    file: SupportsWrite[str] | None = None,
+) -> None:  # pragma: no cover
     pass
 
 
 @overload
 def apply(
     sequence: Callable[P, EscapeSequence],
     file: SupportsWrite[str] | None = None,
     *args: P.args,
     **kwargs: P.kwargs,
-) -> None:
+) -> None:  # pragma: no cover
     pass
 
 
 def apply(
     sequence: EscapeSequence | Callable[P, EscapeSequence],
     file: SupportsWrite[str] | None = None,
     *args: P.args,
@@ -135,24 +138,24 @@
 @dataclass(slots=True)
 class Coquille:
     sequences: list[EscapeSequence]
     file: SupportsWrite[str] | None
 
     @overload
     @classmethod
-    def new(cls: type[Self], *sequences: EscapeSequence) -> Self:
+    def new(cls: type[Self], *sequences: EscapeSequence) -> Self:  # pragma: no cover
         pass
 
     @overload
     @classmethod
     def new(
         cls: type[Self],
         *sequences: EscapeSequence,
         file: SupportsWrite[str],
-    ) -> Self:
+    ) -> Self:  # pragma: no cover
         pass
 
     @classmethod
     def new(
         cls: type[Self],
         *sequences: EscapeSequence,
         file: SupportsWrite[str] | None = None,
```

### Comparing `Coquille-0.1.0/src/coquille/sequences.py` & `Coquille-0.1.1/src/coquille/sequences.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 BACKGROUND_CODE = 40
 UNDERLINE_CODE = 50
 RESET = 9
 
 
 # Helper types
 EscapeSequence = NewType("EscapeSequence", str)
-AltFontNumber = Literal[11, 12, 13, 14, 15, 16, 17, 18, 19]
+AltFontNumber = Literal[1, 2, 3, 4, 5, 6, 7, 8, 9]
 
 
 def escape_sequence(
     code: str,
     subcode: str | None = None,
     *args: int,
 ) -> EscapeSequence:
@@ -163,15 +163,15 @@
     return _CSI_private("h", *args)
 
 
 def _disable_CSI(*args: int) -> EscapeSequence:
     return _CSI_private("l", *args)
 
 
-def _cursor_shape(n: int) -> EscapeSequence:
+def cursor_shape(n: int) -> EscapeSequence:
     return EscapeSequence(CHAR_ESC + f"[{n} q")
 
 
 # sequences
 def cursor_up(n: int = 1) -> EscapeSequence:
     return CSI("A", n)
 
@@ -196,15 +196,15 @@
     return CSI("F", n)
 
 
 def cursor_horizontal_absolute(n: int = 1) -> EscapeSequence:
     return CSI("G", n)
 
 
-def cursor_position(n: int, m: int = 1) -> EscapeSequence:
+def cursor_position(n: int = 1, m: int = 1) -> EscapeSequence:
     return CSI("H", n, m)
 
 
 def erase_in_display(n: int) -> EscapeSequence:
     return CSI("J", n)
 
 
@@ -245,21 +245,21 @@
 disable_alternative_screen_buffer = _disable_CSI(ALT_SCREEN_BUFFER)
 enable_bracketed_paste_mode = _enable_CSI(BRACKETED_PASTE_MODE)
 disable_bracketed_paste_mode = _disable_CSI(BRACKETED_PASTE_MODE)
 
 
 # *- Cursor shapes -* #
 
-user_defined_cursor_shape = _cursor_shape(0)
-blinking_block_cursor_shape = _cursor_shape(1)
-steady_block_cursor_shape = _cursor_shape(2)
-blinking_underline_cursor_shape = _cursor_shape(3)
-steady_underline_cursor_shape = _cursor_shape(4)
-blinking_bar_cursor_shape = _cursor_shape(5)
-steady_bar_cursor_shape = _cursor_shape(6)
+user_defined_cursor_shape = cursor_shape(0)
+blinking_block_cursor_shape = cursor_shape(1)
+steady_block_cursor_shape = cursor_shape(2)
+blinking_underline_cursor_shape = cursor_shape(3)
+steady_underline_cursor_shape = cursor_shape(4)
+blinking_bar_cursor_shape = cursor_shape(5)
+steady_bar_cursor_shape = cursor_shape(6)
 
 
 # aliases
 CUU = cursor_up
 CUD = cursor_down
 CUF = cursor_forward
 CUB = cursor_back
@@ -308,15 +308,15 @@
 invert = SGR(7)
 conceal = SGR(8)  # = hide
 crossed_out = SGR(9)
 primary_font = SGR(10)
 
 
 def alternative_font(n: AltFontNumber) -> EscapeSequence:
-    return SGR(n - 10)
+    return SGR(n + 10)
 
 
 fraktur = SGR(20)  # [RS]
 double_underline = SGR(21)  # THIS MIGHT DISABLE BOLD ON SOME TERMINALS
 normal_intensity = SGR(22)
 no_italic = SGR(23)
 no_underline = SGR(24)  # Also disables double underline
```

