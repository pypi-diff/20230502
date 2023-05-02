# Comparing `tmp/jatsgenerator-0.5.0.tar.gz` & `tmp/jatsgenerator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jatsgenerator-0.5.0.tar", last modified: Wed Sep 28 05:25:13 2022, max compression
+gzip compressed data, was "jatsgenerator-0.6.0.tar", last modified: Tue May  2 02:24:54 2023, max compression
```

## Comparing `jatsgenerator-0.5.0.tar` & `jatsgenerator-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-28 05:25:13.865237 jatsgenerator-0.5.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5752 2022-09-28 05:25:13.865237 jatsgenerator-0.5.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5253 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-28 05:25:13.865237 jatsgenerator-0.5.0/jatsgenerator/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       22 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/jatsgenerator/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    21503 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/jatsgenerator/build.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1531 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/jatsgenerator/conf.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    15894 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/jatsgenerator/generate.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     3093 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/jatsgenerator/utils.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-28 05:25:13.865237 jatsgenerator-0.5.0/jatsgenerator.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5752 2022-09-28 05:25:13.000000 jatsgenerator-0.5.0/jatsgenerator.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      359 2022-09-28 05:25:13.000000 jatsgenerator-0.5.0/jatsgenerator.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2022-09-28 05:25:13.000000 jatsgenerator-0.5.0/jatsgenerator.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       68 2022-09-28 05:25:13.000000 jatsgenerator-0.5.0/jatsgenerator.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       14 2022-09-28 05:25:13.000000 jatsgenerator-0.5.0/jatsgenerator.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      139 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/requirements.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2022-09-28 05:25:13.865237 jatsgenerator-0.5.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      895 2022-09-28 05:24:47.000000 jatsgenerator-0.5.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-05-02 02:24:54.731606 jatsgenerator-0.6.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5752 2023-05-02 02:24:54.731606 jatsgenerator-0.6.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5253 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-05-02 02:24:54.731606 jatsgenerator-0.6.0/jatsgenerator/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       22 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/jatsgenerator/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    23597 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/jatsgenerator/build.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1531 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/jatsgenerator/conf.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    17217 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/jatsgenerator/generate.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     3093 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/jatsgenerator/utils.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-05-02 02:24:54.731606 jatsgenerator-0.6.0/jatsgenerator.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5752 2023-05-02 02:24:54.000000 jatsgenerator-0.6.0/jatsgenerator.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      441 2023-05-02 02:24:54.000000 jatsgenerator-0.6.0/jatsgenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-05-02 02:24:54.000000 jatsgenerator-0.6.0/jatsgenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       68 2023-05-02 02:24:54.000000 jatsgenerator-0.6.0/jatsgenerator.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       14 2023-05-02 02:24:54.000000 jatsgenerator-0.6.0/jatsgenerator.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      140 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/requirements.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-05-02 02:24:54.731606 jatsgenerator-0.6.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      895 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-05-02 02:24:54.731606 jatsgenerator-0.6.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    15310 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/tests/test_build.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     2711 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/tests/test_conf.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    15992 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/tests/test_generate.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      907 2023-05-02 02:24:24.000000 jatsgenerator-0.6.0/tests/test_utils.py
```

### Comparing `jatsgenerator-0.5.0/LICENSE` & `jatsgenerator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.5.0/PKG-INFO` & `jatsgenerator-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatsgenerator
-Version: 0.5.0
+Version: 0.6.0
 Summary: JATS XML generator.
 Home-page: https://github.com/elifesciences/jats-generator
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jatsgenerator-0.5.0/README.md` & `jatsgenerator-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.5.0/jatsgenerator/build.py` & `jatsgenerator-0.6.0/jatsgenerator/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from xml.etree.ElementTree import Element, SubElement
 from elifearticle import utils as eautils
 from jatsgenerator import utils
 
 
 def set_journal_title_group(parent, journal_title):
     # journal-title-group
@@ -257,14 +258,63 @@
     history = SubElement(parent, "history")
     for date_type in date_types:
         date = poa_article.get_date(date_type)
         if date:
             set_date(history, poa_article, date_type)
 
 
