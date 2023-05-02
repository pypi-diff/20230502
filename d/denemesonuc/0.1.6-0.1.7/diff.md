# Comparing `tmp/denemesonuc-0.1.6.tar.gz` & `tmp/denemesonuc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denemesonuc-0.1.6.tar", max compression
+gzip compressed data, was "denemesonuc-0.1.7.tar", max compression
```

## Comparing `denemesonuc-0.1.6.tar` & `denemesonuc-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/LICENSE
--rw-r--r--   0        0        0       67 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/README.md
--rw-r--r--   0        0        0      186 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/__init__.py
--rw-r--r--   0        0        0     3078 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/denek.py
--rw-r--r--   0        0        0     6501 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/fetch_new.py
--rw-r--r--   0        0        0     4982 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/fetch_old.py
--rw-r--r--   0        0        0     2736 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/models.py
--rw-r--r--   0        0        0      622 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 denemesonuc-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/LICENSE
+-rw-r--r--   0        0        0       67 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/README.md
+-rw-r--r--   0        0        0      186 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/__init__.py
+-rw-r--r--   0        0        0     3078 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/denek.py
+-rw-r--r--   0        0        0     6684 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/fetch_new.py
+-rw-r--r--   0        0        0     4982 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/fetch_old.py
+-rw-r--r--   0        0        0     2736 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/models.py
+-rw-r--r--   0        0        0      622 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 denemesonuc-0.1.7/PKG-INFO
```

### Comparing `denemesonuc-0.1.6/LICENSE` & `denemesonuc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.6/denemesonuc/denek.py` & `denemesonuc-0.1.7/denemesonuc/denek.py`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.6/denemesonuc/fetch_new.py` & `denemesonuc-0.1.7/denemesonuc/fetch_new.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from selenium.common.exceptions import NoSuchElementException, TimeoutException
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.ui import WebDriverWait
 
 import denemesonuc.models
 
 
 def fetch(
     driver: WebDriver,
@@ -28,25 +27,34 @@
     ret = denemesonuc.models.DenemeResult()
 
     if deneme.logout_url:
         driver.get(deneme.logout_url)
 
     driver.get(deneme.url)
 
+    def click_on_list_element(text_equal_to: str, *args, **kwargs):
+        ul = driver.find_element(*args, **kwargs)
+        li = ul.find_elements("tag name", "li")
+        for i in li:
+            if i.text == text_equal_to:
+                i.click()
+                return
+        raise RuntimeError(f"element with text {text_equal_to} not found")
+
     driver.find_element("id", "select2-gt_ogrencino_sinifcombo-container").click()
-    Select(driver.find_element("id", "select2-gt_ogrencino_sinifcombo-results")).select_by_visible_text(str(duzey) + ".Sınıf")
+    click_on_list_element(str(duzey) + ".Sınıf", "id", "select2-gt_ogrencino_sinifcombo-results")
 
     driver.find_element("id", "select2-gt_ogrencino_ilcombo-container").click()
-    Select(driver.find_element("id", "select2-gt_ogrencino_ilcombo-results")).select_by_visible_text(sehir)
+    click_on_list_element(sehir, "id", "select2-gt_ogrencino_ilcombo-results")
 
     driver.find_element("id", "select2-gt_ogrencino_ilcecombo-container").click()
-    Select(driver.find_element("id", "select2-gt_ogrencino_ilcecombo-results")).select_by_visible_text(ilce)
+    click_on_list_element(ilce, "id", "select2-gt_ogrencino_ilcecombo-results")
 
     driver.find_element("id", "select2-gt_ogrencino_kurumcombo-container").click()
-    Select(driver.find_element("id", "select2-gt_ogrencino_kurumcombo-results")).select_by_visible_text(kurum)
+    click_on_list_element(kurum, "id", "select2-gt_ogrencino_kurumcombo-results")
 
     ogrnoinp = driver.find_element("id", "gt_ogrencino_ogrnoedit")
     ogrnoinp.send_keys(str(no))
 
     # if it exists, type value
     for i in ("gt_ogrencino_adsoyadedit", "gt_ogrencino_adedit"):
         try:
```

### Comparing `denemesonuc-0.1.6/denemesonuc/fetch_old.py` & `denemesonuc-0.1.7/denemesonuc/fetch_old.py`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.6/denemesonuc/models.py` & `denemesonuc-0.1.7/denemesonuc/models.py`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.6/pyproject.toml` & `denemesonuc-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "denemesonuc"
-version = "0.1.6"
+version = "0.1.7"
 description = "orbim ölçme değerlendirme şeyi için bir modül"
 authors = ["insanolanbiri <erenakgun2007@hotmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com:/insanolanbiri/denemesonuc"
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `denemesonuc-0.1.6/PKG-INFO` & `denemesonuc-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denemesonuc
-Version: 0.1.6
+Version: 0.1.7
 Summary: orbim ölçme değerlendirme şeyi için bir modül
 Home-page: https://github.com:/insanolanbiri/denemesonuc
 License: GPL-3.0-only
 Author: insanolanbiri
 Author-email: erenakgun2007@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

