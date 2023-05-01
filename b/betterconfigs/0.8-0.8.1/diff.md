# Comparing `tmp/betterconfigs-0.8.tar.gz` & `tmp/betterconfigs-0.8.1.tar.gz`

## Comparing `betterconfigs-0.8.tar` & `betterconfigs-0.8.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 betterconfigs-0.8/buildscript.sh
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 betterconfigs-0.8/test_conf.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 betterconfigs-0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 betterconfigs-0.8/src/betterconfigs/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 betterconfigs-0.8/src/betterconfigs/utilities.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 betterconfigs-0.8/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 betterconfigs-0.8/LICENSE
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 betterconfigs-0.8/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 betterconfigs-0.8/pyproject.toml
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 betterconfigs-0.8/PKG-INFO
+-rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/buildscript.sh
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/test_conf.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/src/betterconfigs/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/src/betterconfigs/utilities.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/README.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 betterconfigs-0.8.1/PKG-INFO
```

### Comparing `betterconfigs-0.8/test_conf.py` & `betterconfigs-0.8.1/test_conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from src.betterconfigs import *
 import os
 import pytest
+def test_cleanup():
+    try:
+        os.remove('test.config')
+    except:
+        pass
+    assert(os.path.exists('test.config')==False)
 def test_basic():
     h = config('test.config')
     h['hello'] = 'world'
     assert(h['hello']=='world')
     assert(h['_version']==executableVersion)
     os.remove('test.config')
 def test_remove():
@@ -27,23 +33,22 @@
     h = config('test.config')
     assert(h['_encrypted']==False)
     assert(h.encKey!=None)
     t = config('test.config')
     assert(t['_encrypted']==False)
     assert(t.encKey==None)
     os.remove('test.config')
-def test_encryption():
     h = config('test.config')
     assert(h['_encrypted']==False)
     assert(h.encKey!=None)
     h['hello']='world'
     assert(h.encryptFile()==0)
     assert(h['hello']=='world')
     assert(h.getRaw('hello')!='world')
-    assert(h.getRaw('_version')=='0.7')
+    assert(h.getRaw('_version')=='0.8.1')
     encryptionKey = h.encKey
     t = config('test.config')
     assert(t.getRaw('_encrypted')==True)
     with pytest.raises(Exception):
         t['hello']='world'
     os.remove('test.config')
 def test_decryption():
@@ -73,8 +78,36 @@
     h['hello2']='world2'
     encryptionKey = h.encKey
     t = config('test.config')
     t.encKey = encryptionKey
     assert(t['hello']=='world')
     assert(t['hello2']=='world2')
     assert(t.decryptFile()==0)
+    os.remove('test.config')
+def test_encdec_int():
+    h = config('test.config')
+    h['hello']='world'
+    assert(h.encryptFile()==0)
+    h['hello2']=3
+    assert(h['hello2']==3)
+    os.remove('test.config')
+def test_encdec_bool():
+    h = config('test.config')
+    h['hello']='world'
+    assert(h.encryptFile()==0)
+    h['hello2']=True
+    assert(h['hello2']==True)
+    os.remove('test.config')
+def test_encdec_list():
+    h = config('test.config')
+    h['hello']='world'
+    assert(h.encryptFile()==0)
+    h['hello2']=['hello','world']
+    assert(h['hello2']==['hello','world'])
+    os.remove('test.config')
+def test_encdec_badtype():
+    h = config('test.config')
+    h['hello']='world'
+    assert(h.encryptFile()==0)
+    with pytest.raises(Exception):
+        h['hello2']=21.49857203958
     os.remove('test.config')
```

### Comparing `betterconfigs-0.8/.github/workflows/python-publish.yml` & `betterconfigs-0.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8/src/betterconfigs/__init__.py` & `betterconfigs-0.8.1/src/betterconfigs/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pickle
 import os
 import warnings
 from cryptography.fernet import Fernet
-executableVersion = "0.8"
+executableVersion = "0.8.1"
+supportedTypes=[int, str, list, bool]
 class config:
     def __init__(self, path) -> None:
         self.path = path
         self.encKey = None
         if os.path.exists(path)==False:
             try:
                 loadConfig = {}
@@ -80,19 +81,44 @@
         if self.decryptValue('_checksum')==self.encKey.decode():
             return 0
         else:
             return 1
     def encryptValue(self, value):
         self.checkReady()
         fernet = Fernet(self.encKey)
