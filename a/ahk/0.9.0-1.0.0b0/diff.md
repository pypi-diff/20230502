# Comparing `tmp/ahk-0.9.0.tar.gz` & `tmp/ahk-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ahk-0.9.0.tar", last modified: Sat May 30 08:28:54 2020, max compression
+gzip compressed data, was "ahk-1.0.0b0.tar", last modified: Tue May  2 04:34:59 2023, max compression
```

## Comparing `ahk-0.9.0.tar` & `ahk-1.0.0b0.tar`

### file list

```diff
@@ -1,78 +1,38 @@
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/
--rw-rw-rw-   0        0        0     1078 2020-05-30 08:28:31.000000 ahk-0.9.0/LICENSE
--rw-rw-rw-   0        0        0       73 2020-05-30 08:28:31.000000 ahk-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0    16504 2020-05-30 08:28:54.000000 ahk-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2020-05-30 08:28:31.000000 ahk-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/
--rw-rw-rw-   0        0        0       94 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/__init__.py
--rw-rw-rw-   0        0        0     1645 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/autohotkey.py
--rw-rw-rw-   0        0        0     3324 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/directives.py
--rw-rw-rw-   0        0        0     7290 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/keyboard.py
--rw-rw-rw-   0        0        0     5557 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/keys.py
--rw-rw-rw-   0        0        0     7901 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/mouse.py
--rw-rw-rw-   0        0        0     3080 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/registery.py
--rw-rw-rw-   0        0        0     5978 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/screen.py
--rw-rw-rw-   0        0        0     7406 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/script.py
--rw-rw-rw-   0        0        0     2612 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/sound.py
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/templates/
--rw-rw-rw-   0        0        0      203 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/base.ahk
--rw-rw-rw-   0        0        0      105 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/hotkey.ahk
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/templates/keyboard/
--rw-rw-rw-   0        0        0      188 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/keyboard/key_state.ahk
--rw-rw-rw-   0        0        0      157 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/keyboard/key_wait.ahk
--rw-rw-rw-   0        0        0      151 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/keyboard/send.ahk
--rw-rw-rw-   0        0        0      130 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/keyboard/send_event.ahk
--rw-rw-rw-   0        0        0       80 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/keyboard/send_input.ahk
--rw-rw-rw-   0        0        0      129 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/keyboard/send_play.ahk
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/templates/mouse/
--rw-rw-rw-   0        0        0      133 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/mouse/click.ahk
--rw-rw-rw-   0        0        0      214 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/mouse/mouse_drag.ahk
--rw-rw-rw-   0        0        0      153 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/mouse/mouse_move.ahk
--rw-rw-rw-   0        0        0      167 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/mouse/mouse_position.ahk
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/templates/registery/
--rw-rw-rw-   0        0        0      106 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/registery/reg_delete.ahk
--rw-rw-rw-   0        0        0      106 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/registery/reg_loop.ahk
--rw-rw-rw-   0        0        0      136 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/registery/reg_read.ahk
--rw-rw-rw-   0        0        0       89 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/registery/reg_set_view.ahk
--rw-rw-rw-   0        0        0      123 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/registery/reg_write.ahk
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/templates/screen/
--rw-rw-rw-   0        0        0      313 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/screen/image_search.ahk
--rw-rw-rw-   0        0        0      239 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/screen/pixel_get_color.ahk
--rw-rw-rw-   0        0        0      327 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/screen/pixel_search.ahk
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/templates/sound/
--rw-rw-rw-   0        0        0      105 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/sound/beep.ahk
--rw-rw-rw-   0        0        0      134 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/sound/get_volume.ahk
--rw-rw-rw-   0        0        0      124 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/sound/play.ahk
--rw-rw-rw-   0        0        0      115 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/sound/set_volume.ahk
--rw-rw-rw-   0        0        0      167 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/sound/sound_get.ahk
--rw-rw-rw-   0        0        0      171 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/sound/sound_set.ahk
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk/templates/window/
--rw-rw-rw-   0        0        0      141 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/base_check.ahk
--rw-rw-rw-   0        0        0      147 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/base_command.ahk
--rw-rw-rw-   0        0        0      117 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/base_get_command.ahk
--rw-rw-rw-   0        0        0      174 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/control_send.ahk
--rw-rw-rw-   0        0        0      112 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/from_mouse.ahk
--rw-rw-rw-   0        0        0      185 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/get.ahk
--rw-rw-rw-   0        0        0      166 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/id_list.ahk
--rw-rw-rw-   0        0        0      129 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/set.ahk
--rw-rw-rw-   0        0        0      198 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/title_list.ahk
--rw-rw-rw-   0        0        0      106 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/win_click.ahk
--rw-rw-rw-   0        0        0      191 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/win_is_always_on_top.ahk
--rw-rw-rw-   0        0        0      181 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/win_move.ahk
--rw-rw-rw-   0        0        0      178 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/win_position.ahk
--rw-rw-rw-   0        0        0      196 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/win_send.ahk
--rw-rw-rw-   0        0        0      109 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/win_set.ahk
--rw-rw-rw-   0        0        0      116 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/templates/window/win_set_title.ahk
--rw-rw-rw-   0        0        0     1147 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/utils.py
--rw-rw-rw-   0        0        0    19393 2020-05-30 08:28:31.000000 ahk-0.9.0/ahk/window.py
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk.egg-info/
--rw-rw-rw-   0        0        0    16504 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1887 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2020-05-30 08:28:54.000000 ahk-0.9.0/ahk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-05-30 08:28:54.000000 ahk-0.9.0/docs/
--rw-rw-rw-   0        0        0    12262 2020-05-30 08:28:31.000000 ahk-0.9.0/docs/README.md
--rw-rw-rw-   0        0        0       81 2020-05-30 08:28:54.000000 ahk-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1122 2020-05-30 08:28:32.000000 ahk-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 04:34:49.000000 ahk-1.0.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-05-02 04:34:59.929923 ahk-1.0.0b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169734 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82888 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164017 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78237 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 04:34:49.000000 ahk-1.0.0b0/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-05-02 04:34:49.000000 ahk-1.0.0b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 04:34:49.000000 ahk-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-02 04:34:59.929923 ahk-1.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:34:49.000000 ahk-1.0.0b0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ahk-0.9.0/ahk/directives.py` & `ahk-1.0.0b0/ahk/directives.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 """
 Contains directive classes
 """
