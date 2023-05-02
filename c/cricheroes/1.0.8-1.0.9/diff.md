# Comparing `tmp/cricheroes-1.0.8-py2.py3-none-any.whl.zip` & `tmp/cricheroes-1.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6712 bytes, number of entries: 7
+Zip file size: 6747 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       25 b- defN 22-Dec-12 08:08 cricheroes/__init__.py
--rw-rw-rw-  2.0 fat    15239 b- defN 23-Jan-21 07:16 cricheroes/cricheroes.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jan-21 07:19 cricheroes-1.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2762 b- defN 23-Jan-21 07:19 cricheroes-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jan-21 07:19 cricheroes-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jan-21 07:19 cricheroes-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      561 b- defN 23-Jan-21 07:19 cricheroes-1.0.8.dist-info/RECORD
-7 files, 19802 bytes uncompressed, 5718 bytes compressed:  71.1%
+-rw-rw-rw-  2.0 fat    15355 b- defN 23-May-02 08:22 cricheroes/cricheroes.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-May-02 08:25 cricheroes-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2762 b- defN 23-May-02 08:25 cricheroes-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-02 08:25 cricheroes-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-02 08:25 cricheroes-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      561 b- defN 23-May-02 08:25 cricheroes-1.0.9.dist-info/RECORD
+7 files, 19918 bytes uncompressed, 5753 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: cricheroes/__init__.py
 Comment: 
 
 Filename: cricheroes/cricheroes.py
 Comment: 
 
-Filename: cricheroes-1.0.8.dist-info/LICENSE
+Filename: cricheroes-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: cricheroes-1.0.8.dist-info/METADATA
+Filename: cricheroes-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: cricheroes-1.0.8.dist-info/WHEEL
+Filename: cricheroes-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: cricheroes-1.0.8.dist-info/top_level.txt
+Filename: cricheroes-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: cricheroes-1.0.8.dist-info/RECORD
+Filename: cricheroes-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cricheroes/cricheroes.py

```diff
@@ -77,15 +77,18 @@
     @property
     def match_date(self):
         """
         Parse and return match date from info
         :return: date time object
 
         """
-        return parse(self.info, fuzzy=True).date()
+        datastring = self.info
+        if len(self.info) > 2:
+            datastring = self.info.split(",")[2]
+        return parse(datastring, fuzzy=True).date()
 
     @property
     def venue(self):
         """
         Parse and return venue from info
         :return: venue as str
 
@@ -196,15 +199,15 @@
                 print("Checking load more for element to appear. {}".format(time.time() - start_time))
 
             driver.find_element(value='body', by=By.TAG_NAME).send_keys(Keys.CONTROL + Keys.HOME)
             time.sleep(5)
         start_time = time.time()
         if match_text:
             while match_text not in driver.find_element(value=text_div_class_or_id, by=by).text.lower() and \
-                    time.time() - start_time < 60:
+                    time.time() - start_time < 30:
                 time.sleep(5)
                 print("Checking for matching element to appear . {}".format(time.time() - start_time))
         time.sleep(5)
         return copy.deepcopy(driver.page_source)
 
     def get_page_texts(self):
         data = {}
@@ -221,15 +224,15 @@
 
         # Matches tab
         data['members'] = copy.deepcopy(driver.page_source)
 
         # Matches tab
         data['matches'] = self.__click_and_fetch(driver,
                                                  tab='matchesTab',
-                                                 match_text="individual",
+                                                 match_text="result",
                                                  text_div_class_or_id='tournamentmatches'
                                                  )
         data['stats'] = self.__click_and_fetch(driver,
                                                tab='statTab',
                                                match_text="matches",
                                                text_div_class_or_id='statsDiv',
                                                by=By.CLASS_NAME
@@ -363,9 +366,9 @@
         out_path = base_dir / Path('out.json')
         with open(str(out_path.absolute()), 'w') as f:
             json.dump(self.fetch_all_data(), f, indent=4, cls=ChJsonEncoder)
         print("Json file created : " + str(out_path.absolute()))
 
 
 if __name__ == '__main__':
-    team = Team(url="2580003/CP-Sm@shers")
+    team = Team(url="345698/Spartans-CC---RED")
     team.dump_all()
```

## Comparing `cricheroes-1.0.8.dist-info/LICENSE` & `cricheroes-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cricheroes-1.0.8.dist-info/METADATA` & `cricheroes-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cricheroes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python APIs to fetch and store team data from cricheroes.in
 Home-page: https://github.com/pupattan/cricheroes
 Author: pattap
 Author-email: pulak.pattanayak@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `cricheroes-1.0.8.dist-info/RECORD` & `cricheroes-1.0.9.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 cricheroes/__init__.py,sha256=vrUwh4j4VmTtBLaB4uUMbMjyDioN4IlQ7lNX9aQAxFY,25
-cricheroes/cricheroes.py,sha256=XfzquaXnEaVB6IX_6YeVhzjR7TivIQG12JAv6u9UU6s,15239
-cricheroes-1.0.8.dist-info/LICENSE,sha256=lLCS2cUgWmp6yd5uvIiRF8kwyPs6jXMpZwL-Gchk_jU,1094
-cricheroes-1.0.8.dist-info/METADATA,sha256=uY5rhk-GN6ZCpJYyOIC5MAhR0znEw5dZ_2AEfquc0Zg,2762
-cricheroes-1.0.8.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-cricheroes-1.0.8.dist-info/top_level.txt,sha256=3v5PtwV0fPwe44nELTaEW_O-6-dsWtdD0oY3QI5phYg,11
-cricheroes-1.0.8.dist-info/RECORD,,
+cricheroes/cricheroes.py,sha256=waZaUOQHw5hPBHESv66KWdiKmqECn6uhAe00W6gr2EQ,15355
+cricheroes-1.0.9.dist-info/LICENSE,sha256=lLCS2cUgWmp6yd5uvIiRF8kwyPs6jXMpZwL-Gchk_jU,1094
+cricheroes-1.0.9.dist-info/METADATA,sha256=ATseozAx4X91zdm8yRkVDujkGNrSSOk-LbLGRUogCf0,2762
+cricheroes-1.0.9.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+cricheroes-1.0.9.dist-info/top_level.txt,sha256=3v5PtwV0fPwe44nELTaEW_O-6-dsWtdD0oY3QI5phYg,11
+cricheroes-1.0.9.dist-info/RECORD,,
```

