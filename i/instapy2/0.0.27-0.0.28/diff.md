# Comparing `tmp/instapy2-0.0.27.tar.gz` & `tmp/instapy2-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instapy2-0.0.27.tar", last modified: Sun Dec 11 07:05:14 2022, max compression
+gzip compressed data, was "instapy2-0.0.28.tar", last modified: Tue May  2 18:52:26 2023, max compression
```

## Comparing `instapy2-0.0.27.tar` & `instapy2-0.0.28.tar`

### file list

```diff
@@ -1,38 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-12-11 07:05:14.496606 instapy2-0.0.27/
--rw-rw-rw-   0        0        0    35823 2022-11-08 15:30:57.000000 instapy2-0.0.27/LICENSE.md
--rw-rw-rw-   0        0        0     3237 2022-12-11 07:05:14.495546 instapy2-0.0.27/PKG-INFO
--rw-rw-rw-   0        0        0     2303 2022-11-25 08:28:47.000000 instapy2-0.0.27/README.md
--rw-rw-rw-   0        0        0       42 2022-12-11 07:05:14.496606 instapy2-0.0.27/setup.cfg
--rw-rw-rw-   0        0        0     1497 2022-11-15 05:55:36.000000 instapy2-0.0.27/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-11 07:05:14.468910 instapy2-0.0.27/src/
-drwxrwxrwx   0        0        0        0 2022-12-11 07:05:14.474403 instapy2-0.0.27/src/instapy2/
--rw-rw-rw-   0        0        0       30 2022-11-08 15:30:57.000000 instapy2-0.0.27/src/instapy2/__init__.py
--rw-rw-rw-   0        0        0      946 2022-12-11 06:18:44.000000 instapy2-0.0.27/src/instapy2/configuration.py
-drwxrwxrwx   0        0        0        0 2022-12-11 07:05:14.487053 instapy2-0.0.27/src/instapy2/helpers/
--rw-rw-rw-   0        0        0       70 2022-11-10 06:52:56.000000 instapy2-0.0.27/src/instapy2/helpers/__init__.py
--rw-rw-rw-   0        0        0     1184 2022-11-08 15:30:57.000000 instapy2-0.0.27/src/instapy2/helpers/location.py
--rw-rw-rw-   0        0        0     1129 2022-11-08 15:30:57.000000 instapy2-0.0.27/src/instapy2/helpers/people.py
--rw-rw-rw-   0        0        0    21751 2022-12-11 06:28:46.000000 instapy2-0.0.27/src/instapy2/instapy2.py
--rw-rw-rw-   0        0        0     1943 2022-12-11 06:17:44.000000 instapy2-0.0.27/src/instapy2/instapy2_base.py
-drwxrwxrwx   0        0        0        0 2022-12-11 07:05:14.490557 instapy2-0.0.27/src/instapy2/types/
--rw-rw-rw-   0        0        0      181 2022-11-14 04:24:25.000000 instapy2-0.0.27/src/instapy2/types/__init__.py
--rw-rw-rw-   0        0        0       68 2022-11-08 15:30:57.000000 instapy2-0.0.27/src/instapy2/types/comment_type.py
--rw-rw-rw-   0        0        0      132 2022-11-14 03:53:07.000000 instapy2-0.0.27/src/instapy2/types/follow_type.py
--rw-rw-rw-   0        0        0      108 2022-11-08 15:30:57.000000 instapy2-0.0.27/src/instapy2/types/like_type.py
--rw-rw-rw-   0        0        0       94 2022-11-14 04:23:48.000000 instapy2-0.0.27/src/instapy2/types/post_type.py
--rw-rw-rw-   0        0        0       65 2022-11-14 03:53:14.000000 instapy2-0.0.27/src/instapy2/types/unfollow_type.py
-drwxrwxrwx   0        0        0        0 2022-12-11 07:05:14.495546 instapy2-0.0.27/src/instapy2/utilities/
--rw-rw-rw-   0        0        0      225 2022-11-25 07:34:50.000000 instapy2-0.0.27/src/instapy2/utilities/__init__.py
--rw-rw-rw-   0        0        0     1840 2022-11-10 06:52:56.000000 instapy2-0.0.27/src/instapy2/utilities/comments.py
--rw-rw-rw-   0        0        0     1220 2022-11-14 04:19:51.000000 instapy2-0.0.27/src/instapy2/utilities/follows.py
--rw-rw-rw-   0        0        0      630 2022-11-10 06:52:56.000000 instapy2-0.0.27/src/instapy2/utilities/interactions.py
--rw-rw-rw-   0        0        0      816 2022-11-10 06:52:56.000000 instapy2-0.0.27/src/instapy2/utilities/likes.py
--rw-rw-rw-   0        0        0     3828 2022-11-15 05:54:08.000000 instapy2-0.0.27/src/instapy2/utilities/media.py
--rw-rw-rw-   0        0        0     2009 2022-11-25 08:10:29.000000 instapy2-0.0.27/src/instapy2/utilities/messages.py
--rw-rw-rw-   0        0        0      125 2022-11-08 15:41:53.000000 instapy2-0.0.27/src/instapy2/utilities/utility_base.py
-drwxrwxrwx   0        0        0        0 2022-12-11 07:05:14.486004 instapy2-0.0.27/src/instapy2.egg-info/
--rw-rw-rw-   0        0        0     3237 2022-12-11 07:05:14.000000 instapy2-0.0.27/src/instapy2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2022-12-11 07:05:14.000000 instapy2-0.0.27/src/instapy2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-11 07:05:14.000000 instapy2-0.0.27/src/instapy2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-12-11 07:05:14.000000 instapy2-0.0.27/src/instapy2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-11 07:05:14.000000 instapy2-0.0.27/src/instapy2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 18:52:26.331956 instapy2-0.0.28/
+-rw-rw-rw-   0        0        0    35823 2022-11-08 15:30:57.000000 instapy2-0.0.28/LICENSE.md
+-rw-rw-rw-   0        0        0     3226 2023-05-02 18:52:26.331956 instapy2-0.0.28/PKG-INFO
+-rw-rw-rw-   0        0        0     2276 2023-03-31 07:54:51.000000 instapy2-0.0.28/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 18:52:26.332959 instapy2-0.0.28/setup.cfg
+-rw-rw-rw-   0        0        0     1569 2023-05-02 18:51:57.000000 instapy2-0.0.28/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:52:25.916832 instapy2-0.0.28/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 18:52:25.919833 instapy2-0.0.28/src/instapy2/
+-rw-rw-rw-   0        0        0       30 2022-12-30 23:48:03.000000 instapy2-0.0.28/src/instapy2/__init__.py
+-rw-rw-rw-   0        0        0    11562 2023-04-11 09:08:04.000000 instapy2-0.0.28/src/instapy2/instapy2.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:52:25.932861 instapy2-0.0.28/src/instapy2/types/
+-rw-rw-rw-   0        0        0      100 2023-03-31 07:47:23.000000 instapy2-0.0.28/src/instapy2/types/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-01-14 05:27:35.000000 instapy2-0.0.28/src/instapy2/types/commenttype.py
+-rw-rw-rw-   0        0        0       95 2023-01-13 08:28:57.000000 instapy2-0.0.28/src/instapy2/types/liketype.py
+-rw-rw-rw-   0        0        0       97 2023-04-03 09:26:28.000000 instapy2-0.0.28/src/instapy2/types/posttype.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:52:26.331452 instapy2-0.0.28/src/instapy2/utilities/
+-rw-rw-rw-   0        0        0       73 2023-01-14 05:04:04.000000 instapy2-0.0.28/src/instapy2/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-01-14 05:38:12.000000 instapy2-0.0.28/src/instapy2/utilities/authentication.py
+-rw-rw-rw-   0        0        0      271 2023-01-14 05:49:41.000000 instapy2-0.0.28/src/instapy2/utilities/comments.py
+-rw-rw-rw-   0        0        0     2814 2023-01-13 08:53:12.000000 instapy2-0.0.28/src/instapy2/utilities/limitations.py
+-rw-rw-rw-   0        0        0     1484 2023-01-14 06:02:47.000000 instapy2-0.0.28/src/instapy2/utilities/logger.py
+-rw-rw-rw-   0        0        0     3619 2023-03-31 07:50:41.000000 instapy2-0.0.28/src/instapy2/utilities/medias.py
+-rw-rw-rw-   0        0        0     1957 2023-05-02 18:16:41.000000 instapy2-0.0.28/src/instapy2/utilities/persistence.py
+-rw-rw-rw-   0        0        0     2431 2023-01-16 05:44:34.000000 instapy2-0.0.28/src/instapy2/utilities/utility.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:52:25.931409 instapy2-0.0.28/src/instapy2.egg-info/
+-rw-rw-rw-   0        0        0     3226 2023-05-02 18:52:25.000000 instapy2-0.0.28/src/instapy2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-05-02 18:52:25.000000 instapy2-0.0.28/src/instapy2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:52:25.000000 instapy2-0.0.28/src/instapy2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-02 18:52:25.000000 instapy2-0.0.28/src/instapy2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 18:52:25.000000 instapy2-0.0.28/src/instapy2.egg-info/top_level.txt
```

### Comparing `instapy2-0.0.27/LICENSE.md` & `instapy2-0.0.28/LICENSE.md`

 * *Files identical despite different names*

### Comparing `instapy2-0.0.27/PKG-INFO` & `instapy2-0.0.28/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: instapy2
-Version: 0.0.27
+Version: 0.0.28
 Summary: Automation script for Instagram that farms comments, follows and likes.
 Home-page: https://github.com/InstaPy2/InstaPy2
 Author: Antique
 Author-email: official.antique@gmail.com
