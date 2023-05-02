# Comparing `tmp/securepasswordgenerator-1.0.1.tar.gz` & `tmp/securepasswordgenerator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "securepasswordgenerator-1.0.1.tar", last modified: Wed Apr 26 19:12:25 2023, max compression
+gzip compressed data, was "securepasswordgenerator-2.0.0.tar", last modified: Tue May  2 17:59:49 2023, max compression
```

## Comparing `securepasswordgenerator-1.0.1.tar` & `securepasswordgenerator-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 quill     (1000) quill     (1000)        0 2023-04-26 19:12:25.366215 securepasswordgenerator-1.0.1/
--rw-rw-r--   0 quill     (1000) quill     (1000)     1094 2023-04-26 18:27:40.000000 securepasswordgenerator-1.0.1/LICENSE
--rw-rw-r--   0 quill     (1000) quill     (1000)     6697 2023-04-26 19:12:25.366215 securepasswordgenerator-1.0.1/PKG-INFO
--rw-rw-r--   0 quill     (1000) quill     (1000)     5525 2023-04-26 18:58:04.000000 securepasswordgenerator-1.0.1/README.md
-drwxrwxr-x   0 quill     (1000) quill     (1000)        0 2023-04-26 19:12:25.362214 securepasswordgenerator-1.0.1/securepasswordgenerator/
--rw-rw-r--   0 quill     (1000) quill     (1000)      265 2023-04-26 19:00:00.000000 securepasswordgenerator-1.0.1/securepasswordgenerator/__init__.py
--rw-rw-r--   0 quill     (1000) quill     (1000)     9335 2023-04-26 18:59:55.000000 securepasswordgenerator-1.0.1/securepasswordgenerator/securepasswordgenerator.py
-drwxrwxr-x   0 quill     (1000) quill     (1000)        0 2023-04-26 19:12:25.366215 securepasswordgenerator-1.0.1/securepasswordgenerator.egg-info/
--rw-rw-r--   0 quill     (1000) quill     (1000)     6697 2023-04-26 19:12:25.000000 securepasswordgenerator-1.0.1/securepasswordgenerator.egg-info/PKG-INFO
--rw-rw-r--   0 quill     (1000) quill     (1000)      351 2023-04-26 19:12:25.000000 securepasswordgenerator-1.0.1/securepasswordgenerator.egg-info/SOURCES.txt
--rw-rw-r--   0 quill     (1000) quill     (1000)        1 2023-04-26 19:12:25.000000 securepasswordgenerator-1.0.1/securepasswordgenerator.egg-info/dependency_links.txt
--rw-rw-r--   0 quill     (1000) quill     (1000)       97 2023-04-26 19:12:25.000000 securepasswordgenerator-1.0.1/securepasswordgenerator.egg-info/entry_points.txt
--rw-rw-r--   0 quill     (1000) quill     (1000)       24 2023-04-26 19:12:25.000000 securepasswordgenerator-1.0.1/securepasswordgenerator.egg-info/top_level.txt
--rw-rw-r--   0 quill     (1000) quill     (1000)       38 2023-04-26 19:12:25.366215 securepasswordgenerator-1.0.1/setup.cfg
--rw-rw-r--   0 quill     (1000) quill     (1000)     1597 2023-04-26 19:11:45.000000 securepasswordgenerator-1.0.1/setup.py
+drwxrwxr-x   0 quill     (1000) quill     (1000)        0 2023-05-02 17:59:49.919603 securepasswordgenerator-2.0.0/
+-rw-rw-r--   0 quill     (1000) quill     (1000)     1094 2023-04-26 18:27:40.000000 securepasswordgenerator-2.0.0/LICENSE
+-rw-rw-r--   0 quill     (1000) quill     (1000)     8067 2023-05-02 17:59:49.919603 securepasswordgenerator-2.0.0/PKG-INFO
+-rw-rw-r--   0 quill     (1000) quill     (1000)     6844 2023-05-02 17:53:16.000000 securepasswordgenerator-2.0.0/README.md
+drwxrwxr-x   0 quill     (1000) quill     (1000)        0 2023-05-02 17:59:49.891603 securepasswordgenerator-2.0.0/securepasswordgenerator/
+-rw-rw-r--   0 quill     (1000) quill     (1000)      265 2023-04-26 19:00:00.000000 securepasswordgenerator-2.0.0/securepasswordgenerator/__init__.py
+-rw-rw-r--   0 quill     (1000) quill     (1000)     7955 2023-05-02 16:41:28.000000 securepasswordgenerator-2.0.0/securepasswordgenerator/securepasswordgenerator.py
+drwxrwxr-x   0 quill     (1000) quill     (1000)        0 2023-05-02 17:59:49.919603 securepasswordgenerator-2.0.0/securepasswordgenerator.egg-info/
+-rw-rw-r--   0 quill     (1000) quill     (1000)     8067 2023-05-02 17:59:49.000000 securepasswordgenerator-2.0.0/securepasswordgenerator.egg-info/PKG-INFO
+-rw-rw-r--   0 quill     (1000) quill     (1000)      351 2023-05-02 17:59:49.000000 securepasswordgenerator-2.0.0/securepasswordgenerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 quill     (1000) quill     (1000)        1 2023-05-02 17:59:49.000000 securepasswordgenerator-2.0.0/securepasswordgenerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 quill     (1000) quill     (1000)       97 2023-05-02 17:59:49.000000 securepasswordgenerator-2.0.0/securepasswordgenerator.egg-info/entry_points.txt
+-rw-rw-r--   0 quill     (1000) quill     (1000)       24 2023-05-02 17:59:49.000000 securepasswordgenerator-2.0.0/securepasswordgenerator.egg-info/top_level.txt
+-rw-rw-r--   0 quill     (1000) quill     (1000)       38 2023-05-02 17:59:49.919603 securepasswordgenerator-2.0.0/setup.cfg
+-rw-rw-r--   0 quill     (1000) quill     (1000)     1647 2023-05-02 17:53:09.000000 securepasswordgenerator-2.0.0/setup.py
```

### Comparing `securepasswordgenerator-1.0.1/LICENSE` & `securepasswordgenerator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `securepasswordgenerator-1.0.1/PKG-INFO` & `securepasswordgenerator-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: securepasswordgenerator
-Version: 1.0.1
+Version: 2.0.0
 Summary: SecurePasswordGenerator is a tool for generating random passwords. It provides both command line utility and underlying python module.
 Home-page: https://github.com/quillfires/SecurePasswordGenerator
 Author: Ali Fayaz (Quill)
 Author-email: fayaz.quill@gmail.com
 License: MIT
 Keywords: password generator
 Classifier: Programming Language :: Python
@@ -15,145 +15,150 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+This is a tool for generating random secure passwords. It provides both command line utility (CLI) and underlying python module.
+
 # SecurePasswordGenerator
-`SecurePasswordGenerator` is a tool for generating random secure passwords. It provides both command line utility (CLI) and underlying python module.
+[![Python Version](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org)  [![securepasswordgenerator · PyPI](https://img.shields.io/pypi/v/securepasswordgenerator.svg?color=4CBB17)](https://pypi.org/project/securepasswordgenerator/)  [![PyPI - Status](https://img.shields.io/pypi/status/securepasswordgenerator)](https://pypi.org/project/securepasswordgenerator/)  [![Maintenance](https://img.shields.io/maintenance/yes/2030)](https://pypi.org/project/securepasswordgenerator/)  [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/quillfires/SecurePasswordGenerator/blob/main/LICENSE)
+
+[![ViewCount](https://views.whatilearened.today/views/github/quillfires/SecurePasswordGenerator.svg)](https://views.whatilearened.today/views/github/quillfires/SecurePasswordGenerator.svg)  [![GitHub forks](https://img.shields.io/github/forks/quillfires/SecurePasswordGenerator)](https://github.com/quillfires/SecurePasswordGenerator/forks)  [![GitHub stars](https://img.shields.io/github/stars/quillfires/SecurePasswordGenerator.svg?color=ffd40c)](https://github.com/quillfires/SecurePasswordGenerator/stargazers)  [![PyPI - Downloads](https://img.shields.io/pypi/dm/securepasswordgenerator?color=orange&label=PIP%20-%20Installs)](https://pypi.org/project/securepasswordgenerator/) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/quillfires/SecurePasswordGenerator/issues)  [![GitHub issues](https://img.shields.io/github/issues/quillfires/SecurePasswordGenerator.svg?color=808080)](https://github.com/quillfires/SecurePasswordGenerator/issues)  
+
 
 ## Table of Contents
 - [Prerequisites](#prerequisites)
 - [Installation](#installation)
 - [Usage](#usage)
+    - [Python Module](#module)
     - [Command Line Utility](#command-line-utility)
 - [License](#license)
 
+
 ## Prerequisites
 You'll need to have Python installed in order to run `SecurePasswordGenerator`. Start by downloading and installing [Python](https://www.python.org/downloads/).
 > *Note: Python 3 is recommended, however `SecurePasswordGenerator` has been successfully tested with Python 2.6+*
 
 
 ## Installation
+You can install this package from PyPI using pip:
 ```
 python -m pip install securepasswordgenerator
 ```
 
+
 ## Usage
-`SecurePasswordGenerator` provides the following methods:
-```py
-securepasswordgenerator.generate(length = 10, use_lower_case = True, use_upper_case = True, use_numbers = True, use_special = False, use_hex = False)
+### Module
+To use this package in your Python program, simply import the `securepasswordgenerator` module and call the `generate` function with the desired options. Or call predefined functions. Here is an example:
+```python
+from securepasswordgenerator.password import generate
+
+password = generate(length=12, use_lower_case=True, use_upper_case=True, use_numbers=True, use_special=True, use_hex=False)
+```
+This will generate a password that is 12 characters long and includes lowercase letters, uppercase letters, numbers, and special characters.
+
+`securepasswordgenerator` provides the following methods:
+```python
+securepasswordgenerator.generate()
+# defaults to 8 characters long that includes atleast 1 lowercase, 1 uppercase, 1 number and 1 special character.
+securepasswordgenerator.generate(length = 8, use_lower_case = True, use_upper_case = True, use_numbers = True, use_special = True, use_hex = False)
+# optins can be provided to generate as you please.
 securepasswordgenerator.decent() 
+# Generate Memorable Passwords - Perfect for securing your computer or mobile device, or somewhere brute force is detectable.
 securepasswordgenerator.strong() 
+# Generate Strong Passwords - Robust enough to keep your web hosting account secure.
 securepasswordgenerator.fort_knox() 
+# Generate Fort Knox Passwords - Secure enough for almost anything, like root or administrator passwords.
 securepasswordgenerator.ci_key() 
+# Generate CodeIgniter Encryption Keys - Can be used for any other 256-bit key requirement.
 securepasswordgenerator.wep_64() 
+# Generate 64-bit WEP Keys
 securepasswordgenerator.wep_128() 
+# Generate 128-bit WEP Keys
 securepasswordgenerator.wep_152() 
+# Generate 152-bit WEP Keys
 securepasswordgenerator.wep_256() 
+# Generate 256-bit WEP Keys
 securepasswordgenerator.wpa_160() 
+# Generate 160-bit WPA Key
 securepasswordgenerator.wpa_504()
+# Generate 504-bit WPA Key
 ```
 
 Sample code:
