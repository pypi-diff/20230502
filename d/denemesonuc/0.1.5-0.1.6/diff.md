# Comparing `tmp/denemesonuc-0.1.5.tar.gz` & `tmp/denemesonuc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denemesonuc-0.1.5.tar", max compression
+gzip compressed data, was "denemesonuc-0.1.6.tar", max compression
```

## Comparing `denemesonuc-0.1.5.tar` & `denemesonuc-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/LICENSE
--rw-r--r--   0        0        0       67 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/README.md
--rw-r--r--   0        0        0      186 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/denemesonuc/__init__.py
--rw-r--r--   0        0        0     3012 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/denemesonuc/denek.py
--rw-r--r--   0        0        0     6329 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/denemesonuc/fetch_new.py
--rw-r--r--   0        0        0     4982 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/denemesonuc/fetch_old.py
--rw-r--r--   0        0        0     2736 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/denemesonuc/models.py
--rw-r--r--   0        0        0      622 2023-03-16 15:32:11.039503 denemesonuc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 denemesonuc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/LICENSE
+-rw-r--r--   0        0        0       67 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/README.md
+-rw-r--r--   0        0        0      186 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/__init__.py
+-rw-r--r--   0        0        0     3078 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/denek.py
+-rw-r--r--   0        0        0     6501 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/fetch_new.py
+-rw-r--r--   0        0        0     4982 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/fetch_old.py
+-rw-r--r--   0        0        0     2736 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/denemesonuc/models.py
+-rw-r--r--   0        0        0      622 2023-05-02 15:01:39.127392 denemesonuc-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 denemesonuc-0.1.6/PKG-INFO
```

### Comparing `denemesonuc-0.1.5/LICENSE` & `denemesonuc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.5/denemesonuc/denek.py` & `denemesonuc-0.1.6/denemesonuc/denek.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,74 +9,75 @@
     """# denemeye giren kişi. denek.
 
     `fetchDeneme`: verilen denemenin sonuçlarını çeker
     `getDeneme`: çekilen deneme sonucunu döndürür"""
 
     def __init__(
         self,
-        driver: WebDriver,
         ad: str,
         no: int,
         sinif_duzeyi: int,
         sehir: str,
         ilce: str,
         kurum: str,
     ) -> None:
         """### denek bilgileri
 
         `ad`: ad
         `no`: numara
         `sinif_duzeyi`: sınıf düzeyi
         `sehir`: şehir, tamamı büyük harf olmalı
         `kurum`: okulun adı"""
-        self.__driver = driver
         self.ad = ad
         self.no = no
         self.sinif_duzeyi = sinif_duzeyi
         self.sehir = (
             sehir.replace("ı", "I").replace("i", "İ").upper()
         )  # pythonın localeler ile sorunu var
         self.ilce = ilce.replace("ı", "I").replace("i", "İ").upper()
         self.kurum = kurum
         self.__deneme: dict[str, denemesonuc.models.DenemeResult] = {}
 
     def __repr__(self) -> str:
         """can sıkıntısı. denekleri stringe çevirmek için. abracadabra"""
         return f"Denek: {self.no} ({self.ad})"
 
-    def fetchDeneme(self, deneme: denemesonuc.models.DenemeLogin) -> int:
+    def fetchDeneme(self, driver: WebDriver, deneme: denemesonuc.models.DenemeLogin, **fetchkwargs) -> int:
         """### denek ve deneme bilgileriyle deneme sonuçlarını çeker
 
+        `driver`: selenium driver
         `deneme`: istenen deneme
 
         return:
         - 0: çekme başarılı
         - 1:
         - 2: denek denemeye girmemiş"""
         try:
             if deneme.deneme_type == "old":
                 self.__deneme[deneme.deneme_adi] = denemesonuc.fetch_old.fetch(
-                    self.__driver,
+                    driver,
                     self.ad,
                     self.no,
                     self.sinif_duzeyi,
                     self.sehir,
                     self.kurum,
                     deneme,
+                    **fetchkwargs,
                 )
             else:
                 self.__deneme[deneme.deneme_adi] = denemesonuc.fetch_new.fetch(
-                    self.__driver,
+                    driver,
                     self.ad,
                     self.no,
                     self.sinif_duzeyi,
                     self.sehir,
                     self.ilce,
                     self.kurum,
                     deneme,
+                    **fetchkwargs,
                 )
         except denemesonuc.models.DenekNotFound:
             return 2
         return 0
 
     def getDenemeList(self) -> list[str]:
         """### girilen denemelerin adlarının listesini döndürür"""