-Keywords: automation,bot,insta,instagram,instagrapi,instapy,instapy2
+Keywords: automation,bot,ig,insta,instagram,instagrapi,instapy,instapy2,python,python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -23,15 +23,15 @@
 
 <img src="https://raw.githubusercontent.com/InstaPy2/InstaPy2/main/instapy2.png" width="44px"></img>
 # InstaPy2
 Automation script for Instagram that *farms* comments, follows and likes.
 
 <span>
     <img src="https://img.shields.io/static/v1?label=Built%20with&message=Instagrapi&color=red"/>
-    <img src="https://img.shields.io/static/v1?label=Built%20with&message=Python%203.11.0rc2&color=red"/>
+    <img src="https://img.shields.io/static/v1?label=Built%20with&message=Python%203.11.2&color=red"/>
     <a href="https://discord.gg/TY8pt8e5Xg" style="text-decoration: none; border: none; outline: 0;">
         <img src="https://img.shields.io/static/v1?label=Connect%20via&message=Discord&color=5865F2"/>
     </a>
     <img src="https://img.shields.io/static/v1?label=License&message=GPLv3&color=blue"/>
 </span>
 <br/>
 <span>
@@ -39,29 +39,28 @@
         <img src="https://img.shields.io/static/v1?label=Support&message=Buy%20Me%20A%20Coffee&color=yellow"/>
     </a>
     <a href="https://paypal.com/paypalme/officialantique" style="text-decoration: none; border: none; outline: 0;">
         <img src="https://img.shields.io/static/v1?label=Support&message=PayPal&color=009cde"/>
     </a>
 </span>
 