-```py
->>> import securepasswordgenerator
->>> securepasswordgenerator.generate()
-'ZgnoiVCQ'
->>> securepasswordgenerator.generate(15, use_lower_case=False, use_numbers=False, use_special=True)
+```python
+>>> import securepasswordgenerator as spw
+>>> spw.generate()
+'ZgnoiV*Q'
+>>> spw.generate(15, use_lower_case=False, use_numbers=False, use_special=True)
 '<)G,{IH~NDGZ+D@'
->>> securepasswordgenerator.decent() 
+>>> spw.decent() 
 'CONt8xy4Vw'
->>> securepasswordgenerator.strong() 
+>>> spw.strong() 
 'm?c$t?WP<y|}vVf'
->>> securepasswordgenerator.fort_knox() 
+>>> spw.fort_knox() 
 "'>[&;6L8?->vXiKWh>Uoe<Uo-.x,Zb"
->>> securepasswordgenerator.ci_key() 
+>>> spw.ci_key() 
 'I9MMEnszZO4mKGJayBXe9kKsEGg7JXBs'
->>> securepasswordgenerator.wep_64() 
+>>> spw.wep_64() 
 '866EE'
->>> securepasswordgenerator.wep_128() 
+>>> spw.wep_128() 
 '9EBD3954549FC'
