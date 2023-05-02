# Comparing `tmp/my_fake_useragent-0.2.0.tar.gz` & `tmp/my_fake_useragent-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\my_fake_useragent-0.2.0.tar", last modified: Mon Sep  7 07:26:54 2020, max compression
+gzip compressed data, was "my_fake_useragent-0.2.1.tar", last modified: Tue May  2 18:18:26 2023, max compression
```

## Comparing `my_fake_useragent-0.2.0.tar` & `my_fake_useragent-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2020-09-07 07:26:54.000000 my_fake_useragent-0.2.0/
--rw-rw-rw-   0        0        0     1210 2020-09-07 06:58:01.000000 my_fake_useragent-0.2.0/.gitignore
--rw-rw-rw-   0        0        0     1062 2020-09-07 07:21:33.000000 my_fake_useragent-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      106 2020-09-07 07:21:33.000000 my_fake_useragent-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3804 2020-09-07 07:26:54.000000 my_fake_useragent-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2056 2020-09-07 07:23:39.000000 my_fake_useragent-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2020-09-07 07:26:54.000000 my_fake_useragent-0.2.0/my_fake_useragent/
--rw-rw-rw-   0        0        0     3312 2020-09-07 07:14:17.000000 my_fake_useragent-0.2.0/my_fake_useragent/__init__.py
--rw-rw-rw-   0        0        0     2064 2020-09-07 06:58:01.000000 my_fake_useragent-0.2.0/my_fake_useragent/const.py
--rw-rw-rw-   0        0        0     2292 2020-09-07 07:21:33.000000 my_fake_useragent-0.2.0/my_fake_useragent/crawler.py
--rw-rw-rw-   0        0        0     3035 2020-09-07 06:58:01.000000 my_fake_useragent-0.2.0/my_fake_useragent/filter.py
--rw-rw-rw-   0        0        0  1699825 2020-09-07 07:12:19.000000 my_fake_useragent-0.2.0/my_fake_useragent/parsed_data.py
--rw-rw-rw-   0        0        0      338 2020-09-07 07:21:33.000000 my_fake_useragent-0.2.0/my_fake_useragent/utils.py
-drwxrwxrwx   0        0        0        0 2020-09-07 07:26:54.000000 my_fake_useragent-0.2.0/my_fake_useragent.egg-info/
--rw-rw-rw-   0        0        0     3804 2020-09-07 07:26:53.000000 my_fake_useragent-0.2.0/my_fake_useragent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2020-09-07 07:26:53.000000 my_fake_useragent-0.2.0/my_fake_useragent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-07 07:26:53.000000 my_fake_useragent-0.2.0/my_fake_useragent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2020-09-07 07:26:53.000000 my_fake_useragent-0.2.0/my_fake_useragent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2020-09-07 06:58:01.000000 my_fake_useragent-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0      102 2020-09-07 07:26:54.000000 my_fake_useragent-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1229 2020-09-07 06:58:01.000000 my_fake_useragent-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-09-07 07:26:54.000000 my_fake_useragent-0.2.0/tests/
--rw-rw-rw-   0        0        0      243 2020-09-07 07:16:52.000000 my_fake_useragent-0.2.0/tests/test_get_random_useragent.py
--rw-rw-rw-   0        0        0      406 2020-09-07 07:17:04.000000 my_fake_useragent-0.2.0/tests/test_json_data.py
--rw-rw-rw-   0        0        0      406 2020-09-07 07:16:52.000000 my_fake_useragent-0.2.0/tests/test_update_json_data.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:18:26.059188 my_fake_useragent-0.2.1/
+-rw-rw-rw-   0        0        0     1315 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/.gitignore
+-rw-rw-rw-   0        0        0     1083 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      113 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3052 2023-05-02 18:18:26.059188 my_fake_useragent-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2023-05-02 18:17:57.000000 my_fake_useragent-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 18:18:26.046010 my_fake_useragent-0.2.1/my_fake_useragent/
+-rw-rw-rw-   0        0        0     3423 2023-05-02 17:40:43.000000 my_fake_useragent-0.2.1/my_fake_useragent/__init__.py
+-rw-rw-rw-   0        0        0     2160 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/my_fake_useragent/const.py
+-rw-rw-rw-   0        0        0     2394 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/my_fake_useragent/crawler.py
+-rw-rw-rw-   0        0        0     3151 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/my_fake_useragent/filter.py
+-rw-rw-rw-   0        0        0  1715737 2023-05-02 17:49:50.000000 my_fake_useragent-0.2.1/my_fake_useragent/parsed_data.py
+-rw-rw-rw-   0        0        0      353 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/my_fake_useragent/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:18:26.056932 my_fake_useragent-0.2.1/my_fake_useragent.egg-info/
+-rw-rw-rw-   0        0        0     3052 2023-05-02 18:18:25.000000 my_fake_useragent-0.2.1/my_fake_useragent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2023-05-02 18:18:26.000000 my_fake_useragent-0.2.1/my_fake_useragent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:18:25.000000 my_fake_useragent-0.2.1/my_fake_useragent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-02 18:18:25.000000 my_fake_useragent-0.2.1/my_fake_useragent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       53 2023-05-02 17:27:32.000000 my_fake_useragent-0.2.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0      102 2023-05-02 18:18:26.059188 my_fake_useragent-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:18:26.059188 my_fake_useragent-0.2.1/tests/
+-rw-rw-rw-   0        0        0      326 2023-05-02 18:11:12.000000 my_fake_useragent-0.2.1/tests/test_get_random_useragent.py
+-rw-rw-rw-   0        0        0      170 2023-05-02 17:58:00.000000 my_fake_useragent-0.2.1/tests/test_json_data.py
+-rw-rw-rw-   0        0        0      425 2023-05-02 16:57:02.000000 my_fake_useragent-0.2.1/tests/test_update_json_data.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `my_fake_useragent-0.2.0/LICENSE` & `my_fake_useragent-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 wanze
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 wanze
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `my_fake_useragent-0.2.0/my_fake_useragent/__init__.py` & `my_fake_useragent-0.2.1/my_fake_useragent/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-#!/usr/bin/env python
-# -*-coding:utf-8-*-
-
-import random
-
-from .filter import filter_family, filter_os_family, filter_phone, \
-    filter_version_range
-from .utils import build_stream_function
-
-
-class UserAgent():
-    from my_fake_useragent.parsed_data import parsed_data
-
-    def __init__(self,
-                 family=None,
-                 os_family=None,
-                 phone=None,
-                 version_range=None,
-                 ):
-        """
-
-        :param mode: default mode
-        :param family: 不设置则不管 指定浏览器类型
-        :param os_family: 不设置则不管 指定操作系统
-        :param phone: 指定是否是手机端 True 是 False 不是 不设置默认None则不管
-        :param version_range: 不设置则不管 指定浏览器版本范围
-
-        手机检测 根据设备family参数之外 操作系统检测到 android 或 ios 也认为是移动端
-
-        """
-
-        if isinstance(family, str):
-            family = family.lower()
-            self.family = [family]
-        elif isinstance(family, (list, tuple)):
-            self.family = [f.lower() for f in family]
-        elif family is None:
-            self.family = None
-        else:
-            raise ValueError('family')
-
-        if isinstance(os_family, str):
-            os_family = os_family.lower()
-            self.os_family = [os_family]
-        elif isinstance(os_family, (list, tuple)):
-            self.os_family = [f.lower() for f in os_family]
-        elif os_family is None:
-            self.os_family = None
-        else:
-            raise ValueError('os_family')
-
-        self.phone = phone
-        if self.phone not in [None, True, False]:
-            raise ValueError('phone')
-
-        self.version_range = version_range
-
-        self.filter_func = build_stream_function(filter_family,
-                                                 filter_os_family, filter_phone,
-                                                 filter_version_range)
-
-    def random(self):
-        user_agent_list = self.get_useragent_list()
-
-        if user_agent_list:
-            return random.choice(user_agent_list)
-        else:
-            raise Exception('empty result')
-
-    def get_useragent_list(self):
-        origin_data = []
-        for key in self.parsed_data:
-            origin_data += self.parsed_data[key]
-
-        d = {
-            'data': origin_data,
-            'family': self.family,
-            'version_range': self.version_range,
-            'os_family': self.os_family,
-            'phone': self.phone
-        }
-
-        d = self.filter_func(d)
-
-        ua_string_list = [i['string'] for i in d['data']]
-        return ua_string_list
-
-    def test_possible_family(self):
-        t1 = set()
-        for k, v in self.parsed_data.items():
-            for i in v:
-                t1.add(i['user_agent']['family'])
-        return t1
-
-    def test_possible_os_family(self):
-        t1 = set()
-        for k, v in self.parsed_data.items():
-            for i in v:
-                t1.add(i['os']['family'])
-        return t1
-
-    def test_possible_device_family(self):
-        t1 = set()
-        for k, v in self.parsed_data.items():
-            for i in v:
-                t1.add(i['device']['family'])
-        return t1
-
-
-__softname__ = 'my_fake_useragent'
-__version__ = '0.2.0'
+#!/usr/bin/env python
+# -*-coding:utf-8-*-
+
+import random
+
+from .filter import filter_family, filter_os_family, filter_phone, \
+    filter_version_range
+from .utils import build_stream_function
+
+
+class UserAgent():
+    from my_fake_useragent.parsed_data import parsed_data
+
+    def __init__(self,
+                 family=None,
+                 os_family=None,
+                 phone=None,
+                 version_range=None,
+                 ):
+        """
+
+        :param mode: default mode
+        :param family: 不设置则不管 指定浏览器类型
+        :param os_family: 不设置则不管 指定操作系统
+        :param phone: 指定是否是手机端 True 是 False 不是 不设置默认None则不管
+        :param version_range: 不设置则不管 指定浏览器版本范围
+
+        手机检测 根据设备family参数之外 操作系统检测到 android 或 ios 也认为是移动端
+
+        """
+
+        if isinstance(family, str):
+            family = family.lower()
+            self.family = [family]
+        elif isinstance(family, (list, tuple)):
+            self.family = [f.lower() for f in family]
+        elif family is None:
+            self.family = None
+        else:
+            raise ValueError('family')
+
+        if isinstance(os_family, str):
+            os_family = os_family.lower()
+            self.os_family = [os_family]
+        elif isinstance(os_family, (list, tuple)):
+            self.os_family = [f.lower() for f in os_family]
+        elif os_family is None:
+            self.os_family = None
+        else:
+            raise ValueError('os_family')
+
+        self.phone = phone
+        if self.phone not in [None, True, False]:
+            raise ValueError('phone')
+
+        self.version_range = version_range
+
+        self.filter_func = build_stream_function(filter_family,
+                                                 filter_os_family, filter_phone,
+                                                 filter_version_range)
+
+    def random(self):
+        user_agent_list = self.get_useragent_list()
+
+        if user_agent_list:
+            return random.choice(user_agent_list)
+        else:
+            raise Exception('empty result')
+
+    def get_useragent_list(self):
+        origin_data = []
+        for key in self.parsed_data:
+            origin_data += self.parsed_data[key]
+
+        d = {
+            'data': origin_data,
+            'family': self.family,
+            'version_range': self.version_range,
+            'os_family': self.os_family,
+            'phone': self.phone
+        }
+
+        d = self.filter_func(d)
+
+        ua_string_list = [i['string'] for i in d['data']]
+        return ua_string_list
+
+    def test_possible_family(self):
+        t1 = set()
+        for k, v in self.parsed_data.items():
+            for i in v:
+                t1.add(i['user_agent']['family'])
+        return t1
+
+    def test_possible_os_family(self):
+        t1 = set()
+        for k, v in self.parsed_data.items():
+            for i in v:
+                t1.add(i['os']['family'])
+        return t1
+
+    def test_possible_device_family(self):
+        t1 = set()
+        for k, v in self.parsed_data.items():
+            for i in v:
+                t1.add(i['device']['family'])
+        return t1
+
+
+__softname__ = 'my_fake_useragent'
+__version__ = '0.2.1'
```

### Comparing `my_fake_useragent-0.2.0/my_fake_useragent/crawler.py` & `my_fake_useragent-0.2.1/my_fake_useragent/crawler.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-#!/usr/bin/env python
-# -*-coding:utf-8-*-
-
-import re
-import json
-import requests
-from bs4 import BeautifulSoup
-from collections import defaultdict
-
-from my_fake_useragent.const import SUPPORT_TYPES
-
-ALL_DETAIL_URL = 'http://www.useragentstring.com/pages/useragentstring.php?name=All'
-
-WEB_TIMEOUT = 30
-
-
-def write_json(file, data):
-    with open(file, 'w', encoding='utf8') as f:
-        json.dump(data, f, indent=4, ensure_ascii=False)
-
-
-def update_json_data():
-    res = requests.get(ALL_DETAIL_URL, timeout=WEB_TIMEOUT)
-
-    soup = BeautifulSoup(res.text, 'html5lib')
-
-    liste = soup.find(id='liste')
-
-    data = defaultdict(list)
-
-    h3_text = None
-    for item in liste.find_all(recursive=False):
-
-        if item.name == 'h3':
-            h3_text = item.text
-
-            data[h3_text] = []
-
-        if item.find_all('a'):
-            a_list = item.find_all('a')
-            for a in a_list:
-                s = a.text
-                # adjust
-                if re.match('^More ', s):
-                    continue
-
-                if h3_text in data:
-                    data[h3_text].append(s)
-
-    write_json('data.json', data)
-
-    return 0
-
-
-def update_parsed_json_data():
-    """
-    更新parsed_json_data
-    :return:
-    """
-    json_data = load_json_data()
-    from ua_parser import user_agent_parser
-    from collections import defaultdict
-    new_json_data = defaultdict(list)
-
-    for key, value in json_data.items():
-        if value:
-            for us_string in value:
-                ua_parsed = user_agent_parser.Parse(us_string)
-                item_data = dict(ua_parsed)
-                new_json_data[key].append(item_data)
-        else:
-            new_json_data[key] = []
-
-    write_json('parsed_data.json', new_json_data)
-
-    return 0
-
-
-def load_json_data():
-    f = open("data.json", encoding='utf8')
-
-    res = json.load(f)
-    return res
-
-
-def load_parsed_json_data():
-    f = open("parsed_data.json", encoding='utf8')
-
-    res = json.load(f)
-
-    new_res = {}
-    for k in res:
-        if k in SUPPORT_TYPES:
-            new_res[k] = res[k]
-
-    return new_res
-
-
-def convert_parsed_data_py():
-    parsed_data_json = load_parsed_json_data()
-    with open('parsed_data.py', 'w', encoding='utf8') as f:
-        f.write(f'parsed_data = {parsed_data_json}')
+#!/usr/bin/env python
+# -*-coding:utf-8-*-
+
+import re
+import json
+import requests
+from bs4 import BeautifulSoup
+from collections import defaultdict
+
+from my_fake_useragent.const import SUPPORT_TYPES
+
+ALL_DETAIL_URL = 'http://www.useragentstring.com/pages/useragentstring.php?name=All'
+
+WEB_TIMEOUT = 30
+
+
+def write_json(file, data):
+    with open(file, 'w', encoding='utf8') as f:
+        json.dump(data, f, indent=4, ensure_ascii=False)
+
+
+def update_json_data():
+    res = requests.get(ALL_DETAIL_URL, timeout=WEB_TIMEOUT)
+
+    soup = BeautifulSoup(res.text, 'html5lib')
+
+    liste = soup.find(id='liste')
+
+    data = defaultdict(list)
+
+    h3_text = None
+    for item in liste.find_all(recursive=False):
+
+        if item.name == 'h3':
+            h3_text = item.text
+
+            data[h3_text] = []
+
+        if item.find_all('a'):
+            a_list = item.find_all('a')
+            for a in a_list:
+                s = a.text
+                # adjust
+                if re.match('^More ', s):
+                    continue
+
+                if h3_text in data:
+                    data[h3_text].append(s)
+
+    write_json('data.json', data)
+
+    return 0
+
+
+def update_parsed_json_data():
+    """
+    更新parsed_json_data
+    :return:
+    """
+    json_data = load_json_data()
+    from ua_parser import user_agent_parser
+    from collections import defaultdict
+    new_json_data = defaultdict(list)
+
+    for key, value in json_data.items():
+        if value:
+            for us_string in value:
+                ua_parsed = user_agent_parser.Parse(us_string)
+                item_data = dict(ua_parsed)
+                new_json_data[key].append(item_data)
+        else:
+            new_json_data[key] = []
+
+    write_json('parsed_data.json', new_json_data)
+
+    return 0
+
+
+def load_json_data():
+    f = open("data.json", encoding='utf8')
+
+    res = json.load(f)
+    return res
+
+
+def load_parsed_json_data():
+    f = open("parsed_data.json", encoding='utf8')
+
+    res = json.load(f)
+
+    new_res = {}
+    for k in res:
+        if k in SUPPORT_TYPES:
+            new_res[k] = res[k]
+
+    return new_res
+
+
+def convert_parsed_data_py():
+    parsed_data_json = load_parsed_json_data()
+    with open('parsed_data.py', 'w', encoding='utf8') as f:
+        f.write(f'parsed_data = {parsed_data_json}')
```

### Comparing `my_fake_useragent-0.2.0/my_fake_useragent/filter.py` & `my_fake_useragent-0.2.1/my_fake_useragent/filter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-#!/usr/bin/env python
-# -*-coding:utf-8-*-
-
-import logging
-from .const import FAMILY_MAP, PHONE_DEVICE_FAMILY_LIST, OS_FAMILY_MAP
-
-logger = logging.getLogger(__name__)
-
-
-def filter_family(d):
-    data = d['data']
-    family = d.get('family')
-
-    if family:
-        extend_family = []
-        for i in family:
-            if i in FAMILY_MAP:
-                extend_item = FAMILY_MAP[i]
-            else:
-                extend_item = [i]
-            extend_family += extend_item
-
-        new_data = []
-        for item_data in data:
-            target_family = item_data['user_agent']['family']
-
-            if target_family in extend_family:
-                new_data.append(item_data)
-
-        d['data'] = new_data
-    return d
-
-
-def filter_os_family(d):
-    data = d['data']
-    os_family = d.get('os_family')
-
-    if os_family:
-        extend_family = []
-        for i in os_family:
-            if i in OS_FAMILY_MAP:
-                extend_item = OS_FAMILY_MAP[i]
-            else:
-                extend_item = [i]
-            extend_family += extend_item
-
-        new_data = []
-        for item_data in data:
-            target_os_family = item_data['os']['family']
-
-            if target_os_family in extend_family:
-                new_data.append(item_data)
-
-        d['data'] = new_data
-    return d
-
-
-def filter_phone(d):
-    data = d['data']
-    phone = d.get('phone')
-
-    if phone is None:
-        return d
-    extend_family = []
-    for i in ['android', 'ios']:
-        if i in OS_FAMILY_MAP:
-            extend_item = OS_FAMILY_MAP[i]
-        else:
-            extend_item = [i]
-        extend_family += extend_item
-
-    if phone:
-        new_data = []
-        for item_data in data:
-            target_device_family = item_data['device']['family']
-            target_os_family = item_data['os']['family']
-
-            if target_device_family in PHONE_DEVICE_FAMILY_LIST:
-                new_data.append(item_data)
-            elif target_os_family in extend_family:
-                new_data.append(item_data)
-
-        d['data'] = new_data
-        return d
-    else:
-        # phone is False only return computer webbrower
-        new_data = []
-        for item_data in data:
-            target_device_family = item_data['device']['family']
-            target_os_family = item_data['os']['family']
-
-            extend_family = []
-            for i in ['android', 'ios']:
-                if i in OS_FAMILY_MAP:
-                    extend_item = OS_FAMILY_MAP[i]
-                else:
-                    extend_item = [i]
-                extend_family += extend_item
-
-            if target_device_family in PHONE_DEVICE_FAMILY_LIST:
-                pass
-            elif target_os_family in extend_family:
-                pass
-            else:
-                new_data.append(item_data)
-
-        d['data'] = new_data
-        return d
-
-
-def filter_version_range(d):
-    data = d['data']
-    version_range = d.get('version_range')
-    if version_range is not None:
-        logger.warning('not implement yet')
-    return d
+#!/usr/bin/env python
+# -*-coding:utf-8-*-
+
+import logging
+from .const import FAMILY_MAP, PHONE_DEVICE_FAMILY_LIST, OS_FAMILY_MAP
+
+logger = logging.getLogger(__name__)
+
+
+def filter_family(d):
+    data = d['data']
+    family = d.get('family')
+
+    if family:
+        extend_family = []
+        for i in family:
+            if i in FAMILY_MAP:
+                extend_item = FAMILY_MAP[i]
+            else:
+                extend_item = [i]
+            extend_family += extend_item
+
+        new_data = []
+        for item_data in data:
+            target_family = item_data['user_agent']['family']
+
+            if target_family in extend_family:
+                new_data.append(item_data)
+
+        d['data'] = new_data
+    return d
+
+
+def filter_os_family(d):
+    data = d['data']
+    os_family = d.get('os_family')
+
+    if os_family:
+        extend_family = []
+        for i in os_family:
+            if i in OS_FAMILY_MAP:
+                extend_item = OS_FAMILY_MAP[i]
+            else:
+                extend_item = [i]
+            extend_family += extend_item
+
+        new_data = []
+        for item_data in data:
+            target_os_family = item_data['os']['family']
+
+            if target_os_family in extend_family:
+                new_data.append(item_data)
+
+        d['data'] = new_data
+    return d
+
+
+def filter_phone(d):
+    data = d['data']
+    phone = d.get('phone')
+
+    if phone is None:
+        return d
+    extend_family = []
+    for i in ['android', 'ios']:
+        if i in OS_FAMILY_MAP:
+            extend_item = OS_FAMILY_MAP[i]
+        else:
+            extend_item = [i]
+        extend_family += extend_item
+
+    if phone:
+        new_data = []
+        for item_data in data:
+            target_device_family = item_data['device']['family']
+            target_os_family = item_data['os']['family']
+
+            if target_device_family in PHONE_DEVICE_FAMILY_LIST:
+                new_data.append(item_data)
+            elif target_os_family in extend_family:
+                new_data.append(item_data)
+
+        d['data'] = new_data
+        return d
+    else:
+        # phone is False only return computer webbrower
+        new_data = []
+        for item_data in data:
+            target_device_family = item_data['device']['family']
+            target_os_family = item_data['os']['family']
+
+            extend_family = []
+            for i in ['android', 'ios']:
+                if i in OS_FAMILY_MAP:
+                    extend_item = OS_FAMILY_MAP[i]
+                else:
+                    extend_item = [i]
+                extend_family += extend_item
+
+            if target_device_family in PHONE_DEVICE_FAMILY_LIST:
+                pass
+            elif target_os_family in extend_family:
+                pass
+            else:
+                new_data.append(item_data)
+
+        d['data'] = new_data
+        return d
+
+
+def filter_version_range(d):
+    data = d['data']
+    version_range = d.get('version_range')
+    if version_range is not None:
+        logger.warning('not implement yet')
+    return d
```

### Comparing `my_fake_useragent-0.2.0/my_fake_useragent/parsed_data.py` & `my_fake_useragent-0.2.1/my_fake_useragent/parsed_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
```

### Comparing `my_fake_useragent-0.2.0/setup.py` & `my_fake_useragent-0.2.1/setup.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-#!/usr/bin/env python
-# -*-coding:utf-8-*-
-
-import os
-from setuptools import setup, find_packages
-import my_fake_useragent
-
-REQUIREMENTS = []
-
-this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='my_fake_useragent',
-    version=my_fake_useragent.__version__,
-    description='create a fake useragent',
-    url='https://github.com/a358003542/my-fake-useragent',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='wanze',
-    author_email='a358003542@gmail.com',
-    maintainer='wanze',
-    maintainer_email='a358003542@gmail.com',
-    license='MIT',
-    keywords=['useragent', 'python'],
-    classifiers=['Development Status :: 4 - Beta',
-                 'Operating System :: Microsoft :: Windows',
-                 'Operating System :: POSIX :: Linux',
-                 'License :: OSI Approved :: MIT License',
-                 'Programming Language :: Python :: 3', ],
-    packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
-    include_package_data=True,
-    setup_requires=REQUIREMENTS,
-    install_requires=REQUIREMENTS,
-)
+#!/usr/bin/env python
+# -*-coding:utf-8-*-
+
+import os
+from setuptools import setup, find_packages
+import my_fake_useragent
+
+REQUIREMENTS = []
+
+this_directory = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='my_fake_useragent',
+    version=my_fake_useragent.__version__,
+    description='create a fake useragent',
+    url='https://github.com/a358003542/my-fake-useragent',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author='wanze',
+    author_email='a358003542@gmail.com',
+    maintainer='wanze',
+    maintainer_email='a358003542@gmail.com',
+    license='MIT',
+    keywords=['useragent', 'python'],
+    classifiers=['Development Status :: 4 - Beta',
+                 'Operating System :: Microsoft :: Windows',
+                 'Operating System :: POSIX :: Linux',
+                 'License :: OSI Approved :: MIT License',
+                 'Programming Language :: Python :: 3', ],
+    packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
+    include_package_data=True,
+    setup_requires=REQUIREMENTS,
+    install_requires=REQUIREMENTS,
+)
```