-<br/>
-
-## [Documentation](https://github.com/InstaPy2/InstaPy2/tree/main/documentation)
+## [Documentation](https://official-antique.gitbook.io/instapy2/documentation)
 Find all of the documentation in the link above.
 
-## [Examples](https://github.com/InstaPy2/InstaPy2/tree/main/examples)
+## [Examples](https://official-antique.gitbook.io/instapy2/examples)
 Find a variety of examples in the link above.
 
 ## Latest Changes
-> 25th November 2022
+### Rework Branch
+> 31st March 2023
 
-- Added ability to direct message users.
-    - See [CHANGELOG.md](CHANGELOG.md) for more information.
+- See [CHANGELOG.md](CHANGELOG.md) for more information.
 
 ## Previous Changes
+### Main Branch
 > 25th November 2022
 
 No changes have been made.
 
 ## Social Media
 <span>
   <img src="https://img.shields.io/static/v1?label=Discord&message=Antique%239837&color=blueviolet"/>
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: instapy2 Version: 0.0.27 Summary: Automation script
+Metadata-Version: 2.1 Name: instapy2 Version: 0.0.28 Summary: Automation script
 for Instagram that farms comments, follows and likes. Home-page: https://
 github.com/InstaPy2/InstaPy2 Author: Antique Author-email:
 official.antique@gmail.com Keywords:
-automation,bot,insta,instagram,instagrapi,instapy,instapy2 Classifier:
-Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: End Users/
-Desktop Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Natural Language :: English Classifier: Operating System ::
-MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: POSIX Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development Classifier: Topic :: Utilities
+automation,bot,ig,insta,instagram,instagrapi,instapy,instapy2,python,python3
+Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+End Users/Desktop Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
+Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX Classifier: Programming Language ::
+Python Classifier: Topic :: Software Development Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE.md [https://
 raw.githubusercontent.com/InstaPy2/InstaPy2/main/instapy2.png] # InstaPy2
 Automation script for Instagram that *farms* comments, follows and likes.
 [https://img.shields.io/static/
 v1?label=Built%20with&message=Instagrapi&color=red] [https://img.shields.io/
-static/v1?label=Built%20with&message=Python%203.11.0rc2&color=red] [https://
+static/v1?label=Built%20with&message=Python%203.11.2&color=red] [https://
 img.shields.io/static/v1?label=Connect%20via&message=Discord&color=5865F2]
 [https://img.shields.io/static/v1?label=License&message=GPLv3&color=blue]
  [https://img.shields.io/static/
 v1?label=Support&message=Buy%20Me%20A%20Coffee&color=yellow] [https://
-img.shields.io/static/v1?label=Support&message=PayPal&color=009cde]
-## [Documentation](https://github.com/InstaPy2/InstaPy2/tree/main/
-documentation) Find all of the documentation in the link above. ## [Examples]
-(https://github.com/InstaPy2/InstaPy2/tree/main/examples) Find a variety of
-examples in the link above. ## Latest Changes > 25th November 2022 - Added
-ability to direct message users. - See [CHANGELOG.md](CHANGELOG.md) for more
-information. ## Previous Changes > 25th November 2022 No changes have been
-made. ## Social Media  [https://img.shields.io/static/
+img.shields.io/static/v1?label=Support&message=PayPal&color=009cde]  ##
+[Documentation](https://official-antique.gitbook.io/instapy2/documentation)
+Find all of the documentation in the link above. ## [Examples](https://
+official-antique.gitbook.io/instapy2/examples) Find a variety of examples in
+the link above. ## Latest Changes ### Rework Branch > 31st March 2023 - See
+[CHANGELOG.md](CHANGELOG.md) for more information. ## Previous Changes ### Main
+Branch > 25th November 2022 No changes have been made. ## Social Media  [https:
+//img.shields.io/static/
 v1?label=Discord&message=Antique%239837&color=blueviolet] [https://
 img.shields.io/static/v1?label=Reddit&message=%40antique_codes&color=red]
 [https://img.shields.io/static/
 v1?label=Twitch&message=official_antique&color=blueviolet] [https://
 img.shields.io/static/v1?label=Twitter&message=%40antique_codes&color=blue]
```

### Comparing `instapy2-0.0.27/README.md` & `instapy2-0.0.28/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="https://raw.githubusercontent.com/InstaPy2/InstaPy2/main/instapy2.png" width="44px"></img>
 # InstaPy2
 Automation script for Instagram that *farms* comments, follows and likes.
 
 <span>
     <img src="https://img.shields.io/static/v1?label=Built%20with&message=Instagrapi&color=red"/>
-    <img src="https://img.shields.io/static/v1?label=Built%20with&message=Python%203.11.0rc2&color=red"/>
+    <img src="https://img.shields.io/static/v1?label=Built%20with&message=Python%203.11.2&color=red"/>
     <a href="https://discord.gg/TY8pt8e5Xg" style="text-decoration: none; border: none; outline: 0;">
         <img src="https://img.shields.io/static/v1?label=Connect%20via&message=Discord&color=5865F2"/>
     </a>
     <img src="https://img.shields.io/static/v1?label=License&message=GPLv3&color=blue"/>
 </span>
 <br/>
 <span>