->>> securepasswordgenerator.wep_152() 
+>>> spw.wep_152() 
 'D5CB8A9668F2153D'
->>> securepasswordgenerator.wep_256() 
+>>> spw.wep_256() 
 'E775C1FA7D96CF94DFB19CB9ED534'
->>> securepasswordgenerator.wpa_160() 
+>>> spw.wpa_160() 
 '1XkW\\eHu5,ox9I&K`I<R'
->>> securepasswordgenerator.wpa_504()
+>>> spw.wpa_504()
 "AkW~Z9/)d2rf`JWPU}CcUq*`BTsq8%'i+,~BAp2nf@*t!W&~rlpxq(Grh6>$1rj"
 ```
 
 ### Command Line Utility
-`SecurePasswordGenerator` includes a command line utility for generating passwords.
+To generate a password from the command line, simply run the `securepasswordgenerator` command and specify the desired options. Here are a few examples:
+
 ```
-securepasswordgenerator --help
-usage: securepasswordgenerator.py [-h] [-l] [-L] [-u] [-U] [-n] [-N] [-s] [-S] [-x] [-X] [-DP] [-SP] [-FP] [-ci] [-wpa160] [-wpa504]
-                         [-wep64] [-wep128] [-wep152] [-wep256]
-                         [length]
+securepasswordgenerator
+```
+This will generate a password that is 8 characters long that includes atleast 1 lowercase, 1 uppercase, 1 number and 1 special character.
 
-The Secure Password or Keygen Generator
+```
+securepasswordgenerator 11 -l -n -s -x -p
+```
+This will generate a password that is 15 characters long and includes lowercase letters, numbers, special characters, and hex characters.
+
+Here are the available options:
+```
+usage: securepasswordgenerator [-h] [-l] [-u] [-n] [-s] [-x] [-p {decent,strong,fort_knox,wpa_160,wpa_504,wep_64,wep_128,wep_152,wep_256}] [length]
 
 positional arguments:
   length                Length of password (default is 8 characters)
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
-  -l, --lower-enable    Use lowercase characters
-  -L, --lower-disable   Don't use lowercase characters
-  -u, --upper-enable    use upper case characters
-  -U, --upper-disable   don't use upper case characters
-  -n, --number-enable   use number characters
-  -N, --number-disable  don't use number characters
-  -s, --special-enable  use special characters
-  -S, --special-disable
-                        don't use special characters
-  -x, --hex-enable      use hex characters
-  -X, --hex-disable     don't use hex characters
-  -DP, --decent         Generate Memorable Passwords - Perfect for securing your computer or mobile device, or somewhere brute
-                        force is detectable.
-  -SP, --strong         Generate Strong Passwords - Robust enough to keep your web hosting account secure.
-  -FP, --fort_knox      Generate Fort Knox Passwords - Secure enough for almost anything, like root or administrator passwords.
-  -ci, --ci_key         Generate CodeIgniter Encryption Keys - Can be used for any other 256-bit key requirement.
-  -wpa160, --wpa_160    Generate 160-bit WPA Key
-  -wpa504, --wpa_504    Generate 504-bit WPA Key
-  -wep64, --wep_64      Generate 64-bit WEP Keys
-  -wep128, --wep_128    Generate 128-bit WEP Keys
-  -wep152, --wep_152    Generate 152-bit WEP Keys
-  -wep256, --wep_256    Generate 256-bit WEP Keys
+  -l, --lower-case      Use lowercase characters
+  -u, --upper-case      Use uppercase characters
+  -n, --numbers         Use numbers
+  -s, --special         Use special characters
+  -x, --hex             Use hex characters
+  -p {decent,strong,fort_knox,wpa_160,wpa_504,wep_64,wep_128,wep_152,wep_256}, --password-strength {decent,strong,fort_knox,wpa_160,wpa_504,wep_64,wep_128,wep_152,wep_256}
+                        Generate a password with a predefined strength
 ```
-> *Note: `-DP`, `--decent`, `-SP`, `--strong`, `-FP`, `--fort_knox`, `-ci`, `--ci_key`, `-wpa160`, `--wpa_160`, `-wpa504`, `--wpa_504`, `-wep64`, `--wep_64`, `-wep128`, `--wep_128`, `-wep152`, `--wep_152`, `-wep256`, `--wep_256` doesn't require any other arguments*
+> *Note: `securepasswordgenerator -p [option]` or `securepasswordgenerator --password-strength [option]` doesn't require any other arguments*
 
 
-## License
+# Changlog
+[See the change log here](https://github.com/quillfires/SecurePasswordGenerator/blob/main/CHANGELOG.md)
 
-This project is licensed under the MIT License
-```
-MIT License
 