+def set_publication_history(parent, poa_article):
+    pub_history = SubElement(parent, "pub-history")
+    for event in poa_article.publication_history:
+        event_tag = SubElement(pub_history, "event")
+        if event.event_desc:
+            event_desc_tag = SubElement(event_tag, "event-desc")
+            event_desc_tag.text = event.event_desc
+        if event.date:
+            event_date_tag = SubElement(event_tag, "date")
+            event_date_tag.set("date-type", event.event_type)
+            event_date_tag.set("iso-8601-date", time.strftime("%Y-%m-%d", event.date))
+            set_dmy(event_date_tag, event.date)
+        if event.uri:
+            self_uri_tag = SubElement(event_tag, "self-uri")
+            self_uri_tag.set("content-type", event.event_type)
+            self_uri_tag.set("xlink:href", event.uri)
+
+
+def set_sub_articles(parent, article):
+    for review_article in article.review_articles:
+        set_sub_article(parent, review_article)
+
+
+def set_sub_article(parent, article):
+    sub_article_tag = SubElement(parent, "sub-article")
+    if article.id:
+        sub_article_tag.set("id", article.id)
+    if article.article_type:
+        sub_article_tag.set("article-type", article.article_type)
+    front_stub_tag = SubElement(sub_article_tag, "front-stub")
+    set_article_id(front_stub_tag, article)
+    set_title_group(front_stub_tag, article)
+    if article.contributors:
+        for contributor in article.contributors:
+            contrib_group_tag = SubElement(front_stub_tag, "contrib-group")
+            contrib_tag = SubElement(contrib_group_tag, "contrib")
+            contrib_tag.set("contrib-type", contributor.contrib_type)
+            set_contrib_name(contrib_tag, contributor)
+            set_contrib_orcid(contrib_tag, contributor)
+            # add inline aff tags
+            for affiliation in contributor.affiliations:
+                set_aff(
+                    contrib_tag,
+                    affiliation,
+                    contributor.contrib_type,
+                    institution_wrap=True,
+                )
+
+
 def set_license(parent, poa_article):
     license_tag = SubElement(parent, "license")
 
     license_tag.set("xlink:href", poa_article.license.href)
 
     license_p = SubElement(license_tag, "license-p")
     license_p.text = poa_article.license.paragraph1
@@ -479,37 +529,37 @@
         volume.text = str(poa_article.volume)
 
 
 def set_pub_date(parent, poa_article, pub_type):
     # pub-date pub-type = pub_type
     date = poa_article.get_date(pub_type)
     if date:
-        if pub_type == "pub":
+        if pub_type in ["posted_date", "pub"]:
             date_tag = SubElement(parent, "pub-date")
             date_tag.set("date-type", pub_type)
             date_tag.set("publication-format", "electronic")
-            set_dmy(date_tag, date)
+            set_dmy(date_tag, date.date)
 
 
 def set_date(parent, poa_article, date_type):
     # date date-type = date_type
     date = poa_article.get_date(date_type)
     if date:
         date_tag = SubElement(parent, "date")
         date_tag.set("date-type", date_type)
-        set_dmy(date_tag, date)
+        set_dmy(date_tag, date.date)
 
 
 def set_dmy(parent, date):
     day = SubElement(parent, "day")
-    day.text = str(date.date.tm_mday).zfill(2)
+    day.text = str(date.tm_mday).zfill(2)
     month = SubElement(parent, "month")
-    month.text = str(date.date.tm_mon).zfill(2)
+    month.text = str(date.tm_mon).zfill(2)
     year = SubElement(parent, "year")
-    year.text = str(date.date.tm_year)
+    year.text = str(date.tm_year)
 
 
 def set_author_notes(parent, poa_article):
     author_notes = SubElement(parent, "author-notes")
     corresp_count = 0
     for contributor in poa_article.contributors:
         if contributor.corresp is True:
```

### Comparing `jatsgenerator-0.5.0/jatsgenerator/conf.py` & `jatsgenerator-0.6.0/jatsgenerator/conf.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.5.0/jatsgenerator/generate.py` & `jatsgenerator-0.6.0/jatsgenerator/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,36 +82,45 @@
 
         self.build(self.root, poa_article)
 
     def build(self, root, poa_article):
         self.set_frontmatter(root, poa_article)
         # self.set_title(self.root, poa_article)
         self.set_backmatter(root, poa_article)
+        build.set_sub_articles(root, poa_article)
 
     def set_frontmatter(self, parent, poa_article):
         front = SubElement(parent, "front")
         self.set_journal_meta(front)
         self.set_article_meta(front, poa_article)
         return front
 
     def set_backmatter(self, parent, poa_article):