@@ -16,29 +16,28 @@
         <img src="https://img.shields.io/static/v1?label=Support&message=Buy%20Me%20A%20Coffee&color=yellow"/>
     </a>
     <a href="https://paypal.com/paypalme/officialantique" style="text-decoration: none; border: none; outline: 0;">
         <img src="https://img.shields.io/static/v1?label=Support&message=PayPal&color=009cde"/>
     </a>
 </span>
 
-<br/>
-
-## [Documentation](https://github.com/InstaPy2/InstaPy2/tree/main/documentation)
+## [Documentation](https://official-antique.gitbook.io/instapy2/documentation)
 Find all of the documentation in the link above.
 
-## [Examples](https://github.com/InstaPy2/InstaPy2/tree/main/examples)
+## [Examples](https://official-antique.gitbook.io/instapy2/examples)
 Find a variety of examples in the link above.
 
 ## Latest Changes
-> 25th November 2022
+### Rework Branch
+> 31st March 2023
 
-- Added ability to direct message users.
-    - See [CHANGELOG.md](CHANGELOG.md) for more information.
+- See [CHANGELOG.md](CHANGELOG.md) for more information.
 
 ## Previous Changes
+### Main Branch
 > 25th November 2022
 
 No changes have been made.
 
 ## Social Media
 <span>
   <img src="https://img.shields.io/static/v1?label=Discord&message=Antique%239837&color=blueviolet"/>
@@ -47,8 +46,8 @@
   </a>
   <a href="https://twitch.tv/official_antique">
     <img src="https://img.shields.io/static/v1?label=Twitch&message=official_antique&color=blueviolet"/>
   </a>
   <a href="https://twitter.com/antique_codes">
     <img src="https://img.shields.io/static/v1?label=Twitter&message=%40antique_codes&color=blue"/>
   </a>
-</span>
+</span>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 [https://raw.githubusercontent.com/InstaPy2/InstaPy2/main/instapy2.png] #
 InstaPy2 Automation script for Instagram that *farms* comments, follows and
 likes.  [https://img.shields.io/static/
 v1?label=Built%20with&message=Instagrapi&color=red] [https://img.shields.io/
-static/v1?label=Built%20with&message=Python%203.11.0rc2&color=red] [https://
+static/v1?label=Built%20with&message=Python%203.11.2&color=red] [https://
 img.shields.io/static/v1?label=Connect%20via&message=Discord&color=5865F2]
 [https://img.shields.io/static/v1?label=License&message=GPLv3&color=blue]
  [https://img.shields.io/static/
 v1?label=Support&message=Buy%20Me%20A%20Coffee&color=yellow] [https://
-img.shields.io/static/v1?label=Support&message=PayPal&color=009cde]
-## [Documentation](https://github.com/InstaPy2/InstaPy2/tree/main/
-documentation) Find all of the documentation in the link above. ## [Examples]
-(https://github.com/InstaPy2/InstaPy2/tree/main/examples) Find a variety of
-examples in the link above. ## Latest Changes > 25th November 2022 - Added
-ability to direct message users. - See [CHANGELOG.md](CHANGELOG.md) for more
-information. ## Previous Changes > 25th November 2022 No changes have been
-made. ## Social Media  [https://img.shields.io/static/
+img.shields.io/static/v1?label=Support&message=PayPal&color=009cde]  ##
+[Documentation](https://official-antique.gitbook.io/instapy2/documentation)
+Find all of the documentation in the link above. ## [Examples](https://
+official-antique.gitbook.io/instapy2/examples) Find a variety of examples in
+the link above. ## Latest Changes ### Rework Branch > 31st March 2023 - See
+[CHANGELOG.md](CHANGELOG.md) for more information. ## Previous Changes ### Main
+Branch > 25th November 2022 No changes have been made. ## Social Media  [https:
+//img.shields.io/static/
 v1?label=Discord&message=Antique%239837&color=blueviolet] [https://
 img.shields.io/static/v1?label=Reddit&message=%40antique_codes&color=red]
 [https://img.shields.io/static/
 v1?label=Twitch&message=official_antique&color=blueviolet] [https://
 img.shields.io/static/v1?label=Twitter&message=%40antique_codes&color=blue]
