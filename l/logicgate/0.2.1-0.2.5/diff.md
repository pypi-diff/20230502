# Comparing `tmp/LogicGate-0.2.1.tar.gz` & `tmp/LogicGate-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogicGate-0.2.1.tar", max compression
+gzip compressed data, was "LogicGate-0.2.5.tar", max compression
```

## Comparing `LogicGate-0.2.1.tar` & `LogicGate-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 LogicGate-0.2.1/LICENSE
--rw-r--r--   0        0        0    12581 2023-05-01 00:34:55.780982 LogicGate-0.2.1/LogicGate/LogicGate.py
--rw-r--r--   0        0        0     4209 2023-04-28 07:41:48.636486 LogicGate-0.2.1/LogicGate/lgEncrypt.py
--rw-r--r--   0        0        0     5175 2023-04-28 07:51:30.723628 LogicGate-0.2.1/README.rst
--rw-r--r--   0        0        0      773 2023-05-01 00:47:23.903948 LogicGate-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6066 2023-05-01 00:47:59.184358 LogicGate-0.2.1/setup.py
--rw-r--r--   0        0        0     5902 2023-05-01 00:47:59.184880 LogicGate-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 LogicGate-0.2.5/LICENSE
+-rw-r--r--   0        0        0    12712 2023-05-02 13:24:30.526632 LogicGate-0.2.5/LogicGate/LogicGate.py
+-rw-r--r--   0        0        0     4315 2023-05-02 13:22:24.970750 LogicGate-0.2.5/LogicGate/lgEncrypt.py
+-rw-r--r--   0        0        0     5175 2023-04-28 07:51:30.723628 LogicGate-0.2.5/README.rst
+-rw-r--r--   0        0        0      773 2023-05-02 13:25:40.426566 LogicGate-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6066 2023-05-02 13:25:55.297106 LogicGate-0.2.5/setup.py
+-rw-r--r--   0        0        0     5902 2023-05-02 13:25:55.300955 LogicGate-0.2.5/PKG-INFO
```

### Comparing `LogicGate-0.2.1/LICENSE` & `LogicGate-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LogicGate-0.2.1/LogicGate/LogicGate.py` & `LogicGate-0.2.5/LogicGate/LogicGate.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
   else:
     sys.stdout = open(os.devnull, 'w')
   if exists(filename):
     with open(filename, 'r') as f:
       f.seek(0,0)
       Out = [[]]
       dt = f.readlines()
-      if filename[-6:] != '.lgeso':
+      if not filename.endswith('.lgeso'):
         sys.tracebacklimit = 0
         sys.stdout = sys.__stdout__
         raise NameError(
           f'{filename} is not an lgeso file, maybe renaming the file extension to lgeso and try again')
       for dtidx, line in enumerate(dt):
         line = line.replace('\n', '')
         if '---' in line:
@@ -232,14 +232,16 @@
   random_range: list, the maximum set of gates in the written data will be the square of the second item while the minimum will be the square of the first item.
   write: boolean, if the result is returned or is written to file
   override: boolean, safety checks are off, proceed with caution
   BitLock: integer, if the binary of a character is shorter than this value, 0 will be appended. Defalt is -1, which is off, all negative number will be counted as ignore as well"""
 
   out = ""
   override = not override
+  if not output.isascii() and override:
+    raise ValueError(f'message received ({repr(output)}) is not available in ascii')
   if not output and override:
     output = 'Hello World!'
   if filename and write and override:
     if len(filename) > 6:
       if filename[-6:] != '.lgeso':
         print(f'filename is not an lgeso file, filename changed to {filename}')
         filename += '.lgeso'
```

### Comparing `LogicGate-0.2.1/LogicGate/lgEncrypt.py` & `LogicGate-0.2.5/LogicGate/lgEncrypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
   an encryption module with the help of LogicGate main module, LogicGate.py is needed.
   Note: this encryption method is not safe, anyone with the data of the 2 files will be able to see the information. 
   filename: string, file to write the encrypted code to
   key_file: string, file to keep the key string into
   msg: string, word to encrypt
   """
 
+  if not msg.isascii():
+    raise ValueError(f'message received ({repr(msg)}) is not available in ascii')
   k, f, kOut, fOut = ['']*4
   data = []
   chekK = []
   chekF = []
   for char in msg:
     data.append(str(bin(ord(char))[2:]))
   for i in data:
```

### Comparing `LogicGate-0.2.1/README.rst` & `LogicGate-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `LogicGate-0.2.1/pyproject.toml` & `LogicGate-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LogicGate"
-version = "0.2.1"
+version = "0.2.5"
 description = "an esolang designed for manual encryption with logic gates"
 license = "MIT"
 authors = ["Taokyle <taokyle415@gmail.com>"]
 readme = "README.rst"
 repository = "https://replit.com/@s3D27ZHOU/LogicGate"
 packages = [
     { include = "LogicGate.py", from = "LogicGate" },
```

### Comparing `LogicGate-0.2.1/setup.py` & `LogicGate-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = \
 {'': 'LogicGate'}
 
 modules = \
 ['LogicGate', 'lgEncrypt']
 setup_kwargs = {
     'name': 'logicgate',
-    'version': '0.2.1',
+    'version': '0.2.5',
     'description': 'an esolang designed for manual encryption with logic gates',
     'long_description': 'LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you\ncould make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult and indeed it is.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be lgeso\n\nRunner\n------\n\nTo use it, import the python file **LogicGate.py** in your python\nscript, or just run the LogicGate.py.\nRemember for the run function, only\nthe filename argument is needed. The run function will return an exit\ncode if you use the run function, and outputs of the file will be\nprinted(binary to ascii, and logical binary if enabled). The compile\nfunction does the otherwise, it doesn’t return anything but it can write\ncode into lgeso file.\n\nSpecial encrypt module\n----------------------\na special encrypt module is included in this package, which is lgEncrypt.py. \nit contain two functions, encrypt() and decrypt().\nencrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt()\nencrypth) have 3 arguments, data file name, key file name, message\nThey are very self explainatory\n\ndecrypt() have 3 arguments, data file, key file, sause\nthe first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\neach line as each command For gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically\nbe processed. No linking between words, unless the syntax at the middle\nis invalid\n\nBasic gates(gates that doesn’t require includes):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the\nbinary for ascii translation\n\n### (three hashes): comment everything after the syntax\n\nFor any of the special syntax, they are not being interpreted as special\nsyntax unless the entire syntax appears. They can be anywhere in a line,\nand that line will act like what the syntax shows (if the special syntax\nappears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n\n`gitbub\n<https://github.com/TaokyleYT/LogicGate/>`__\\\n\nEsolang wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\\n\nReplit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n',
     'author': 'Taokyle',
     'author_email': 'taokyle415@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://replit.com/@s3D27ZHOU/LogicGate',
```

### Comparing `LogicGate-0.2.1/PKG-INFO` & `LogicGate-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logicgate
-Version: 0.2.1
+Version: 0.2.5
 Summary: an esolang designed for manual encryption with logic gates
 Home-page: https://replit.com/@s3D27ZHOU/LogicGate
 License: MIT
 Author: Taokyle
 Author-email: taokyle415@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

