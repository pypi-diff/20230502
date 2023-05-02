# Comparing `tmp/hume-0.3.1b0.tar.gz` & `tmp/hume-0.3.20b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.3.1b0.tar", last modified: Wed May 29 19:46:41 2019, max compression
+gzip compressed data, was "hume-0.3.20b0.tar", last modified: Sat Jun  1 23:14:25 2019, max compression
```

## Comparing `hume-0.3.1b0.tar` & `hume-0.3.20b0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2019-05-28 18:43:24.499597 hume-0.3.1b0/LICENSE
--rw-r--r--   0        0        0     2025 2019-05-29 19:46:17.616602 hume-0.3.1b0/README.md
--rw-r--r--   0        0        0    72163 2019-05-28 18:24:11.503000 hume-0.3.1b0/docs/console_demo.png
--rw-r--r--   0        0        0       25 2019-05-28 11:29:38.076584 hume-0.3.1b0/hume/decorators/__init__.py
--rw-r--r--   0        0        0     4624 2019-05-29 19:17:11.511443 hume-0.3.1b0/hume/decorators/profilers.py
--rw-r--r--   0        0        0     1120 2019-05-29 19:46:03.478910 hume-0.3.1b0/pyproject.toml
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 hume-0.3.1b0/setup.py
--rw-r--r--   0        0        0     2966 1970-01-01 00:00:00.000000 hume-0.3.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2019-05-28 18:43:24.499597 hume-0.3.20b0/LICENSE
+-rw-r--r--   0        0        0     3712 2019-05-30 17:08:33.892698 hume-0.3.20b0/README.md
+-rw-r--r--   0        0        0    72163 2019-05-28 18:24:11.503000 hume-0.3.20b0/docs/console_demo.png
+-rw-r--r--   0        0        0       25 2019-05-28 11:29:38.076584 hume-0.3.20b0/hume/decorators/__init__.py
+-rw-r--r--   0        0        0     4764 2019-05-29 22:06:28.379043 hume-0.3.20b0/hume/decorators/profilers.py
+-rw-r--r--   0        0        0     1109 2019-06-01 23:12:11.740831 hume-0.3.20b0/pyproject.toml
+-rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 hume-0.3.20b0/setup.py
+-rw-r--r--   0        0        0     4642 1970-01-01 00:00:00.000000 hume-0.3.20b0/PKG-INFO
```

### Comparing `hume-0.3.1b0/LICENSE` & `hume-0.3.20b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.3.1b0/docs/console_demo.png` & `hume-0.3.20b0/docs/console_demo.png`

 * *Files identical despite different names*

### Comparing `hume-0.3.1b0/hume/decorators/profilers.py` & `hume-0.3.20b0/hume/decorators/profilers.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,26 +65,30 @@
         show_kwargs {bool} -- show the kwargs passed to the function (default: False)
         show_result {bool} -- show the return value of the decorated function (default: False)
         mute_console {bool} -- supress print statements from the decorated function (default: False)
     
     Returns:
         the return value of func(*args, **kwargs) when func() is wrapped 
     """
+    # there must be a better way
     try:
         nums = profile.explicit_args[0]
     except IndexError:
         nums = CONFIG.get("nums", profile.defaults.get("nums"))
 
     item_names = [x for x in profile.defaults.keys() if x != "nums"]
     items = [show_args, show_kwargs, show_result, mute_console]
+
     for index, (item_name, item_value) in enumerate(zip(item_names, items)):
         items[index] = profile.explicit_kwargs.get(
             item_name, CONFIG.get(item_name, profile.defaults.get(item_name))
         )
 
+    show_args, show_kwargs, show_result, mute_console = items
+
     def middle(func):
         is_evaluating = False
         # start evaluating recursion after funciton definition
         _, lines = inspect.getsource(func).split(f"{func.__name__}", 1)
         # take the docs out in case they include the function name
         lines = lines.replace(str(func.__doc__), "")
 
@@ -93,15 +97,15 @@
         )  # pylint: disable=all
 
         if func.__name__ in lines:
             pre_message += (
                 f"{fg.li_yellow}{ef.b}(recursive function detected) {fg.rs}{rs.all}"
             )
 
-        pre_message += "\n------------"
+        pre_message += "\n------------------------------------------------"
 
         print(pre_message, end="")
 
         def wrapper(*args, **kwargs):
             nonlocal is_evaluating
             f = io.StringIO()
             stdout = ""
@@ -113,15 +117,15 @@
                 def timing_func():
                     with HiddenPrints():
                         func(*args, **kwargs)
 
                 is_evaluating = True
                 timings = timeit.repeat(stmt=timing_func, repeat=nums, number=1)
 
-                av = sum(timings) / len(timings)
+                av = sum(timings) / float(len(timings))
 
                 timing_str = f"→ name: {func.__name__}"
                 if show_args:
                     timing_str += f"\n→ args: {args}"
                 if show_kwargs:
                     timing_str += f"\n→ kwargs: {kwargs}"
```

### Comparing `hume-0.3.1b0/pyproject.toml` & `hume-0.3.20b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "hume"
-version = "0.3.1b"
+version = "0.3.20b"
 description = "really simple profiling for mere mortals"
-authors = ["Shibel K. Mansour <hi@shibel.com>"]
+authors = ["SHxKM <hi@shibel.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SHxKM/hume"
 repository = "https://github.com/SHxKM/hume"
 documentation = "https://github.com/SHxKM/hume/blob/master/README.md"
 keywords = ["profiling", "profile", "timing"]
```

### Comparing `hume-0.3.1b0/PKG-INFO` & `hume-0.3.20b0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,125 @@
-Metadata-Version: 2.1
-Name: hume
-Version: 0.3.1b0
-Summary: really simple profiling for mere mortals
-Home-page: https://github.com/SHxKM/hume
-License: MIT
-Keywords: profiling,profile,timing
-Author: Shibel K. Mansour
-Author-email: hi@shibel.com
-Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Utilities
-Requires-Dist: sty (>=1.0-beta.1,<2.0)
-Project-URL: Documentation, https://github.com/SHxKM/hume/blob/master/README.md
-Project-URL: Repository, https://github.com/SHxKM/hume
-Description-Content-Type: text/markdown
+# hume - simple & quick profiling for mere mortals
 
-# hume - simple & quick profiling for mortals
+hume is a fun-expirement turned Python package. In short, it exposes a decorator `profile` that you can use to measure 
+the execution time of functions. It goes out of its way to make its protocol clear, usage simple, and configuration flexible. 
 
+Like many profiling libraries, hume adds overhead which means its measurements are (often) slower than real execution time when testing small pieces of code. **Don't** use it for super-scientific benchmarking.
+
+**Note:** Python >= 3.6 required.
 
 ## Installation
 
 You can install `hume` from [PyPI](https://pypi.org/):
 
     pip install hume
 
-**Note:** Python >= 3.6 required.
+or:
+
+    pipenv install hume
 
 ## ★ hume.decorators
 
 ### ★★ profile
 
 A simple decorator to measure function execution times. 
 
 - Supports N simulations and average times. 
 - Supports, recognizes, and reports recursive functions.
 - (optional) List `args` and `kwargs` as provided to the decorated function.
 - (optional) Display the decorated function's return value
 - (optional) Supress `print` statements in decorated functions (default is `False`, output is only reported for one simulation)
 
-#### ★★★ how to use
+
+`profile` does not in any way modify what's returned by the decorated function. The only thing it will possibly augment are `print` statements.
+
+#### ★★★ usage
 
 Simply decorate any function:
 
 ```python
 from hume.decorators import profile
 
-@profile(nums=3)
+@profile(6)
 def slow_add(num):
-    """slow_add does somethig
     """
+    slow_add sleeps one second and returns num + 1
+    """
+
     time.sleep(1)