-        back = SubElement(parent, "back")
-        info_sec = self.set_section(back, "additional-information")
-        info_sec_title = SubElement(info_sec, "title")
-        info_sec_title.text = "Additional information"
-        if poa_article.has_contributor_conflict() or poa_article.conflict_default:
-            build.set_fn_group_competing_interest(info_sec, poa_article)
-        if poa_article.ethics:
-            build.set_fn_group_ethics_information(info_sec, poa_article)
-        if poa_article.datasets or poa_article.data_availability:
-            supp_sec = self.set_section(back, "supplementary-material")
-            supp_sec_title = SubElement(supp_sec, "title")
-            supp_sec_title.text = "Additional Files"
-            data_sec = self.set_section(supp_sec, "data-availability")
-            self.set_article_datasets(data_sec, poa_article)
+        # whether to add a back tag at all
+        if (
+            poa_article.has_contributor_conflict()
+            or poa_article.conflict_default
+            or poa_article.ethics
+            or poa_article.datasets
+            or poa_article.data_availability
+        ):
+            back = SubElement(parent, "back")
+            info_sec = self.set_section(back, "additional-information")
+            info_sec_title = SubElement(info_sec, "title")
+            info_sec_title.text = "Additional information"
+            if poa_article.has_contributor_conflict() or poa_article.conflict_default:
+                build.set_fn_group_competing_interest(info_sec, poa_article)
+            if poa_article.ethics:
+                build.set_fn_group_ethics_information(info_sec, poa_article)
+            if poa_article.datasets or poa_article.data_availability:
+                supp_sec = self.set_section(back, "supplementary-material")
+                supp_sec_title = SubElement(supp_sec, "title")
+                supp_sec_title.text = "Additional Files"
+                data_sec = self.set_section(supp_sec, "data-availability")
+                self.set_article_datasets(data_sec, poa_article)
 
     def set_section(self, parent, sec_type):
         self.context.sec_count += 1
         sec = SubElement(parent, "sec")
         sec.set("id", "s" + str(self.context.sec_count))
         sec.set("sec-type", sec_type)
         return sec
@@ -129,44 +138,65 @@
         # article-id pub-id-type="doi"
         if poa_article.doi:
             pub_id_type = "doi"
             article_id = SubElement(article_meta, "article-id")
             article_id.text = poa_article.doi
             article_id.set("pub-id-type", pub_id_type)
 
+        # article-id pub-id-type="doi" specific-use="version"
+        if hasattr(poa_article, "version_doi") and poa_article.version_doi:
+            pub_id_type = "doi"
+            article_id = SubElement(article_meta, "article-id")
+            article_id.text = poa_article.version_doi
+            article_id.set("pub-id-type", pub_id_type)
+            article_id.set("specific-use", "version")
+
         # article-categories
         build.set_article_categories(article_meta, poa_article)
 
-        build.set_title_group(article_meta, poa_article)
+        if poa_article.title:
+            build.set_title_group(article_meta, poa_article)
 
-        for contrib_type in self.jats_config.get("contrib_types"):
-            self.set_contrib_group(article_meta, poa_article, contrib_type)
+        if poa_article.contributors:
+            for contrib_type in self.jats_config.get("contrib_types"):
+                self.set_contrib_group(article_meta, poa_article, contrib_type)
 
         if bool(
             [contrib for contrib in poa_article.contributors if contrib.corresp is True]
         ):
             build.set_author_notes(article_meta, poa_article)
 
         build.set_pub_date(article_meta, poa_article, "pub")
 
+        build.set_pub_date(article_meta, poa_article, "posted_date")
+
         build.set_volume(article_meta, poa_article)
 
         if poa_article.manuscript:
             elocation_id = SubElement(article_meta, "elocation-id")
-            elocation_id.text = "e" + str(int(poa_article.manuscript)).zfill(5)
+            if "elocation_id_pattern" in self.jats_config:
+                elocation_id.text = self.jats_config.get("elocation_id_pattern").format(
+                    manuscript=poa_article.manuscript
+                )
+            else:
+                elocation_id.text = "e" + str(int(poa_article.manuscript)).zfill(5)
 
         if poa_article.dates:
             build.set_history(
                 article_meta, poa_article, self.jats_config.get("history_date_types")
             )
 
+        if poa_article.publication_history:
+            build.set_publication_history(article_meta, poa_article)
+
         if poa_article.license:
             build.set_permissions(article_meta, poa_article)
 
-        build.set_abstract(article_meta, poa_article)
+        if poa_article.abstract:
+            build.set_abstract(article_meta, poa_article)
 
         # Disabled author keywords from inclusion Oct 2, 2015
         # if poa_article.author_keywords:
         #     build.set_kwd_group_author_keywords(article_meta, poa_article)
 
         if poa_article.research_organisms:
             build.set_kwd_group_research_organism(article_meta, poa_article)
```

### Comparing `jatsgenerator-0.5.0/jatsgenerator/utils.py` & `jatsgenerator-0.6.0/jatsgenerator/utils.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.5.0/jatsgenerator.egg-info/PKG-INFO` & `jatsgenerator-0.6.0/jatsgenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatsgenerator
-Version: 0.5.0
+Version: 0.6.0
 Summary: JATS XML generator.
 Home-page: https://github.com/elifesciences/jats-generator
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jatsgenerator-0.5.0/setup.py` & `jatsgenerator-0.6.0/setup.py`

 * *Files identical despite different names*

