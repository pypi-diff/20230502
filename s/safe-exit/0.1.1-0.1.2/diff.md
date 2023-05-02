# Comparing `tmp/safe-exit-0.1.1.tar.gz` & `tmp/safe-exit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-exit-0.1.1.tar", last modified: Wed Apr 26 16:01:46 2023, max compression
+gzip compressed data, was "safe-exit-0.1.2.tar", last modified: Fri Apr 28 12:55:18 2023, max compression
```

## Comparing `safe-exit-0.1.1.tar` & `safe-exit-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-26 16:01:46.053489 safe-exit-0.1.1/
--rw-r--r--   0 zja        (501) staff       (20)     1072 2023-04-23 06:48:07.000000 safe-exit-0.1.1/LICENSE.txt
--rw-r--r--   0 zja        (501) staff       (20)     2894 2023-04-26 16:01:46.053617 safe-exit-0.1.1/PKG-INFO
--rw-r--r--   0 zja        (501) staff       (20)     2503 2023-04-26 15:58:15.000000 safe-exit-0.1.1/README.rst
-drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-26 16:01:46.050672 safe-exit-0.1.1/safe_exit/
--rw-r--r--   0 zja        (501) staff       (20)     7952 2023-04-26 02:46:59.000000 safe-exit-0.1.1/safe_exit/__init__.py
-drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-26 16:01:46.052569 safe-exit-0.1.1/safe_exit.egg-info/
--rw-r--r--   0 zja        (501) staff       (20)     2894 2023-04-26 16:01:46.000000 safe-exit-0.1.1/safe_exit.egg-info/PKG-INFO
--rw-r--r--   0 zja        (501) staff       (20)      289 2023-04-26 16:01:46.000000 safe-exit-0.1.1/safe_exit.egg-info/SOURCES.txt
--rw-r--r--   0 zja        (501) staff       (20)        1 2023-04-26 16:01:46.000000 safe-exit-0.1.1/safe_exit.egg-info/dependency_links.txt
--rw-r--r--   0 zja        (501) staff       (20)        7 2023-04-26 16:01:46.000000 safe-exit-0.1.1/safe_exit.egg-info/requires.txt
--rw-r--r--   0 zja        (501) staff       (20)       10 2023-04-26 16:01:46.000000 safe-exit-0.1.1/safe_exit.egg-info/top_level.txt
--rw-r--r--   0 zja        (501) staff       (20)      539 2023-04-26 16:01:46.054245 safe-exit-0.1.1/setup.cfg
--rw-r--r--   0 zja        (501) staff       (20)       38 2023-04-23 07:21:27.000000 safe-exit-0.1.1/setup.py
-drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-26 16:01:46.053240 safe-exit-0.1.1/tests/
--rw-r--r--   0 zja        (501) staff       (20)     2124 2023-04-26 02:54:01.000000 safe-exit-0.1.1/tests/test_safe_exit_posix.py
--rw-r--r--   0 zja        (501) staff       (20)     4077 2023-04-26 02:55:32.000000 safe-exit-0.1.1/tests/test_safe_exit_windows.py
+drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-28 12:55:18.819905 safe-exit-0.1.2/
+-rw-r--r--   0 zja        (501) staff       (20)     1072 2023-04-23 06:48:07.000000 safe-exit-0.1.2/LICENSE.txt
+-rw-r--r--   0 zja        (501) staff       (20)     2894 2023-04-28 12:55:18.820055 safe-exit-0.1.2/PKG-INFO
+-rw-r--r--   0 zja        (501) staff       (20)     2503 2023-04-26 15:58:15.000000 safe-exit-0.1.2/README.rst
+drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-28 12:55:18.816299 safe-exit-0.1.2/safe_exit/
+-rw-r--r--   0 zja        (501) staff       (20)     9365 2023-04-28 11:55:46.000000 safe-exit-0.1.2/safe_exit/__init__.py
+drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-28 12:55:18.818081 safe-exit-0.1.2/safe_exit.egg-info/
+-rw-r--r--   0 zja        (501) staff       (20)     2894 2023-04-28 12:55:18.000000 safe-exit-0.1.2/safe_exit.egg-info/PKG-INFO
+-rw-r--r--   0 zja        (501) staff       (20)      289 2023-04-28 12:55:18.000000 safe-exit-0.1.2/safe_exit.egg-info/SOURCES.txt
+-rw-r--r--   0 zja        (501) staff       (20)        1 2023-04-28 12:55:18.000000 safe-exit-0.1.2/safe_exit.egg-info/dependency_links.txt
+-rw-r--r--   0 zja        (501) staff       (20)        7 2023-04-28 12:55:18.000000 safe-exit-0.1.2/safe_exit.egg-info/requires.txt
+-rw-r--r--   0 zja        (501) staff       (20)       10 2023-04-28 12:55:18.000000 safe-exit-0.1.2/safe_exit.egg-info/top_level.txt
+-rw-r--r--   0 zja        (501) staff       (20)      539 2023-04-28 12:55:18.820697 safe-exit-0.1.2/setup.cfg
+-rw-r--r--   0 zja        (501) staff       (20)       38 2023-04-23 07:21:27.000000 safe-exit-0.1.2/setup.py
+drwxr-xr-x   0 zja        (501) staff       (20)        0 2023-04-28 12:55:18.819313 safe-exit-0.1.2/tests/
+-rw-r--r--   0 zja        (501) staff       (20)     2124 2023-04-26 02:54:01.000000 safe-exit-0.1.2/tests/test_safe_exit_posix.py
+-rw-r--r--   0 zja        (501) staff       (20)     4077 2023-04-26 02:55:32.000000 safe-exit-0.1.2/tests/test_safe_exit_windows.py
```

### Comparing `safe-exit-0.1.1/LICENSE.txt` & `safe-exit-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `safe-exit-0.1.1/PKG-INFO` & `safe-exit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-exit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Handle graceful process termination
 Home-page: https://github.com/ZhangJianAo/safe-exit
 Author: Zhang JianAo
 Author-email: zhangjianao@gmail.com
 License: MIT
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `safe-exit-0.1.1/README.rst` & `safe-exit-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `safe-exit-0.1.1/safe_exit/__init__.py` & `safe-exit-0.1.2/safe_exit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,27 +10,38 @@
 _logger = logging.getLogger("safe_exit")
 _registered = False
 _ctrl_handler = None
 _exit_funcs = []
 
 
 class ConfigFlag(Flag):
-    """Config Flags"""
+    """Configuration Flags:"""
     SIGQUIT = auto()
+    """Handle SIGQUIT signal."""
     SIGHUP = auto()
+    """Handle SIGHUP signal."""
     SIGBREAK = auto()
+    """Handle SIGBREAK signal."""
     CTRL_CLOSE = auto()
+    """Handle CTRL_CLOSE_EVENT."""
     CTRL_SHUTDOWN = auto()
+    """Handle CTRL_SHUTDOWN_EVENT."""
     CTRL_LOGOFF = auto()
+    """Handle CTRL_LOGOFF_EVENT."""
     AUTO_CREATE_CONSOLE = auto()
+    """Alloc a console and set it hidden."""
     FORCE_HIDE_CONSOLE = auto()
+    """If program is in a console, set the console hidden."""
 
 
 CONFIG_CTRL_ALL = ConfigFlag.CTRL_CLOSE | ConfigFlag.CTRL_SHUTDOWN | ConfigFlag.CTRL_LOGOFF
+"""All Windows ctrl events."""
+
 DEFAULT_CONFIG = ConfigFlag.SIGQUIT | ConfigFlag.SIGHUP | ConfigFlag.SIGBREAK | CONFIG_CTRL_ALL
+"""Default config: will handle all signals."""
 
 
 class WinCtrlEvent(IntEnum):
     CTRL_C_EVENT = 0
     CTRL_BREAK_EVENT = 1
     CTRL_CLOSE_EVENT = 2
     CTRL_LOGOFF_EVENT = 5
@@ -169,22 +180,32 @@
         except Exception as e:
             error_msg.append(str(e))
 
     raise SafeExitException(' and '.join(error_msg))
 
 
 def config(flag: ConfigFlag = DEFAULT_CONFIG):
-    """Config to register signals
+    """Configures which signals to register.
+
+    This function must be called before the register() function.
+
+    If the config() function is not called,
+    the register() function will automatically call this function with DEFAULT_CONFIG,
+    which will handle all signals.
 
-    There is no need to call this function on Linux or other POSIX systems,
-     this module will automatically register signal handlers.
-    On Windows, ```config(ConfigFlag.AUTO_CREATE_CONSOLE)``` will check if program attach to a console,
-     if not, it will alloc a console and set it to invisable.
-    If you want to hide the console window even the window is not alloc by program, add ConfigFlag.FORCE_HIDE_CONSOLE,
-     like ```config(ConfigFlag.AUTO_CREATE_CONSOLE | ConfigFlag.FORCE_HIDE_CONSOLE)```
+    Using this function allows you to control which signals to handle. SIGINT and SIGTERM are always handled,
+    and other signals can be set by this function.
+
+    On Windows,
+    ``config(DEFAULT_CONFIG | ConfigFlag.AUTO_CREATE_CONSOLE)`` checks if the program is attached to a console.
+    If not, it allocates a console and sets it to invisible.
+
+    If you want to hide the console window even if it is not allocated by the program,
+    add ConfigFlag.FORCE_HIDE_CONSOLE,
+    like ``config(DEFAULT_CONFIG | ConfigFlag.AUTO_CREATE_CONSOLE | ConfigFlag.FORCE_HIDE_CONSOLE)``.
 
     :param flag: Configuration flags
     :type flag: ConfigFlag
     """
     if os.name == 'nt':
         user32 = ctypes.windll.user32
         kernel32 = ctypes.windll.kernel32
@@ -200,41 +221,60 @@
             hwnd = kernel32.GetConsoleWindow()
             user32.ShowWindow(hwnd, 0)
 
     _register_signals(flag)
 
 
 def register(func, *args, **kwargs):
-    """Register function will call when program will exit
+    """Register func as a function to be executed at termination.
+
+    Any optional arguments that are to be passed to func must be passed as arguments to register().
 
-    This function can be used as function annot
+    This function can be used as function decorator.
     """
     if not _registered:
         config(DEFAULT_CONFIG)
     _exit_funcs.append((func, args, kwargs))
+    return func
 
 
 def unregister(func):
-    """Unregister function"""
+    """Remove func from the list of functions to be run at interpreter shutdown."""
     idx = 0
     while idx < len(_exit_funcs):
         if _exit_funcs[idx][0] == func:
             _exit_funcs.pop(idx)
         else:
             idx += 1
 
 
 def safe_kill(pid, kill_signal=None, timeout_secs=4, force_kill=True, silence=True):
-    """Graceful kill a process
+    """Gracefully kills a process.
+
+    :param pid: Process id to be killed.
+    :type pid: int
+
+    :param kill_signal: Which signal to send; can be None to use default signal
+    :type kill_signal: int
+
+    :param timeout_secs: How many seconds to wait for the process to terminate.
+    :type timeout_secs: int
+
+    :param force_kill: If True, force kill the process after timeout.
+    :type force_kill: bool
+
+    :param silence: If True, raise no exception if sending the signal results in an error.
+    :type silence: bool
+
+    This function first try to send kill_signal to the process,
+    and wait for timeout_secs, if the process still alive, it then forces kill it.
 
-    This function first try to send SIGTERM signal to the process,
-     and wait for timeout_secs, if the process still alive, then force kill it.
-    On windows, this function will try to find window for process, if found, it will send WM_CLOSE event,
-     if no window found, it will try to find console for process,
-     if found console, it will try to attach the console and send CTRL_C_EVENT to process.
+    On windows, this function tries to find a window for the process, if found, it sends the WM_CLOSE event.
+    If no window is found, it tries to find console for the process.
+    If a console is found, it tries to attach the console and sends the CTRL_C_EVENT to the process.
     """
     import psutil
 
     proc = psutil.Process(pid)
 
     try:
         if os.name == 'posix':
```

### Comparing `safe-exit-0.1.1/safe_exit.egg-info/PKG-INFO` & `safe-exit-0.1.2/safe_exit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-exit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Handle graceful process termination
 Home-page: https://github.com/ZhangJianAo/safe-exit
 Author: Zhang JianAo
 Author-email: zhangjianao@gmail.com
 License: MIT
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `safe-exit-0.1.1/setup.cfg` & `safe-exit-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = safe-exit
-version = 0.1.1
+version = 0.1.2
 license = MIT
 description = Handle graceful process termination
 long_description = file: README.rst
 author = Zhang JianAo
 author_email = zhangjianao@gmail.com
 url = https://github.com/ZhangJianAo/safe-exit
 classifiers =
```

### Comparing `safe-exit-0.1.1/tests/test_safe_exit_posix.py` & `safe-exit-0.1.2/tests/test_safe_exit_posix.py`

 * *Files identical despite different names*

### Comparing `safe-exit-0.1.1/tests/test_safe_exit_windows.py` & `safe-exit-0.1.2/tests/test_safe_exit_windows.py`

 * *Files identical despite different names*