```

### Comparing `denemesonuc-0.1.5/denemesonuc/fetch_new.py` & `denemesonuc-0.1.6/denemesonuc/fetch_new.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 from selenium.common.exceptions import NoSuchElementException, TimeoutException
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.ui import WebDriverWait
 
 import denemesonuc.models
 
 
 def fetch(
     driver: WebDriver,
     ad: str,
     no: int,
     duzey: int,
     sehir: str,
     ilce: str,
     kurum: str,
     deneme: denemesonuc.models.DenemeLogin,
+    starting_div: int = 8,
+    naming_aliases: dict[str, str] = {},
 ) -> denemesonuc.models.DenemeResult:
     """### denek ve deneme bilgileriyle yeni tip deneme sonuçlarını çeker
 
     returns DenemeResult if successful
     raises DenekNotFound if denek did not take the test
     raises RunTimeError if element with text not found on login page"""
 
     ret = denemesonuc.models.DenemeResult()
 
     if deneme.logout_url:
         driver.get(deneme.logout_url)
 
     driver.get(deneme.url)
 
-    def click_on_list_element(text_equal_to: str, *args, **kwargs):
-        ul = driver.find_element(*args, **kwargs)
-        li = ul.find_elements("tag name", "li")
-        for i in li:
-            if i.text == text_equal_to:
-                i.click()
-                return
-        raise RuntimeError(f"element with text {text_equal_to} not found")
-
     driver.find_element("id", "select2-gt_ogrencino_sinifcombo-container").click()
-    click_on_list_element(str(duzey) + ".Sınıf", "id", "select2-gt_ogrencino_sinifcombo-results")
+    Select(driver.find_element("id", "select2-gt_ogrencino_sinifcombo-results")).select_by_visible_text(str(duzey) + ".Sınıf")
 
     driver.find_element("id", "select2-gt_ogrencino_ilcombo-container").click()
-    click_on_list_element(sehir, "id", "select2-gt_ogrencino_ilcombo-results")
+    Select(driver.find_element("id", "select2-gt_ogrencino_ilcombo-results")).select_by_visible_text(sehir)
 
     driver.find_element("id", "select2-gt_ogrencino_ilcecombo-container").click()
-    click_on_list_element(ilce, "id", "select2-gt_ogrencino_ilcecombo-results")
+    Select(driver.find_element("id", "select2-gt_ogrencino_ilcecombo-results")).select_by_visible_text(ilce)
 
     driver.find_element("id", "select2-gt_ogrencino_kurumcombo-container").click()
-    click_on_list_element(kurum, "id", "select2-gt_ogrencino_kurumcombo-results")
+    Select(driver.find_element("id", "select2-gt_ogrencino_kurumcombo-results")).select_by_visible_text(kurum)
 
     ogrnoinp = driver.find_element("id", "gt_ogrencino_ogrnoedit")
     ogrnoinp.send_keys(str(no))
 
     # if it exists, type value
-    try:
-        adinp = driver.find_element("id", "gt_ogrencino_adedit")
-        adinp.send_keys(ad)
-    except NoSuchElementException:
-        pass
+    for i in ("gt_ogrencino_adsoyadedit", "gt_ogrencino_adedit"):
+        try:
+            adinp = driver.find_element("id", i)
+            adinp.send_keys(ad)
+        except NoSuchElementException:
+            pass
 
     driver.find_element("id", "gt_ogrencino_girisbtn").submit()
 
     try:
         WebDriverWait(driver, 6).until(
             EC.presence_of_element_located(("xpath", "/html/body/section/div/div[1]/div/div/h6[2]"))
         )