-Copyright (c) 2023-present Ali Fayaz (Quill) (quillfires)
+## License
 
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
-```
+This package is licensed under the MIT License. See the [LICENSE](https://github.com/quillfires/SecurePasswordGenerator/blob/main/LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `securepasswordgenerator-1.0.1/securepasswordgenerator.egg-info/PKG-INFO` & `securepasswordgenerator-2.0.0/securepasswordgenerator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: securepasswordgenerator
-Version: 1.0.1
+Version: 2.0.0
 Summary: SecurePasswordGenerator is a tool for generating random passwords. It provides both command line utility and underlying python module.
 Home-page: https://github.com/quillfires/SecurePasswordGenerator
 Author: Ali Fayaz (Quill)
 Author-email: fayaz.quill@gmail.com
 License: MIT
 Keywords: password generator
 Classifier: Programming Language :: Python
@@ -15,145 +15,150 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+This is a tool for generating random secure passwords. It provides both command line utility (CLI) and underlying python module.
+
 # SecurePasswordGenerator
-`SecurePasswordGenerator` is a tool for generating random secure passwords. It provides both command line utility (CLI) and underlying python module.
+[![Python Version](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org)  [![securepasswordgenerator · PyPI](https://img.shields.io/pypi/v/securepasswordgenerator.svg?color=4CBB17)](https://pypi.org/project/securepasswordgenerator/)  [![PyPI - Status](https://img.shields.io/pypi/status/securepasswordgenerator)](https://pypi.org/project/securepasswordgenerator/)  [![Maintenance](https://img.shields.io/maintenance/yes/2030)](https://pypi.org/project/securepasswordgenerator/)  [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/quillfires/SecurePasswordGenerator/blob/main/LICENSE)
+
+[![ViewCount](https://views.whatilearened.today/views/github/quillfires/SecurePasswordGenerator.svg)](https://views.whatilearened.today/views/github/quillfires/SecurePasswordGenerator.svg)  [![GitHub forks](https://img.shields.io/github/forks/quillfires/SecurePasswordGenerator)](https://github.com/quillfires/SecurePasswordGenerator/forks)  [![GitHub stars](https://img.shields.io/github/stars/quillfires/SecurePasswordGenerator.svg?color=ffd40c)](https://github.com/quillfires/SecurePasswordGenerator/stargazers)  [![PyPI - Downloads](https://img.shields.io/pypi/dm/securepasswordgenerator?color=orange&label=PIP%20-%20Installs)](https://pypi.org/project/securepasswordgenerator/) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/quillfires/SecurePasswordGenerator/issues)  [![GitHub issues](https://img.shields.io/github/issues/quillfires/SecurePasswordGenerator.svg?color=808080)](https://github.com/quillfires/SecurePasswordGenerator/issues)  
+
 
 ## Table of Contents
 - [Prerequisites](#prerequisites)
 - [Installation](#installation)
 - [Usage](#usage)
+    - [Python Module](#module)
     - [Command Line Utility](#command-line-utility)
 - [License](#license)
 
+
 ## Prerequisites
 You'll need to have Python installed in order to run `SecurePasswordGenerator`. Start by downloading and installing [Python](https://www.python.org/downloads/).
 > *Note: Python 3 is recommended, however `SecurePasswordGenerator` has been successfully tested with Python 2.6+*
 
 
 ## Installation
+You can install this package from PyPI using pip:
 ```
 python -m pip install securepasswordgenerator
 ```
 
+
 ## Usage
-`SecurePasswordGenerator` provides the following methods:
-```py
-securepasswordgenerator.generate(length = 10, use_lower_case = True, use_upper_case = True, use_numbers = True, use_special = False, use_hex = False)
+### Module
+To use this package in your Python program, simply import the `securepasswordgenerator` module and call the `generate` function with the desired options. Or call predefined functions. Here is an example:
+```python
+from securepasswordgenerator.password import generate
+
+password = generate(length=12, use_lower_case=True, use_upper_case=True, use_numbers=True, use_special=True, use_hex=False)
+```
+This will generate a password that is 12 characters long and includes lowercase letters, uppercase letters, numbers, and special characters.
+
+`securepasswordgenerator` provides the following methods:
+```python
+securepasswordgenerator.generate()
+# defaults to 8 characters long that includes atleast 1 lowercase, 1 uppercase, 1 number and 1 special character.
+securepasswordgenerator.generate(length = 8, use_lower_case = True, use_upper_case = True, use_numbers = True, use_special = True, use_hex = False)
+# optins can be provided to generate as you please.
 securepasswordgenerator.decent() 
+# Generate Memorable Passwords - Perfect for securing your computer or mobile device, or somewhere brute force is detectable.
 securepasswordgenerator.strong() 
+# Generate Strong Passwords - Robust enough to keep your web hosting account secure.
 securepasswordgenerator.fort_knox() 
+# Generate Fort Knox Passwords - Secure enough for almost anything, like root or administrator passwords.
 securepasswordgenerator.ci_key() 
+# Generate CodeIgniter Encryption Keys - Can be used for any other 256-bit key requirement.
 securepasswordgenerator.wep_64() 
+# Generate 64-bit WEP Keys
 securepasswordgenerator.wep_128() 
+# Generate 128-bit WEP Keys
 securepasswordgenerator.wep_152() 
+# Generate 152-bit WEP Keys
 securepasswordgenerator.wep_256() 
+# Generate 256-bit WEP Keys
 securepasswordgenerator.wpa_160() 
+# Generate 160-bit WPA Key
 securepasswordgenerator.wpa_504()
+# Generate 504-bit WPA Key
 ```
 
 Sample code:
-```py
->>> import securepasswordgenerator
->>> securepasswordgenerator.generate()
-'ZgnoiVCQ'
->>> securepasswordgenerator.generate(15, use_lower_case=False, use_numbers=False, use_special=True)
+```python
+>>> import securepasswordgenerator as spw
+>>> spw.generate()
+'ZgnoiV*Q'
+>>> spw.generate(15, use_lower_case=False, use_numbers=False, use_special=True)
 '<)G,{IH~NDGZ+D@'
->>> securepasswordgenerator.decent() 
+>>> spw.decent() 
 'CONt8xy4Vw'
->>> securepasswordgenerator.strong() 
+>>> spw.strong() 
 'm?c$t?WP<y|}vVf'
->>> securepasswordgenerator.fort_knox() 
+>>> spw.fort_knox() 
 "'>[&;6L8?->vXiKWh>Uoe<Uo-.x,Zb"
->>> securepasswordgenerator.ci_key() 
+>>> spw.ci_key() 
 'I9MMEnszZO4mKGJayBXe9kKsEGg7JXBs'
->>> securepasswordgenerator.wep_64() 
+>>> spw.wep_64() 
 '866EE'
->>> securepasswordgenerator.wep_128() 
+>>> spw.wep_128() 
 '9EBD3954549FC'
->>> securepasswordgenerator.wep_152() 
+>>> spw.wep_152() 
 'D5CB8A9668F2153D'
->>> securepasswordgenerator.wep_256() 
+>>> spw.wep_256() 
 'E775C1FA7D96CF94DFB19CB9ED534'
->>> securepasswordgenerator.wpa_160() 
+>>> spw.wpa_160() 
 '1XkW\\eHu5,ox9I&K`I<R'
->>> securepasswordgenerator.wpa_504()
+>>> spw.wpa_504()
 "AkW~Z9/)d2rf`JWPU}CcUq*`BTsq8%'i+,~BAp2nf@*t!W&~rlpxq(Grh6>$1rj"
 ```
 
 ### Command Line Utility
-`SecurePasswordGenerator` includes a command line utility for generating passwords.
+To generate a password from the command line, simply run the `securepasswordgenerator` command and specify the desired options. Here are a few examples:
+
 ```
-securepasswordgenerator --help
-usage: securepasswordgenerator.py [-h] [-l] [-L] [-u] [-U] [-n] [-N] [-s] [-S] [-x] [-X] [-DP] [-SP] [-FP] [-ci] [-wpa160] [-wpa504]
-                         [-wep64] [-wep128] [-wep152] [-wep256]
-                         [length]
+securepasswordgenerator
+```
+This will generate a password that is 8 characters long that includes atleast 1 lowercase, 1 uppercase, 1 number and 1 special character.
 
-The Secure Password or Keygen Generator
+```
+securepasswordgenerator 11 -l -n -s -x -p
+```
+This will generate a password that is 15 characters long and includes lowercase letters, numbers, special characters, and hex characters.
+
+Here are the available options:
+```
+usage: securepasswordgenerator [-h] [-l] [-u] [-n] [-s] [-x] [-p {decent,strong,fort_knox,wpa_160,wpa_504,wep_64,wep_128,wep_152,wep_256}] [length]
 
 positional arguments:
   length                Length of password (default is 8 characters)
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
-  -l, --lower-enable    Use lowercase characters
-  -L, --lower-disable   Don't use lowercase characters
-  -u, --upper-enable    use upper case characters
-  -U, --upper-disable   don't use upper case characters
-  -n, --number-enable   use number characters
-  -N, --number-disable  don't use number characters
-  -s, --special-enable  use special characters
-  -S, --special-disable
-                        don't use special characters
-  -x, --hex-enable      use hex characters
-  -X, --hex-disable     don't use hex characters
-  -DP, --decent         Generate Memorable Passwords - Perfect for securing your computer or mobile device, or somewhere brute
-                        force is detectable.
-  -SP, --strong         Generate Strong Passwords - Robust enough to keep your web hosting account secure.
-  -FP, --fort_knox      Generate Fort Knox Passwords - Secure enough for almost anything, like root or administrator passwords.
-  -ci, --ci_key         Generate CodeIgniter Encryption Keys - Can be used for any other 256-bit key requirement.
-  -wpa160, --wpa_160    Generate 160-bit WPA Key
-  -wpa504, --wpa_504    Generate 504-bit WPA Key
-  -wep64, --wep_64      Generate 64-bit WEP Keys
-  -wep128, --wep_128    Generate 128-bit WEP Keys
-  -wep152, --wep_152    Generate 152-bit WEP Keys
-  -wep256, --wep_256    Generate 256-bit WEP Keys
+  -l, --lower-case      Use lowercase characters
+  -u, --upper-case      Use uppercase characters
+  -n, --numbers         Use numbers
+  -s, --special         Use special characters
+  -x, --hex             Use hex characters
+  -p {decent,strong,fort_knox,wpa_160,wpa_504,wep_64,wep_128,wep_152,wep_256}, --password-strength {decent,strong,fort_knox,wpa_160,wpa_504,wep_64,wep_128,wep_152,wep_256}
+                        Generate a password with a predefined strength
 ```
-> *Note: `-DP`, `--decent`, `-SP`, `--strong`, `-FP`, `--fort_knox`, `-ci`, `--ci_key`, `-wpa160`, `--wpa_160`, `-wpa504`, `--wpa_504`, `-wep64`, `--wep_64`, `-wep128`, `--wep_128`, `-wep152`, `--wep_152`, `-wep256`, `--wep_256` doesn't require any other arguments*
+> *Note: `securepasswordgenerator -p [option]` or `securepasswordgenerator --password-strength [option]` doesn't require any other arguments*
 
 
-## License
+# Changlog
+[See the change log here](https://github.com/quillfires/SecurePasswordGenerator/blob/main/CHANGELOG.md)
 
-This project is licensed under the MIT License
-```
-MIT License
 
-Copyright (c) 2023-present Ali Fayaz (Quill) (quillfires)
+## License
 
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
-```
+This package is licensed under the MIT License. See the [LICENSE](https://github.com/quillfires/SecurePasswordGenerator/blob/main/LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `securepasswordgenerator-1.0.1/setup.py` & `securepasswordgenerator-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "securepasswordgenerator",
-    version = "1.0.1",
+    version = "2.0.0",
     author = "Ali Fayaz (Quill)",
     author_email = "fayaz.quill@gmail.com",
     description = ("SecurePasswordGenerator is a tool for generating random passwords. It provides both command line utility and underlying python module."),
     license = "MIT",
     keywords = "password generator",
     url = "https://github.com/quillfires/SecurePasswordGenerator",
     packages=["securepasswordgenerator"],
@@ -26,14 +26,15 @@
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 5 - Production/Stable"
     ],
     entry_points = {
         'console_scripts': ['securepasswordgenerator=securepasswordgenerator.securepasswordgenerator:main'],
     }
```