-
 from types import SimpleNamespace
+from typing import Any
+from typing import NoReturn
 
 
 class DirectiveMeta(type):
     """
     Overrides __str__ so directives with no arguments can be used without instantiation
     Overrides __hash__ to make objects 'unique' based upon a hash of the str representation
     """
-    def __str__(cls):
-        return f"#{cls.__name__}"
 
-    def __hash__(self):
+    def __str__(cls) -> str:
+        return f'#{cls.__name__}'
+
+    def __hash__(self) -> int:
         return hash(str(self))
 
-    def __eq__(cls, other):
-        return str(cls) == other
+    def __eq__(cls, other: Any) -> bool:
+        return bool(str(cls) == other)
 
 
 class Directive(SimpleNamespace, metaclass=DirectiveMeta):
     """
     Simple directive class
     They are designed to be hashable and comparable with string equivalent of AHK directive.
     Directives that don't require arguments do not need to be instantiated.
     """
-    def __init__(self, **kwargs):
+
+    def __init__(self, **kwargs: Any):
         super().__init__(name=self.name, **kwargs)
         self._kwargs = kwargs
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.__class__.__name__
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self._kwargs:
             arguments = ' '.join(str(value) for key, value in self._kwargs.items())
         else:
             arguments = ''
-        return f"#{self.name} {arguments}".rstrip()
+        return f'#{self.name} {arguments}'.rstrip()
 
-    def __eq__(self, other):
-        return str(self) == other
+    def __eq__(self, other: Any) -> bool:
+        return bool(str(self) == other)
 
-    def __hash__(self):
+    def __hash__(self) -> int:  # type: ignore[override]
         return hash(str(self))
 
 
 class AllowSameLineComments(Directive):
     pass
 
 
 class ClipboardTimeout(Directive):
-    def __init__(self, milliseconds=0, **kwargs):
+    def __init__(self, milliseconds: int = 0, **kwargs: Any):
         kwargs['milliseconds'] = milliseconds
         super().__init__(**kwargs)
 
 
 class ErrorStdOut(Directive):
     pass
 
@@ -67,95 +70,83 @@
 
 
 class HotKeyModifierTimeout(HotKeyInterval):
     pass
 
 
 class Include(Directive):
-    def __init__(self, include_name, **kwargs):
+    def __init__(self, include_name: str, **kwargs: Any):
         kwargs['include_name'] = include_name
         super().__init__(**kwargs)
 
 
 class IncludeAgain(Include):
     pass
 
 
 class InputLevel(Directive):
-    def __init__(self, level, **kwargs):
+    def __init__(self, level: int, **kwargs: Any):
         kwargs['level'] = level
         super().__init__(**kwargs)
 
 
 class InstallKeybdHook(Directive):
     pass
 
 
 class InstallMouseHook(Directive):
     pass
 
 
 class KeyHistory(Directive):
-    def __init__(self, limit=40, **kwargs):
+    def __init__(self, limit: int = 40, **kwargs: Any):
         kwargs['limit'] = limit
         super().__init__(**kwargs)
 
 
 class MaxHotkeysPerInterval(Directive):
-    def __init__(self, value, **kwargs):
+    def __init__(self, value: int, **kwargs: Any):
         kwargs['value'] = value
         super().__init__(**kwargs)
 
 
 class MaxMem(Directive):
-    def __init__(self, megabytes: int, **kwargs):
+    def __init__(self, megabytes: int, **kwargs: Any):
         if megabytes < 1:
             raise ValueError('megabytes cannot be less than 1')
         if megabytes > 4095:
             raise ValueError('megabytes cannot exceed 4095')
         kwargs['megabytes'] = megabytes
         super().__init__(**kwargs)
 
 
 class MaxThreads(Directive):
-    def __init__(self):
-        raise NotImplemented
+    def __init__(self) -> NoReturn:
+        raise NotImplementedError()
 
 
 class MaxThreadsBuffer(Directive):
-    def __init__(self):
-        raise NotImplemented
+    def __init__(self) -> NoReturn:
+        raise NotImplementedError()
 
 
 class MaxThreadsPerHotkey(Directive):
-    def __init__(self):
-        raise NotImplemented
+    def __init__(self) -> NoReturn:
+        raise NotImplementedError()
 
 
 class MenuMaskKey(Directive):
-    def __init__(self):
-        raise NotImplemented
-
-
-class NoEnv(Directive):
-    pass
+    def __init__(self) -> NoReturn:
+        raise NotImplementedError()
 
 
 class NoTrayIcon(Directive):
     pass
 
 
-class Persistent(Directive):
-    pass
-
-
-class SingleInstance(Directive):
-    pass
-
-
 class UseHook(Directive):
     pass
 
 
 class Warn(Directive):
     pass
```

