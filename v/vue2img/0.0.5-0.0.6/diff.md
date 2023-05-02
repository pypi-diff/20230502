# Comparing `tmp/vue2img-0.0.5.tar.gz` & `tmp/vue2img-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vue2img-0.0.5.tar", last modified: Tue May  2 04:28:23 2023, max compression
+gzip compressed data, was "vue2img-0.0.6.tar", last modified: Tue May  2 04:55:50 2023, max compression
```

## Comparing `vue2img-0.0.5.tar` & `vue2img-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 04:28:23.249497 vue2img-0.0.5/
--rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-24 03:40:26.000000 vue2img-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      746 2023-05-02 04:28:23.248507 vue2img-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.5/README.md
--rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 04:28:23.249497 vue2img-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-05-02 04:02:03.000000 vue2img-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:28:23.230561 vue2img-0.0.5/vue2img/
--rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.5/vue2img/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.5/vue2img/app.py
--rw-rw-rw-   0        0        0     9659 2023-04-24 03:04:14.000000 vue2img-0.0.5/vue2img/dom.py
--rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.5/vue2img/manager.py
--rw-rw-rw-   0        0        0     2098 2023-04-24 03:35:55.000000 vue2img-0.0.5/vue2img/operation.py
--rw-rw-rw-   0        0        0    24514 2023-04-24 03:38:11.000000 vue2img-0.0.5/vue2img/stopwords.py
--rw-rw-rw-   0        0        0     5167 2023-05-02 04:21:17.000000 vue2img-0.0.5/vue2img/template.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:28:23.246507 vue2img-0.0.5/vue2img.egg-info/
--rw-rw-rw-   0        0        0      746 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 04:55:50.942376 vue2img-0.0.6/
+-rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-24 03:40:26.000000 vue2img-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      746 2023-05-02 04:55:50.941379 vue2img-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.6/README.md
+-rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 04:55:50.942376 vue2img-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-05-02 04:55:42.000000 vue2img-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:55:50.896910 vue2img-0.0.6/vue2img/
+-rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.6/vue2img/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.6/vue2img/app.py
+-rw-rw-rw-   0        0        0     9784 2023-05-02 04:55:15.000000 vue2img-0.0.6/vue2img/dom.py
+-rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.6/vue2img/manager.py
+-rw-rw-rw-   0        0        0     2096 2023-05-02 04:55:34.000000 vue2img-0.0.6/vue2img/operation.py
+-rw-rw-rw-   0        0        0    24514 2023-04-24 03:38:11.000000 vue2img-0.0.6/vue2img/stopwords.py
+-rw-rw-rw-   0        0        0     5167 2023-05-02 04:21:17.000000 vue2img-0.0.6/vue2img/template.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:55:50.939398 vue2img-0.0.6/vue2img.egg-info/
+-rw-rw-rw-   0        0        0      746 2023-05-02 04:55:50.000000 vue2img-0.0.6/vue2img.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-02 04:55:50.000000 vue2img-0.0.6/vue2img.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 04:55:50.000000 vue2img-0.0.6/vue2img.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-02 04:55:50.000000 vue2img-0.0.6/vue2img.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 04:55:50.000000 vue2img-0.0.6/vue2img.egg-info/top_level.txt
```

### Comparing `vue2img-0.0.5/LICENSE` & `vue2img-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.5/PKG-INFO` & `vue2img-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.5
+Version: 0.0.6
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
```

### Comparing `vue2img-0.0.5/setup.py` & `vue2img-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf8") as f:
     requires = f.read()
 
 setup(
     name="vue2img",
-    version="0.0.5",
+    version="0.0.6",
     license="MIT",
     author="Drelf2018",
     author_email="drelf2018@outlook.com",
     description="通过 .vue 模板生成图片",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `vue2img-0.0.5/vue2img/app.py` & `vue2img-0.0.6/vue2img/app.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.5/vue2img/dom.py` & `vue2img-0.0.6/vue2img/dom.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,16 +234,21 @@
         src = self.attribute.get("src")
         if isinstance(src, str):
             res = httpx.get(self.src)
             data = BytesIO(res.content)
             img = Image.open(data)
         else:
             img = src
+
         self.height = img.height * self.width / img.width
-        self.img = img.resize((int(self.width), int(self.height)), Image.LANCZOS).convert("RGBA")
+        # 强制覆盖高度
+        height, = self.calc("height", self.height)
+        width = height * img.width / img.height
+
+        self.img = img.resize((int(width), int(height)), Image.LANCZOS).convert("RGBA")
 
     def paste(self, canvas: Image.Image, _: ImageDraw.ImageDraw, left: float, top: float):
         a = radiusMask(self.img.getchannel("A"), self.outside("border-radius"))
         canvas.paste(self.img, (int(left), int(top)), a)
 
 
 @dataclass
```

### Comparing `vue2img-0.0.5/vue2img/operation.py` & `vue2img-0.0.6/vue2img/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ).generate(sentence).to_image()
 
 
 def getCuttedBody(nanami: Image.Image):
     "返回下半身具有透明的图片"
 
     w = int(nanami.width * 600 / nanami.height)
-    nanami = nanami.resize((w, 600), Image.ANTIALIAS)
+    nanami = nanami.resize((w, 600), Image.LANCZOS)
     body = nanami.crop((0, 0, w, 400))  # 不是跟下半身切割了吗 上半身透明度保留
 
     a = body.getchannel('A')
     pix = a.load()
     for i in range(351, 400):
         for j in range(w):
             pix[j, i] = int((8-0.02*i) * pix[j, i])  # 下半部分透明度线性降低
```

### Comparing `vue2img-0.0.5/vue2img/stopwords.py` & `vue2img-0.0.6/vue2img/stopwords.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.5/vue2img/template.py` & `vue2img-0.0.6/vue2img/template.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.5/vue2img.egg-info/PKG-INFO` & `vue2img-0.0.6/vue2img.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.5
+Version: 0.0.6
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
```