@@ -104,15 +99,15 @@
             "xpath", f"/html/body/section/div[1]/div[3]/div/div/div/div[2]"
         ).text.replace(",", ".")
     )
 
     ul = driver.find_element("xpath", f"{document}/div[1]")
     li = ul.find_elements("tag name", "div")
 
-    i = 23 - 1
+    i = starting_div - 1
     available_heads = {}
     while True:
         i += 1
         try:
             driver.find_element("xpath", f"{document}/div[1]/div[{i}]")
         except NoSuchElementException:
             break
@@ -156,24 +151,21 @@
             int(
                 driver.find_element(
                     "xpath", f"{document}/div[1]/div[{i+1}]/div[1]/div/div/h{h}"
                 ).text
             ),
         )
 
-    def getDers(name: str = "") -> denemesonuc.models.DersSonuc | None:
-        """#### dersleri tek tek toplamak yerine yazılmış fonksiyon"""
-        return available_heads[name] if name in available_heads else None
-
-    ret.genel = getDers("Toplam")
-    ret.edb = getDers("TYT Türkçe Testi Toplamı")
-    ret.trh = getDers("Tarih-1")
-    ret.cog = getDers("Coğrafya-1")
-    ret.din = getDers("Din Kül. ve Ahl. Bil.")
-    ret.mat = getDers("TYT Matematik Testi Toplamı")
-    ret.fiz = getDers("Fizik")
-    ret.kim = getDers("Kimya")
-    ret.biy = getDers("Biyoloji")
-    ret.fel = getDers("Felsefe")
-    ret.sfl = getDers("Felsefe (Seçmeli)")
+    ret.genel = available_heads.get(naming_aliases.get("genel", "Toplam"))
+    ret.edb = available_heads.get(naming_aliases.get("edb", "TYT Türkçe Testi Toplamı"))
+    ret.trh = available_heads.get(naming_aliases.get("trh", "Tarih-1"))
+    ret.cog = available_heads.get(naming_aliases.get("cog", "Coğrafya-1"))
+    ret.din = available_heads.get(naming_aliases.get("din", "Din Kül. ve Ahl. Bil."))
+    ret.mat = available_heads.get(naming_aliases.get("mat", "TYT Matematik Testi Toplamı"))
+    ret.fiz = available_heads.get(naming_aliases.get("fiz", "Fizik"))
+    ret.kim = available_heads.get(naming_aliases.get("kim", "Kimya"))
+    ret.biy = available_heads.get(naming_aliases.get("biy", "Biyoloji"))
+    ret.fel = available_heads.get(naming_aliases.get("fel", "Felsefe"))
+    ret.sfl = available_heads.get(naming_aliases.get("sfl", "Felsefe (Seçmeli)"))
+
 
     return ret
```

### Comparing `denemesonuc-0.1.5/denemesonuc/fetch_old.py` & `denemesonuc-0.1.6/denemesonuc/fetch_old.py`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.5/denemesonuc/models.py` & `denemesonuc-0.1.6/denemesonuc/models.py`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.5/pyproject.toml` & `denemesonuc-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "denemesonuc"
-version = "0.1.5"
+version = "0.1.6"
 description = "orbim ölçme değerlendirme şeyi için bir modül"
 authors = ["insanolanbiri <erenakgun2007@hotmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com:/insanolanbiri/denemesonuc"
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `denemesonuc-0.1.5/PKG-INFO` & `denemesonuc-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denemesonuc
-Version: 0.1.5
+Version: 0.1.6
 Summary: orbim ölçme değerlendirme şeyi için bir modül
 Home-page: https://github.com:/insanolanbiri/denemesonuc
 License: GPL-3.0-only
 Author: insanolanbiri
 Author-email: erenakgun2007@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

