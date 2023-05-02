# Comparing `tmp/vigilant_kit-1.1.1.tar.gz` & `tmp/vigilant_kit-1.2.0.tar.gz`

## Comparing `vigilant_kit-1.1.1.tar` & `vigilant_kit-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/.vigilant.env.example
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/docs/actions.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/docs/browser_options.md
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/docs/native_selenium.md
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/docs/vigilant_unittest.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vgl_cli/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vgl_cli/local_dev.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vgl_cli/utils.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/LICENSE
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 vigilant_kit-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/.vigilant.env.example
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/actions.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/browser_options.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/native_selenium.md
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/run_selenium_command.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/PKG-INFO
```

### Comparing `vigilant_kit-1.1.1/docs/browser_options.md` & `vigilant_kit-1.2.0/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/docs/native_selenium.md` & `vigilant_kit-1.2.0/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/docs/selenium_install.md` & `vigilant_kit-1.2.0/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/docs/tutorial_pytest.md` & `vigilant_kit-1.2.0/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/docs/vigilant_pytest.md` & `vigilant_kit-1.2.0/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/docs/vigilant_unittest.md` & `vigilant_kit-1.2.0/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/src/vigilant/actions/assertions.py` & `vigilant_kit-1.2.0/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/src/vigilant/actions/finder.py` & `vigilant_kit-1.2.0/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.2.0/src/vigilant/actions/vigilant_actions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/src/vigilant/actions/waiter.py` & `vigilant_kit-1.2.0/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.0/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/.gitignore` & `vigilant_kit-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/LICENSE` & `vigilant_kit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/README.md` & `vigilant_kit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.1.1/pyproject.toml` & `vigilant_kit-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vigilant_kit-1.1.1/PKG-INFO` & `vigilant_kit-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vigilant_kit
-Version: 1.1.1
+Version: 1.2.0
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
```