-    return num
+    return num + 1
 
 print(slow_add(3))
 ```
 
 And let it do its job:
 
 ```terminal
 profiling slow_add 
-------------
+------------------------------------------------
 → name: slow_add
-→ simulations: 3
-→ average execution time: 1.0033866766666666 seconds
+→ simulations: 6
+→ average execution time: 1.0034156345 seconds
 
-3
+4
 ```
 
+#### ★★★ options and defaults
+
 `profile` supports the following params:
 
 - `nums: int = 1` → how many simulations to conduct
 - `show_args: bool = False` → display `args` passed to the decorated function
 - `show_kwargs: bool = False` →  display `kwargs` passed to the decorated function
 - `show_result: bool = False` →  display decorated function return value
-- `mute_console: bool = False` →  supress `print` statements from the decorated function
+- `mute_console: bool = False` →  supress `print` statements inside the decorated function's body. Useful when you have a bunch of these that you don't want to remove just for the sake of measurement.<sup>1</sup>
+
+<span style="font-size:12px;"><sup>1</sup> Even if `mute_console` is `False`, recursive functions will print normally and not per `nums`.</small>
 
 #### ★★★ recursion
 
 For recursive functions, `profile` just knows (and doesn't pollute the console):
 
 ```python
 # recursive function
-@profile(7)
+@profile(2)
 def factorial(n):
     if n == 1:
         return 1
     return n * factorial(n - 1)
 
 
-print(factorial(3))
+factorial(3)
 ```
 
 ```terminal
 profiling factorial (recursive function detected) 
-------------
+------------------------------------------------
 → name: factorial
-→ simulations: 7
-→ average execution time: 3.6912857141706875e-06 seconds
+→ simulations: 2
+→ average execution time: 0.00011469949999964868 seconds
+```
+
+#### ★★★ changing & overriding defaults
+
+If you don't like `profile`'s [default configuration](#-options-and-defaults), you can import the `CONFIG` dict and override them. For example, if you want `profile` to include the `return` from the decorated function by default, you would do the following:
+
+```python
+from hume.decorators import profile, CONFIG
+
+CONFIG["show_results"] = True
 
-6
+@profile(2)
+def return_one():
+    return 1
+
+# you can always override your own defaults:
+@profile(show_result=False)
+def return_two_ignored():
+    return 2
 ```
 
 #### ★★★ colorized output
 
-Output is colorized:
+Output is colorized, because priorities:
 
-![console output demo](/docs/console_demo.png)
+![console output demo](https://raw.githubusercontent.com/SHxKM/hume/master/docs/console_demo.png?token=ABSE3IVTPJ6CWFRQUHSW75C47APAU)
```

