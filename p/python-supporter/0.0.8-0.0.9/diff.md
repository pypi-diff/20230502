# Comparing `tmp/python-supporter-0.0.8.tar.gz` & `tmp/python-supporter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-supporter-0.0.8.tar", last modified: Sun Mar 19 13:59:17 2023, max compression
+gzip compressed data, was "python-supporter-0.0.9.tar", last modified: Tue Mar 28 05:52:14 2023, max compression
```

## Comparing `python-supporter-0.0.8.tar` & `python-supporter-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 13:59:17.736149 python-supporter-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1795 2023-03-19 13:59:17.735149 python-supporter-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1519 2023-03-19 13:59:16.000000 python-supporter-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 13:59:17.734149 python-supporter-0.0.8/python_supporter/
--rw-r--r--   0 root         (0) root         (0)      149 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/cache.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/config.py
--rw-r--r--   0 root         (0) root         (0)      202 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/file.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/logging.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/obfuscator.py
--rw-r--r--   0 root         (0) root         (0)      128 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/random.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-03-19 13:59:16.000000 python-supporter-0.0.8/python_supporter/socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-19 13:59:17.735149 python-supporter-0.0.8/python_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1795 2023-03-19 13:59:17.000000 python-supporter-0.0.8/python_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      437 2023-03-19 13:59:17.000000 python-supporter-0.0.8/python_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-19 13:59:17.000000 python-supporter-0.0.8/python_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-19 13:59:17.000000 python-supporter-0.0.8/python_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-19 13:59:17.000000 python-supporter-0.0.8/python_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-19 13:59:17.737150 python-supporter-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-19 13:59:16.000000 python-supporter-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 05:52:14.231076 python-supporter-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      867 2023-03-28 05:52:14.230076 python-supporter-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      591 2023-03-28 05:52:13.000000 python-supporter-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 05:52:14.230076 python-supporter-0.0.9/python_supporter/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/config.py
+-rw-r--r--   0 root         (0) root         (0)      202 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/file.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/logging.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/obfuscator.py
+-rw-r--r--   0 root         (0) root         (0)      128 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/random.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-03-28 05:52:13.000000 python-supporter-0.0.9/python_supporter/socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 05:52:14.230076 python-supporter-0.0.9/python_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      867 2023-03-28 05:52:14.000000 python-supporter-0.0.9/python_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      437 2023-03-28 05:52:14.000000 python-supporter-0.0.9/python_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 05:52:14.000000 python-supporter-0.0.9/python_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 05:52:14.000000 python-supporter-0.0.9/python_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2023-03-28 05:52:14.000000 python-supporter-0.0.9/python_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-28 05:52:14.231076 python-supporter-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      600 2023-03-28 05:52:13.000000 python-supporter-0.0.9/setup.py
```

### Comparing `python-supporter-0.0.8/python_supporter/cache.py` & `python-supporter-0.0.9/python_supporter/cache.py`

 * *Files identical despite different names*

### Comparing `python-supporter-0.0.8/python_supporter/config.py` & `python-supporter-0.0.9/python_supporter/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,16 +34,28 @@
         return config
     return None
 
 def load_config_from_json_text(json_text):
     config = json.loads(json_text)
     return config
 
+'''
 def save_config(file, config):
     with open(file, "w", encoding='utf8') as f:
         json.dump(config, f, indent=4)
 
 def save_json_text(file, json_text):
     with open(file, "w", encoding='utf8') as f: #이렇게 저장해야 한글 제데로 나옴
         f.write(json_text)
     #config = json.loads(json_text)
     #save_config(file, config)
+'''
+
+def save_config(file, config):
+    with open(file, "w", encoding='utf8') as f:
+        json.dump(config, f, indent=4, ensure_ascii=False) #ensure_ascii=False 해줘야 한글이 \uac1c\ubc1c 이 아닌 개발로 정상적으로 표현
+
+def save_json_text(file, json_text):
+    #with open(file, "w", encoding='utf8') as f: #이렇게 저장해야 한글 제데로 나옴
+    #    f.write(json_text)
+    config = json.loads(json_text)
+    save_config(file, config)
```

### Comparing `python-supporter-0.0.8/python_supporter/obfuscator.py` & `python-supporter-0.0.9/python_supporter/obfuscator.py`

 * *Files identical despite different names*

### Comparing `python-supporter-0.0.8/setup.py` & `python-supporter-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='python-supporter',
-	version='0.0.8',
+	version='0.0.9',
 	description='Python supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/python-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