-        return fernet.encrypt(value.encode())
+        if type(value) not in supportedTypes:
+            raise Exception("type "+ type(value)+ " is not supported for encryption")
+        if 'bool.e' in str(value) or 'int.e' in str(value):
+            raise Exception("value contains encoding information before encoding occurred")
+        if type(value) is int:
+            return fernet.encrypt(("int.e"+str(value)).encode())
+        elif type(value) is bool:
+            return fernet.encrypt(("bool.e"+str(value)).encode())
+        elif type(value) is list:
+            encList = []
+            for i in value:
+                encList.append(fernet.encrypt(i.encode()))
+            return encList
+        else:
+            return fernet.encrypt(value.encode())
     def decryptValue(self, key):
         self.checkReady()
         fernet = Fernet(self.encKey)
-        return fernet.decrypt(self.getRaw(key)).decode()
+        if type(self.getRaw(key)) is list:
+            decList=[]
+            for i in self.getRaw(key):
+                decList.append(fernet.decrypt(i).decode())
+            return decList
+        dec = fernet.decrypt(self.getRaw(key)).decode()
+        if dec[0:5]=='int.e':
+            return int(dec[5:])
+        elif dec[0:6]=='bool.e':
+            return bool(dec[6:])
+        else:
+            return dec
     def encryptFile(self):
         self.checkReady()
         with open(self.path, 'rb') as handle:
                 loadedConfig = pickle.load(handle)
         for i in loadedConfig:
             if not i.startswith("_"):
                 loadedConfig[i] = self.encryptValue(loadedConfig[i])
```

### Comparing `betterconfigs-0.8/LICENSE` & `betterconfigs-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betterconfigs-0.8/README.md` & `betterconfigs-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 t['hello'] = 'world'
 print(t['hello'])
 ```
 
 ## Encrypting/Decrypting
 With version 0.8 of BetterConfigs, you can now encrypt and decrypt your configuration files on the fly. This is great in the case you need to sync configurations, and don't want them to be available to prying eyes.
 
-To get started, use the `encyptFile()` function after you've created the `config` object. This will encrypt all existing configurations in the file, as well as provide you with an encryption key stored in the property `encKey`. When the configuration object is destroyed, the `encKey` value is also unloaded from memory, so make sure you save it!
+To get started, use the `encryptFile()` function after you've created the `config` object. This will encrypt all existing configurations in the file, as well as provide you with an encryption key stored in the property `encKey`. When the configuration object is destroyed, the `encKey` value is also unloaded from memory, so make sure you save it!
 
 To open an encrypted configuration file, create the object again, and set the `encKey` value to the same one used to encrypt it previously. Then, just access the configuration as normal, and BetterConfigs handles everything for you.
 
 Finally, to decrypt the file, make sure the `encKey` value is set correctly, and use the `decryptFile()` function.
```

### Comparing `betterconfigs-0.8/PKG-INFO` & `betterconfigs-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: betterconfigs
-Version: 0.8
+Version: 0.8.1
 Summary: A small package to simplify configuration storing and retrieving
 Project-URL: Homepage, https://github.com/iainrosen/betterconfigs
 Project-URL: Bug Tracker, https://github.com/iainrosen/betterconfigs/issues
 Author-email: Iain Rosen <hello@iainrosen.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: cryptography
+Requires-Dist: pickle
+Requires-Dist: warnings
 Description-Content-Type: text/markdown
 
 # BetterConfigs
 
 A small package to simplify configuration storing and retrieving
 
 ## Usage
@@ -32,12 +35,12 @@
 t['hello'] = 'world'
 print(t['hello'])
 ```
 
 ## Encrypting/Decrypting
 With version 0.8 of BetterConfigs, you can now encrypt and decrypt your configuration files on the fly. This is great in the case you need to sync configurations, and don't want them to be available to prying eyes.
 
-To get started, use the `encyptFile()` function after you've created the `config` object. This will encrypt all existing configurations in the file, as well as provide you with an encryption key stored in the property `encKey`. When the configuration object is destroyed, the `encKey` value is also unloaded from memory, so make sure you save it!
+To get started, use the `encryptFile()` function after you've created the `config` object. This will encrypt all existing configurations in the file, as well as provide you with an encryption key stored in the property `encKey`. When the configuration object is destroyed, the `encKey` value is also unloaded from memory, so make sure you save it!
 
 To open an encrypted configuration file, create the object again, and set the `encKey` value to the same one used to encrypt it previously. Then, just access the configuration as normal, and BetterConfigs handles everything for you.
 
 Finally, to decrypt the file, make sure the `encKey` value is set correctly, and use the `decryptFile()` function.
```

