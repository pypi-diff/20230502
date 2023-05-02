# Comparing `tmp/e-models-1.1.1.tar.gz` & `tmp/e-models-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.1.1.tar", last modified: Wed Apr 19 14:04:04 2023, max compression
+gzip compressed data, was "e-models-1.2.tar", last modified: Tue May  2 19:27:03 2023, max compression
```

## Comparing `e-models-1.1.1.tar` & `e-models-1.2.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.703922 e-models-1.1.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.1.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-04-19 14:04:04.703922 e-models-1.1.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.1.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.699922 e-models-1.1.1/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      447 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       17 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.699922 e-models-1.1.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-04-19 14:03:03.000000 e-models-1.1.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.1.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.703922 e-models-1.1.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34187 2023-04-19 14:01:20.000000 e-models-1.1.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.1.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.1.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.1.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.1.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.1.1/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7028 2023-04-19 13:53:58.000000 e-models-1.1.1/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.1.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-19 14:04:04.703922 e-models-1.1.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      928 2023-04-19 14:02:56.000000 e-models-1.1.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.703922 e-models-1.1.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7946 2023-04-19 14:00:24.000000 e-models-1.1.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 19:27:03.020428 e-models-1.2/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.2/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3268 2023-05-02 19:27:03.020428 e-models-1.2/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.2/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 19:27:03.016429 e-models-1.2/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3268 2023-05-02 19:27:02.000000 e-models-1.2/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      527 2023-05-02 19:27:02.000000 e-models-1.2/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-02 19:27:02.000000 e-models-1.2/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       16 2023-05-02 19:27:02.000000 e-models-1.2/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-02 19:27:02.000000 e-models-1.2/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 19:27:03.016429 e-models-1.2/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2023-05-02 19:18:39.000000 e-models-1.2/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.2/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 19:27:03.016429 e-models-1.2/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34436 2023-04-29 13:57:12.000000 e-models-1.2/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.2/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.2/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.2/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.2/emodels/html2text/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 19:27:03.016429 e-models-1.2/emodels/markdown/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 18:53:53.000000 e-models-1.2/emodels/markdown/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8278 2023-05-02 19:24:09.000000 e-models-1.2/emodels/markdown/tables.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.2/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7223 2023-05-02 19:24:43.000000 e-models-1.2/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.2/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-02 19:27:03.020428 e-models-1.2/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      925 2023-05-02 19:18:31.000000 e-models-1.2/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 19:27:03.020428 e-models-1.2/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2846 2023-05-02 18:50:14.000000 e-models-1.2/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7947 2023-05-02 16:31:36.000000 e-models-1.2/tests/test_scrapyutils.py
```

### Comparing `e-models-1.1.1/LICENSE` & `e-models-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.1.1/PKG-INFO` & `e-models-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.1.1
+Version: 1.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.1.1/README.md` & `e-models-1.2/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.1.1/e_models.egg-info/PKG-INFO` & `e-models-1.2/e_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.1.1
+Version: 1.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.1.1/emodels/html2text/__init__.py` & `e-models-1.2/emodels/html2text/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         """
         super().__init__(convert_charrefs=False)
 
         # Config options
         self.split_next_td = False
         self.td_count = 0
         self.table_start = False
+        self.table_header = False
         self.unicode_snob = config.UNICODE_SNOB  # covered in cli
         self.escape_snob = config.ESCAPE_SNOB  # covered in cli
         self.links_each_paragraph = config.LINKS_EACH_PARAGRAPH
         self.body_width = bodywidth  # covered in cli
         self.skip_internal_links = config.SKIP_INTERNAL_LINKS  # covered in cli
         self.inline_links = config.INLINE_LINKS  # covered in cli
         self.protect_links = config.PROTECT_LINKS  # covered in cli
@@ -628,29 +629,34 @@
                         if self.pad_tables:
                             self.o("<" + config.TABLE_MARKER_FOR_PAD + ">")
                             self.o("  \n")
                     else:
                         if self.pad_tables:
                             self.o("</" + config.TABLE_MARKER_FOR_PAD + ">")
                             self.o("  \n")
+                if tag == "th" and self.table_start:
+                    self.table_header = True
                 if tag in ["td", "th"] and start:
                     if self.split_next_td:
                         self.o("| ")
                     self.split_next_td = True
 
                 if tag == "tr" and start:
                     self.td_count = 0
+                    self.o("| ")
                 if tag == "tr" and not start:
                     self.split_next_td = False
-                    self.soft_br()
-                if tag == "tr" and not start and self.table_start:
+                    self.o("|")
+                    self.pbr()
+                if tag == "tr" and not start and self.table_header:
                     # Underline table header
-                    self.o("|".join(["---"] * self.td_count))
-                    self.soft_br()
+                    self.o("| " + "|".join(["---"] * self.td_count) + "|")
+                    self.pbr()
                     self.table_start = False
+                    self.table_header = False
                 if tag in ["td", "th"] and start:
                     self.td_count += 1
 
         if tag == "pre":
             if start:
                 self.startpre = True
                 self.pre = True
```

### Comparing `e-models-1.1.1/emodels/html2text/config.py` & `e-models-1.2/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.1.1/emodels/html2text/utils.py` & `e-models-1.2/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.1.1/emodels/scrapyutils.py` & `e-models-1.2/emodels/scrapyutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import re
 import os
 import json
 import gzip
 from typing import NewType, Dict, Tuple, List, Optional
 
-from markdown2 import Markdown
-
+from markdown import Markdown
 from scrapy.loader import ItemLoader
 from scrapy.http import TextResponse
 from scrapy import Item
 
 from emodels.config import EMODELS_ITEMS_DIR, EMODELS_SAVE_EXTRACT_ITEMS
+from emodels.markdown.tables import TableExtension
 from emodels import html2text
 
 
 MARKDOWN_LINK_RE = re.compile(r"\[(.+?)\]\((.+?)\s*(\".+\")?\)")
 LINK_RSTRIP_RE = re.compile("(%20)+$")
 LINK_LSTRIP_RE = re.compile("^(%20)+")
 COMMENT_RE = re.compile(r"\s<!--.+?-->")
@@ -61,14 +61,18 @@
         """Generate multiple responses from provided xpath selector"""
         result = []
         for html in self.xpath(selector).extract():
             new = self.replace(body=html.encode("utf-8"))
             result.append(new)
         return result
 
+    def markdown_to_html(self, text: Optional[str] = None):
+        text = text or self.markdown
+        return Markdown(extensions=[TableExtension()]).convert(text).strip()
+
     @staticmethod
     def _clean_markdown(md: str):
         shrink = 0
         for m in MARKDOWN_LINK_RE.finditer(md):
             if m.groups()[1] is not None:
                 start = m.start(2) - shrink
                 end = m.end(2) - shrink
@@ -145,15 +149,14 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         assert "response" in self.context, '"response" is required.'
         if not isinstance(self.context["response"], ExtractTextResponse):
             self.context["response"] = self.context["response"].replace(cls=ExtractTextResponse)
         self.extract_indexes: ExtractDict = ExtractDict({})
-        self._mconverter = Markdown()
 
     def add_text_re(
         self,
         attr: str,
         reg: str = "(.+?)",
         tid: Optional[str] = None,
         flags: int = 0,
@@ -172,15 +175,15 @@
                 self.add_value(attr, t, *processors, **kw)
 
     def add_text_re_as_html(self, attr: str, reg: str, flags: int = 0, *processors, **kw):
         extracted = self.context["response"].text_re(reg, flags=flags, optimize=True)
         if extracted:
             t, s, e = extracted[0]
             if attr not in self.extract_indexes:
-                cleaned = self._mconverter.convert(t).strip()
+                cleaned = self.context["response"].markdown_to_html(t)
                 self.add_value(attr, cleaned, *processors, **kw)
                 self.extract_indexes[attr] = (s, e)
 
     def load_item(self) -> Item:
         item = super().load_item()
         self._save_extract_sample()
         return item
```

### Comparing `e-models-1.1.1/setup.py` & `e-models-1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.1.1',
+    version      = '1.2',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
     packages     = find_packages(),
     install_requires=(
         "scrapy",
-        "markdown2",
+        "markdown",
     ),
     scripts = [],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
```

### Comparing `e-models-1.1.1/tests/test_scrapyutils.py` & `e-models-1.2/tests/test_scrapyutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         )
         self.assertEqual(
             item["description"][-80:],
             "arning skills.\n\n\n\n**Please note, all employment postings close at 11:55pm CST.**",
         )
         self.assertEqual(
             item["description_as_html"][:80],
-            "<h3>Student Athlete Support Services Coord</h3>\n\n<ul>\n<li><p>__ 492556 </p></li>",
+            "<h3>Student Athlete Support Services Coord</h3>\n<ul>\n<li>\n<p>__ 492556 </p>\n</li",
         )
         self.assertEqual(
             item["description_as_html"][-80:],
             "><strong>Please note, all employment postings close at 11:55pm CST.</strong></p>",
         )
 
         response = loader.context["response"]
```