```

### Comparing `instapy2-0.0.27/setup.py` & `instapy2-0.0.28/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,31 +22,35 @@
         'Operating System :: POSIX',
         'Programming Language :: Python',
         'Topic :: Software Development',
         'Topic :: Utilities'
     ],
     description='Automation script for Instagram that farms comments, follows and likes.',
     install_requires=[
+        'emoji',
         'instagrapi',
         'Pillow',
         'python-dotenv'
     ],
     keywords=[
         'automation',
         'bot',
+        'ig',
         'insta',
         'instagram',
         'instagrapi',
         'instapy',
-        'instapy2'
+        'instapy2',
+        'python',
+        'python3'
     ],
     license_file='LICENSE.md',
     long_description=read(file='README.md'),
     long_description_content_type='text/markdown',
     name='instapy2',
     package_dir={
         '' : 'src'
     },
     packages=find_packages(where='src'),
     url=homepage,
-    version='0.0.27'
+    version='0.0.28'
 )
```

### Comparing `instapy2-0.0.27/src/instapy2/instapy2_base.py` & `instapy2-0.0.28/src/instapy2/utilities/authentication.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,60 @@
-from .configuration import Configuration
+from .comments import Comments
+from .limitations import Limitations
+from .logger import Logger
+from .medias import Medias
+from .persistence import Persistence
+
+from os import getcwd, mkdir, sep
+from os.path import exists
+from pathlib import Path
 
 from instagrapi import Client
 
-from os import getcwd, mkdir, path
-from typing import Dict, List, Union
-import urllib3
-
-class InstaPy2Base:
-    def login(self, username: str = None, password: str = None, verification_code: str = ''):
-        def proxy() -> Union[None, str]:
-            for proxy in self.proxies:
-                try:
-                    url = proxy['url'] or ''
-                    username = proxy['username'] or ''
-                    password = proxy['password'] or ''
-
-                    pool = urllib3.ProxyManager(proxy_url=url, headers=urllib3.make_headers(proxy_basic_auth=f'{username}:{password}'))
-                    pool.request('GET', 'https://google.com')
-                    return proxy
-                except:
-                    return None
+class Authentication:
+    def __create_persistence(self):
+        self.persistence.create_tables()
+
+    def __files_exists(self, path: str) -> bool:
+        return exists(path=path)
+    
+    def __make_files(self, path: str) -> bool:
+        return mkdir(path=path) is not None
+
+    def __settings_exists(self, path: str) -> bool:
+        return exists(path=path)
+    
+
+    def __init__(self):
+        self.logger = Logger()
+        
+
+    def login(self, username: str, password: str, verification_code: str = '', proxy: str = ''):
+        files_path = getcwd() + sep + 'files'
+        if not self.__files_exists(path=files_path):
+            _ = self.__make_files(path=files_path)
+
+        self.session = Client(proxy=proxy)
+        settings_path = files_path + sep + username + '.json'
+        try:
+            if not self.__settings_exists(path=settings_path):
+                logged_in = self.session.login(username=username, password=password, verification_code=verification_code)
+                self.session.dump_settings(path=Path(settings_path))
+            else:
+                self.session.load_settings(path=Path(settings_path))
+                logged_in = self.session.login(username=username, password=password, verification_code=verification_code)
+        except:
+            self.logger.error(message='There was an error while logging in.')
+            exit(0)
 
-        if hasattr(self, 'proxies'):
-            self.session = Client(proxy=proxy())
+        if not logged_in:
+            self.logger.error(message='Failed to log in successfully.')
         else:
-            self.session = Client()
+            self.logger.info(message=f'Successfully logged in as: {self.session.username}.')
 
-        if not path.exists(path=getcwd() + f'{path.sep}/files'):
-            mkdir(path=getcwd() + f'{path.sep}/files')
+        # MARK: Placing them here to lessen the amount of code needed to configure shit.
+        self.comments = Comments()
+        self.limitations = Limitations(session=self.session)
+        self.medias = Medias(session=self.session)
+        self.persistence = Persistence()
 
-        if path.exists(path=getcwd() + f'{path.sep}files{path.sep}{username}.json'):
-            self.session.load_settings(path=getcwd() + f'{path.sep}files{path.sep}{username}.json')
-            logged_in = self.session.login(username=username, password=password, verification_code=verification_code)
-        else:
-            logged_in = self.session.login(username=username, password=password, verification_code=verification_code)
-            self.session.dump_settings(path=getcwd() + f'{path.sep}files{path.sep}{username}.json')
-
-        print(f'[INFO]: Successfully logged in as: {self.session.username}.' if logged_in else f'[ERROR]: Failed to log in.')
-        self.configuration = Configuration(session=self.session)
-
-    def set_proxies(self, proxies: List[Dict[str, str]] = None):
-        self.proxies = proxies
+        self.__create_persistence()
```

### Comparing `instapy2-0.0.27/src/instapy2.egg-info/PKG-INFO` & `instapy2-0.0.28/src/instapy2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: instapy2
-Version: 0.0.27
+Version: 0.0.28
 Summary: Automation script for Instagram that farms comments, follows and likes.
 Home-page: https://github.com/InstaPy2/InstaPy2
 Author: Antique
 Author-email: official.antique@gmail.com
-Keywords: automation,bot,insta,instagram,instagrapi,instapy,instapy2
+Keywords: automation,bot,ig,insta,instagram,instagrapi,instapy,instapy2,python,python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -23,15 +23,15 @@
 
 <img src="https://raw.githubusercontent.com/InstaPy2/InstaPy2/main/instapy2.png" width="44px"></img>
 # InstaPy2
 Automation script for Instagram that *farms* comments, follows and likes.
 
 <span>
     <img src="https://img.shields.io/static/v1?label=Built%20with&message=Instagrapi&color=red"/>
-    <img src="https://img.shields.io/static/v1?label=Built%20with&message=Python%203.11.0rc2&color=red"/>
+    <img src="https://img.shields.io/static/v1?label=Built%20with&message=Python%203.11.2&color=red"/>
     <a href="https://discord.gg/TY8pt8e5Xg" style="text-decoration: none; border: none; outline: 0;">
         <img src="https://img.shields.io/static/v1?label=Connect%20via&message=Discord&color=5865F2"/>
     </a>
     <img src="https://img.shields.io/static/v1?label=License&message=GPLv3&color=blue"/>
 </span>
 <br/>
 <span>
@@ -39,29 +39,28 @@
         <img src="https://img.shields.io/static/v1?label=Support&message=Buy%20Me%20A%20Coffee&color=yellow"/>
     </a>
     <a href="https://paypal.com/paypalme/officialantique" style="text-decoration: none; border: none; outline: 0;">
         <img src="https://img.shields.io/static/v1?label=Support&message=PayPal&color=009cde"/>
     </a>
 </span>
 
-<br/>
-
-## [Documentation](https://github.com/InstaPy2/InstaPy2/tree/main/documentation)
+## [Documentation](https://official-antique.gitbook.io/instapy2/documentation)
 Find all of the documentation in the link above.
 
-## [Examples](https://github.com/InstaPy2/InstaPy2/tree/main/examples)
+## [Examples](https://official-antique.gitbook.io/instapy2/examples)
 Find a variety of examples in the link above.
 
 ## Latest Changes
-> 25th November 2022
+### Rework Branch
+> 31st March 2023
 
-- Added ability to direct message users.
-    - See [CHANGELOG.md](CHANGELOG.md) for more information.
+- See [CHANGELOG.md](CHANGELOG.md) for more information.
 
 ## Previous Changes
+### Main Branch
 > 25th November 2022
 
 No changes have been made.
 
 ## Social Media
 <span>
   <img src="https://img.shields.io/static/v1?label=Discord&message=Antique%239837&color=blueviolet"/>
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: instapy2 Version: 0.0.27 Summary: Automation script
+Metadata-Version: 2.1 Name: instapy2 Version: 0.0.28 Summary: Automation script
 for Instagram that farms comments, follows and likes. Home-page: https://
 github.com/InstaPy2/InstaPy2 Author: Antique Author-email:
 official.antique@gmail.com Keywords:
-automation,bot,insta,instagram,instagrapi,instapy,instapy2 Classifier:
-Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: End Users/
-Desktop Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Natural Language :: English Classifier: Operating System ::
-MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: POSIX Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development Classifier: Topic :: Utilities
+automation,bot,ig,insta,instagram,instagrapi,instapy,instapy2,python,python3
+Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+End Users/Desktop Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
+Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX Classifier: Programming Language ::
+Python Classifier: Topic :: Software Development Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE.md [https://
 raw.githubusercontent.com/InstaPy2/InstaPy2/main/instapy2.png] # InstaPy2
 Automation script for Instagram that *farms* comments, follows and likes.
 [https://img.shields.io/static/
 v1?label=Built%20with&message=Instagrapi&color=red] [https://img.shields.io/
-static/v1?label=Built%20with&message=Python%203.11.0rc2&color=red] [https://
+static/v1?label=Built%20with&message=Python%203.11.2&color=red] [https://
 img.shields.io/static/v1?label=Connect%20via&message=Discord&color=5865F2]
 [https://img.shields.io/static/v1?label=License&message=GPLv3&color=blue]
  [https://img.shields.io/static/
 v1?label=Support&message=Buy%20Me%20A%20Coffee&color=yellow] [https://
-img.shields.io/static/v1?label=Support&message=PayPal&color=009cde]
-## [Documentation](https://github.com/InstaPy2/InstaPy2/tree/main/
-documentation) Find all of the documentation in the link above. ## [Examples]
-(https://github.com/InstaPy2/InstaPy2/tree/main/examples) Find a variety of
-examples in the link above. ## Latest Changes > 25th November 2022 - Added
-ability to direct message users. - See [CHANGELOG.md](CHANGELOG.md) for more
-information. ## Previous Changes > 25th November 2022 No changes have been
-made. ## Social Media  [https://img.shields.io/static/
+img.shields.io/static/v1?label=Support&message=PayPal&color=009cde]  ##
+[Documentation](https://official-antique.gitbook.io/instapy2/documentation)
+Find all of the documentation in the link above. ## [Examples](https://
+official-antique.gitbook.io/instapy2/examples) Find a variety of examples in
+the link above. ## Latest Changes ### Rework Branch > 31st March 2023 - See
+[CHANGELOG.md](CHANGELOG.md) for more information. ## Previous Changes ### Main
+Branch > 25th November 2022 No changes have been made. ## Social Media  [https:
+//img.shields.io/static/
 v1?label=Discord&message=Antique%239837&color=blueviolet] [https://
 img.shields.io/static/v1?label=Reddit&message=%40antique_codes&color=red]
 [https://img.shields.io/static/
 v1?label=Twitch&message=official_antique&color=blueviolet] [https://
 img.shields.io/static/v1?label=Twitter&message=%40antique_codes&color=blue]
```

### Comparing `instapy2-0.0.27/src/instapy2.egg-info/SOURCES.txt` & `instapy2-0.0.28/src/instapy2.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 LICENSE.md
 README.md
 setup.py
 src/instapy2/__init__.py
-src/instapy2/configuration.py
 src/instapy2/instapy2.py
-src/instapy2/instapy2_base.py
 src/instapy2.egg-info/PKG-INFO
 src/instapy2.egg-info/SOURCES.txt
 src/instapy2.egg-info/dependency_links.txt
 src/instapy2.egg-info/requires.txt
 src/instapy2.egg-info/top_level.txt
-src/instapy2/helpers/__init__.py
-src/instapy2/helpers/location.py
-src/instapy2/helpers/people.py
 src/instapy2/types/__init__.py
-src/instapy2/types/comment_type.py
-src/instapy2/types/follow_type.py
-src/instapy2/types/like_type.py
-src/instapy2/types/post_type.py
-src/instapy2/types/unfollow_type.py
+src/instapy2/types/commenttype.py
+src/instapy2/types/liketype.py
+src/instapy2/types/posttype.py
 src/instapy2/utilities/__init__.py
+src/instapy2/utilities/authentication.py
 src/instapy2/utilities/comments.py
-src/instapy2/utilities/follows.py
-src/instapy2/utilities/interactions.py
-src/instapy2/utilities/likes.py
-src/instapy2/utilities/media.py
-src/instapy2/utilities/messages.py
-src/instapy2/utilities/utility_base.py
+src/instapy2/utilities/limitations.py
+src/instapy2/utilities/logger.py
+src/instapy2/utilities/medias.py
+src/instapy2/utilities/persistence.py
+src/instapy2/utilities/utility.py
```

