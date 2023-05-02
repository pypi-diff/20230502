# Comparing `tmp/DeltacodeProject-0.7.31.0.tar.gz` & `tmp/DeltacodeProject-0.7.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeltacodeProject-0.7.31.0.tar", last modified: Tue Mar 14 23:41:43 2023, max compression
+gzip compressed data, was "DeltacodeProject-0.7.31.1.tar", last modified: Tue May  2 09:08:28 2023, max compression
```

## Comparing `DeltacodeProject-0.7.31.0.tar` & `DeltacodeProject-0.7.31.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:41:43.276866 DeltacodeProject-0.7.31.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:41:43.272865 DeltacodeProject-0.7.31.0/DeltacodeProject/
--rw-r--r--   0 runner    (1001) docker     (123)    32749 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/Deltacode.py
--rw-r--r--   0 runner    (1001) docker     (123)    26893 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/DeltacodeNew.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/encodings2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/encodings2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/new_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/DeltacodeProject/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:41:43.276866 DeltacodeProject-0.7.31.0/DeltacodeProject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-03-14 23:41:43.000000 DeltacodeProject-0.7.31.0/DeltacodeProject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-14 23:41:43.000000 DeltacodeProject-0.7.31.0/DeltacodeProject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 23:41:43.000000 DeltacodeProject-0.7.31.0/DeltacodeProject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 23:41:43.000000 DeltacodeProject-0.7.31.0/DeltacodeProject.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-03-14 23:41:43.276866 DeltacodeProject-0.7.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 23:41:43.276866 DeltacodeProject-0.7.31.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 23:41:43.276866 DeltacodeProject-0.7.31.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-14 23:41:31.000000 DeltacodeProject-0.7.31.0/test/test_DAY_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:28.373933 DeltacodeProject-0.7.31.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:28.373933 DeltacodeProject-0.7.31.1/DeltacodeProject/
+-rw-r--r--   0 runner    (1001) docker     (123)    32769 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/Deltacode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27285 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/DeltacodeNew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23083 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/encodings2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/encodings3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/new_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/DeltacodeProject/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:28.373933 DeltacodeProject-0.7.31.1/DeltacodeProject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-05-02 09:08:28.000000 DeltacodeProject-0.7.31.1/DeltacodeProject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-02 09:08:28.000000 DeltacodeProject-0.7.31.1/DeltacodeProject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:08:28.000000 DeltacodeProject-0.7.31.1/DeltacodeProject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 09:08:28.000000 DeltacodeProject-0.7.31.1/DeltacodeProject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-05-02 09:08:28.373933 DeltacodeProject-0.7.31.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:08:28.373933 DeltacodeProject-0.7.31.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:08:28.373933 DeltacodeProject-0.7.31.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-02 09:08:15.000000 DeltacodeProject-0.7.31.1/test/test_DAY_time.py
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/Deltacode.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/Deltacode.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         self.status = "in __init__"
         self.center_y = int(chercher(str(shutil.get_terminal_size()), "columns=", ",").replace("columns=", '').replace(",", ''))
         self.banner = ' \\\ DELTACODE // '
         self.password_running = "None"
         self.text_running = "None"
         self.shift_running = 0
         if os.path.exists("historique.txt"):
-            with open("historique.txt", 'r') as f: self.history = f.read()
+            with open("historique.txt", 'r', encoding='UTF-8') as f: self.history = f.read()
         else: self.history = "\n"
         if os.name == "posix": self.OS = "LINUX"
         elif os.name == "nt": self.OS = "WINDOWS"
 
     def copy(self, txt):
         if self.use_copy is True:
             if os.name == "posix":
@@ -471,15 +471,15 @@
         self.text_running = coding
         self.password_running = Password
         return input_return()
 
     def create_menu(self, tab: int, lst: list, encadr="│", centery: int = None):
         if not centery:
             centery = self.center_y
-        print(centery)
+        # print(centery)
         menu_tab = "\t" * tab + encadr
         end = encadr
         menu = """"""
         len_max = 0
         number = 0
         before = 4
         for i in lst:
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/DeltacodeNew.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/DeltacodeNew.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 import sys
 import shutil
 from DeltacodeProject.encodings2 import *
 from DeltacodeProject import __version__
 from DeltacodeProject import *
 from time import sleep
 import string as s
-
-
+import subprocess
+import signal
 
 class Deltacode:
     """                                                 \\\ DELTA-ENCODING //
     To decode or encode a text/string with rotation using all the existing characters.
     Pour encoder ou décoder un texte ou une chaîne de caractères avec une rotation utilisant tous les caractères existants.
 
     """
 
     def __init__(self, *args):
-        print(args[0])
+        # print(args[0])
         self.encodings = {}
         self.class_encodings = []
         for class_ in args[0]:
-            print(class_)
+            # print(class_)
             self.class_encodings.append(class_)
             self.encodings[class_.__name__] = {}
             new_dict = self.encodings[class_.__name__]
             new_dict["name"] = class_.__name__
             new_dict["functions"] = [func for func in dir(class_) if not func.startswith("__") and not func.endswith("__")]
             new_dict["__init__"] = class_.__init__.__code__.co_varnames[1:]
             if "description" in new_dict["__init__"]:
                 new_dict["description"] = new_dict["__init__"]["description"]
             if "abbr" in new_dict["__init__"]:
                 new_dict["description"] = new_dict["__init__"]["abbr"]
-        print(self.encodings)
-        print(self.class_encodings)
+        # print(self.encodings)
+        # print(self.class_encodings)
         for class_ in self.class_encodings:
             self.create_class_func(class_.__name__, class_)
         self.use_copy = True
         self.valid_char = s.printable
         self.status = "in __init__"
         self.center_y = int(
             chercher(str(shutil.get_terminal_size()), "columns=", ",", replace=True))
@@ -117,72 +117,77 @@
         if get_file_ex(filename) in bytes_ext:
             return bytearray(open(filename, 'rb').read())
         else:
             return open(filename, 'r').read()
 
 
     def input_coding(self, coding_class, decode_encode: str, shift=False, password=True, warning="None",
-                     from_file=False, hexa=False):
+                     from_file=False, hexa=False, byte=False):
         self.status = decode_encode
-        byte = False
         self.clear()
-        self.hexa = input("Voulez-vous utiliser l'encodage hexadecimal ? ")
-        if self.hexa.lower() in ["o", "y", "yes", "oui"]:
-            self.hexa = True
-        else:
-            self.hexa = False
+        if hexa:
+            self.hexa = input("Voulez-vous utiliser l'encodage hexadecimal ? ")
+            if self.hexa.lower() in ["o", "y", "yes", "oui"]:
+                self.hexa = True
+            else:
+                self.hexa = False
 
         def ifif(opt):
+            if password:
+                opt = opt(password=Password)
+            else:
+                opt = opt(rot=Password)
             if hexa:
                 opt.hexa = self.hexa
+            if shift:
+                opt.shift = Shift
             if byte:
                 opt.byte_array = coding.byte_array
                 opt.string = coding.string
             return opt
 
         def coding_option():
             print(hexa)
             kwargs = {}
             if hexa:
                 kwargs["hexa"] = self.hexa
             if shift:
                 kwargs["shift"] = Shift
-            if Password:
+            if password:
                 kwargs["password"] = Password
             else:
                 kwargs["rot"] = Password
-            # print(byte, isinstance(Text, bytearray))
+            print(byte, isinstance(Text, bytearray))
             if byte:
                 if self.status == "encode":
                     coding = coding_class(**kwargs).encode_byte(Text)
                 else:
                     coding = coding_class(**kwargs).decode_byte(Text)
                 self.add_history(Password, Text, coding.byte_array, decode_encode, shift=str(Shift))
             else:
-                kwargs["string"] = Text
                 if self.status == "encode":
-                    coding = coding_class(**kwargs).encode()
+                    coding = coding_class(**kwargs).encode(Text)
                 else:
-                    coding = coding_class(**kwargs).decode()
+                    coding = coding_class(**kwargs).decode(Text)
                 self.add_history(Password, Text, coding.string, decode_encode, shift=str(Shift))
             return coding
 
         def input_return():
             if shift:
                 if from_file:
-                    return [Text, ifif(coding_class(password=Password, string=coding.string, shift=Shift)), self.filename]
-                return [Text, ifif(coding_class(password=Password, string=coding.string, shift=Shift))]
+                    return [Text, coding, self.filename]
+                return [Text, coding]
             elif password is False:
                 if from_file:
-                    return [Text, ifif(coding_class(rot=Password, string=coding.string, shift=Shift)), self.filename]
-                return [Text, ifif(coding_class(rot=Password, string=coding.string, shift=Shift))]
+                    return [Text, coding, self.filename]
+                return [Text, coding]
             else:
                 if from_file:
-                    return [Text, ifif(coding_class(password=Password, string=coding.string)), self.filename]
-                return [Text, ifif(coding_class(password=Password, string=coding.string))]
+                    return [Text, coding, self.filename]
+                return [Text, coding]
 
         def get_rot():
             while True:
                 rot = input("Nombre de rotation à effectuer : ")
                 try:
                     int(rot)
                 except:
@@ -218,14 +223,16 @@
                 return Text
             else:
                 self.copy(str(self.text_running))
                 from_file = False
                 Text = input('Texte : ')
                 self.text_running = Text
         if from_file:
+            if get_file_ex(self.filename) in bytes_ext and byte is False:
+                return [False]
             byte = True if isinstance(Text, bytearray) else False
         if shift:
             Shift = input("Utiliser le shift ? ")
             if Shift.lower() == "oui":
                 while True:
                     self.copy(str(self.shift_running))
                     Shift = input('Shift : ')
@@ -243,14 +250,15 @@
                 return input_return()
             else:
                 Shift = 0
                 coding = coding_option()
                 self.shift_running = Shift
                 return input_return()
         else:
+            Shift = "None"
             coding = coding_option()
             print_color(coding.string, color='blue')
         self.text_running = coding.string
         self.password_running = Password
         return input_return()
 
     def create_menu(self, tab: int, lst: list):
@@ -295,15 +303,16 @@
         return menu
 
 
 class main(Deltacode):
 
     def __init__(self, *args, copy=None):
         super().__init__(args)
-        sys.tracebacklimit = 0
+        # sys.tracebacklimit = 0
+        signal.signal(signal.SIGINT, signal_handler)
 
         if copy is None:
             self.use_copy = input(
                 "Voulez-vous utiliser la fonction copier ? Elle vous aidera à copier vos mots de passe, et texte déjà encodés directement quand vous en aurez besoin.\n")
             if self.use_copy.lower() == "oui":
                 self.use_copy = True
             else:
@@ -422,15 +431,15 @@
                         coding = info[1].decode_byte()
                         print_color(coding, color="blue")
                         self.add_history(Password=info[1].password, Text=info[1], coding=coding.byte_array,
                                          decode_encode=self.status, shift=coding.shift if shift else "None")
                         break
                 coding = info[1].decode()
                 print_color(coding, color="blue")
-                self.add_history(Password=info[1].password, Text=info[1], coding=coding.string, decode_encode=self.status, shift=coding.shift if shift else "None")
+                self.add_history(Password=info[1].password if password else info[1].rot, Text=info[1], coding=coding.string, decode_encode=self.status, shift=coding.shift if shift else "None")
                 break
             elif choice_code == "4":
                 print("Développement en cours...")
                 continue
         if choice_code not in [str(i) for i in range(1, len(self.class_encodings) + 1)]:
             print_color('Invalid choice', color='red', effect='bold')
 
@@ -472,15 +481,18 @@
                         hexa = True if "hexa" in self.encodings[name]["__init__"] else False
                         # print("hexa", hexa)
                         byte = True if "byte_array" in self.encodings[name]["__init__"] else False
                         # print("byte", byte)
                         warning = encoding.warning if "warning" in self.encodings[name]["__init__"] else None
                         # print("warning", warning)
                         info = self.input_coding(encoding, decode_encode=self.status, password=password, shift=shift, hexa=hexa,
-                                          warning=warning, from_file=True).copy()
+                                          warning=warning, from_file=True, byte=byte).copy()
+                        if info[0] is False:
+                            print_color('Vous ne pouvez pas choisir cet encodage pour ce fichier', color='red', effect='bold')
+                            break
                         update = info[1]
                         filename = info[-1]
                         if byte:
                             replace_file(filename, update.byte_array)
                         else:
                             replace_file(filename, update.string)
 
@@ -528,21 +540,21 @@
             with open('historique.txt', 'w') as f:
                 f.write("deleted")
             self.save_history()
         self.clear()
         print_color("La sauvegarde de l'historique a été supprimé", effect="italic")
 
     def restart(self):
-        try:
-            os.execl(__file__, *sys.argv)
-            exit(0)
-        except:
-            print_color("Cette fonction n'est actuellement pas fonctionnel sur votre appareil", color="red",
-                        effect="bold")
-            sleep(1.5)
+        command = [sys.executable] + sys.argv
+        for arg in command:
+            if "DeltacodeProject\\__main__.py" in arg:
+                command = command + ["-new"]
+        # print(command)
+        subprocess.Popen(command)
+        sys.exit(88)
 
     def test(self):
         choice_code = input(self.create_menu(2, list(self.encodings.keys())))
 
         for encoding in self.class_encodings:
             name = encoding.__name__
             index = str(self.class_encodings.index(encoding) + 1)
@@ -563,14 +575,15 @@
                 break
             elif choice_code == "4":
                 print("Développement en cours...")
         if choice_code not in [str(i) for i in range(1, len(self.class_encodings) + 1)]:
             print_color('Invalid choice', color='red', effect='bold')
 
     def run(self):
+        wait = 0.5
         while True:
             self.banner = f' \\\ DELTACODE {__version__}// '
             self.clear()
             choice = input(self.create_menu(2, ["Encoder",
                                                 "Décoder",
                                                 "Encoder et Décoder",
                                                 "Encoder ou decoder un fichier",
@@ -594,20 +607,23 @@
             elif choice == "5":
                 self.clear_history()
             elif choice == "6":
                 self.save_history()
             elif choice == "7":
                 self.del_save()
             elif choice == "8":
+                wait = 0
                 self.restart()
             elif choice == "9":
                 self.test()
             elif choice == "8275":
                 print(deltacorp.decode())
                 sleep(10.25)
                 playterm().show()
                 exit(0)
-            sleep(0.5)
-
+            sleep(wait)
 
 if __name__ == '__main__' or "debug" in sys.argv:
+    signal.signal(signal.SIGINT, signal_handler)
     main(Cesar, ROT, DayEncoding, copy=True).run()
+
+
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/__init__.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # __init__.py
 """
 Encoder et décoder du texte/bytes
 """
-from .things.more import playterm
 from DeltacodeProject.encodings2 import DayEncoding
 
 __title__ = "DeltacodeProject"
-__version__ = "0.7.31.0"
+__version__ = "0.7.31.1"
 
 
 
 
 
 
 
@@ -270,8 +269,8 @@
 
 
 
 
 
 
 
-deltacorp = DayEncoding(password="thank you", shift=1111, hexa=False, string="ԘԤԪԨԫҗԲԫԭՀԢԧԺԲҗԴӭԭՁԮԡԷӢӣՅӦԯ԰ӟԛԴԦӜӰԵՁӫԴԬԮԮӠՃ֯ӬԸԮԦӥԲөԿԭԾԬԬԥԪӮҗԳӭԱԾԳӘԲԱӥӰԶԾ԰ԬԡԪԴҗԷԸԭԹԣӘԵԴӦԺԫՀӷӟԢӬԣӠӰԶՁӫԣ֡ԨԱӬՆԸԵԽӟԤӬԫӥԶԵԾԸԠԬԮԳӬԵӦԱԿӟԥԪӢӝԿԸԹ԰ԱӘ֥ӢӧՉԺԴԺԭӘԪԶҗՀԻԵԾӟԙԺӢӣԱԴԳԬԦԝԸӢӛԵӦԼԽԮԟԷԣӤԽԧՀԴԮԦԸӢӜԾӦԳִԭ֡ԷԣӣӾӦԖ԰ӟԫԺԫӪӰԮԱՀԱԝԺԺҗԴԫӬԯԨԪԪӢӨՅԫӬԮԤӘԵԴӦԺԫՀӫԠԪԷԫӭԵӦԮԴԤԦԹֶӫӰ֦ӬԾԮԦӥԶӜՂԳԱӹӟӘӥӯҤӰԃԉԉӟԓԩԣӠՃԹԱՀԱӛӼӹҬԅԣӬԇӼӵ")
+deltacorp = DayEncoding(password="thank you", shift=1111, hexa=False, string="ԘԤԪԨԫҗԲԫԭՀԢԧԺԲҗԴӭԭՁԮԡԷӢӣՅӦԯ԰ӟԛԴԦӜӰԵՁӫԴԬԮԮӠՃ֯ӬԸԮԦӥԲөԿԭԾԬԬԥԪӮҗԳӭԱԾԳӘԲԱӥӰԶԾ԰ԬԡԪԴҗԷԸԭԹԣӘԵԴӦԺԫՀӷӟԢӬԣӠӰԶՁӫԣ֡ԨԱӬՆԸԵԽӟԤӬԫӥԶԵԾԸԠԬԮԳӬԵӦԱԿӟԥԪӢӝԿԸԹ԰ԱӘ֥ӢӧՉԺԴԺԭӘԪԶҗՀԻԵԾӟԙԺӢӣԱԴԳԬԦԝԸӢӛԵӦԼԽԮԟԷԣӤԽԧՀԴԮԦԸӢӜԾӦԳִԭ֡ԷԣӣӾӦԖ԰ӟԫԺԫӪӰԮԱՀԱԝԺԺҗԴԫӬԯԨԪԪӢӨՅԫӬԮԤӘԵԴӦԺԫՀӫԠԪԷԫӭԵӦԮԴԤԦԹֶӫӰ֦ӬԾԮԦӥԶӜՂԳԱӹӟӘӥӯҤӰԃԉԉӟԓԩԣӠՃԹԱՀԱӛӼӹҬԅԣӬԇӼӵ")
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/decode.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/decode.py`

 * *Files identical despite different names*

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/encode.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/encode.py`

 * *Files identical despite different names*

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/encodings.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/encodings.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
             return "ERREUR: La rotation ne doit pas dépasser 26"
 
         result = str()
         for i in range(len(self.string)):
             char = no_accent_char(char=self.string[i])
             try:
                 if char in self.lower:
-                    result += self.lower[self.lower.index(char) + self.rot % 26]
+                    result += self.lower[(self.lower.index(char) + self.rot) % 26]
                 elif char in self.upper:
-                    result += self.upper[self.upper.index(char) + self.rot % 26]
+                    result += self.upper[(self.upper.index(char) + self.rot) % 26]
                 else:
                     result += char
             except:
                 if char in self.lower:
                     result += f"[ERROR string:'{self.lower.index(char)}', rot:'{self.rot}']"
                 elif char in self.upper:
                     result += f"[ERROR string:'{self.upper.index(char)}', rot:'{self.rot}']"
@@ -46,17 +46,17 @@
                 return "ERROR: La rotation doit être un nombre /!\\"
         if self.rot > 26:
             return "ERREUR: La rotation ne doit pas dépasser 26"
         result = str()
         for i in range(len(self.string)):
             char = no_accent_char(char=self.string[i])
             if char in self.lower:
-                result += self.lower[self.lower.index(char) - self.rot % 26]
+                result += self.lower[(self.lower.index(char) - self.rot) % 26]
             elif char in self.upper:
-                result += self.upper[self.upper.index(char) - self.rot % 26]
+                result += self.upper[(self.upper.index(char) - self.rot) % 26]
             else:
                 result += char
 
         return result
 
 
 class ROT:
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/encodings2.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/encodings2.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,58 +24,55 @@
         self.upper = s.ascii_uppercase
         self.rot = rot
         self.string = string
 
     def __str__(self):
         return self.string
 
-
     def verif(self, rot, string):
         if string:
             self.string = string
         if not self.string:
             raise Error("No string")
         if rot:
             self.rot = rot
         if not isinstance(self.rot, int):
             try:
                 self.rot = int(self.rot)
             except:
                 raise Error("La rotation doit être un nombre /!\\")
-        if self.rot > 26:
-            raise Error("La rotation ne doit pas dépasser 26")
 
-    def encode(self, rot=0, string=''):
+    def encode(self, string='', rot=0):
         self.result = ''
         self.verif(rot=rot, string=string)
         for i in range(len(self.string)):
             char = no_accent_char(char=self.string[i])
             try:
                 if char in self.lower:
-                    self.result += self.lower[self.lower.index(char) + self.rot % 26]
+                    self.result += self.lower[(self.lower.index(char) + self.rot) % 26]
                 elif char in self.upper:
-                    self.result += self.upper[self.upper.index(char) + self.rot % 26]
+                    self.result += self.upper[(self.upper.index(char) + self.rot) % 26]
                 else:
                     self.result += char
             except:
                 if char in self.lower:
                     self.result += f"[ERROR string:'{self.lower.index(char)}', rot:'{self.rot}']"
                 elif char in self.upper:
                     self.result += f"[ERROR string:'{self.upper.index(char)}', rot:'{self.rot}']"
         return Cesar(rot=self.rot, string=self.result)
 
-    def decode(self, rot=0, string=''):
+    def decode(self, string='', rot=0):
         self.result = ''
         self.verif(rot=rot, string=string)
         for i in range(len(self.string)):
             char = no_accent_char(char=self.string[i])
             if char in self.lower:
-                self.result += self.lower[self.lower.index(char) - self.rot % 26]
+                self.result += self.lower[(self.lower.index(char) - self.rot) % 26]
             elif char in self.upper:
-                self.result += self.upper[self.upper.index(char) - self.rot % 26]
+                self.result += self.upper[(self.upper.index(char) - self.rot) % 26]
             else:
                 self.result += char
 
         return Cesar(rot=self.rot, string=self.result)
 
 
 class ROT:
@@ -131,14 +128,15 @@
             except:
                 self.error(f"[ERROR string:'{s.printable.index(char)}', password:'{self.password[i % len(self.password)]}']", fatal_error=f"[FATAL ERROR: '{char}']")
         return ROT(password=self.password, string=self.result)
 
     def decode(self, string='', password=''):
         self.result = ''
         self.verif(string=string, password=password)
+
         for i in range(len(self.string)):
             char = self.string[i]
             try:
                 if char not in s.printable:
                     char = no_accent_char(char=char)
                 self.result += s.printable[(s.printable.index(char) - s.printable.index(self.password[i % len(self.password)])) % len(s.printable)]
             except:
@@ -218,14 +216,15 @@
         self.byte_result = bytearray()
         self.int_result = ''
         self.password_len = len(password)
         self.string = ''.join(str(i) for i in string) if isinstance(string, str) or isinstance(string, list) else string
         self.byte_array = byte_array
         self.password = password
         self.shift = shift
+        self.estim = 0
         if hexa:
             self.hexa = True
         else:
             self.hexa = False
         self.debug_var = debug
         self.error_input = error_input
         self.debug(f"DayEncoding vient d'être appelée, result = {type(self.result)} = {self.result}")
@@ -343,20 +342,30 @@
             raise Error(error)
 
     def debug(self, *args):
         if self.debug_var:
             print_color(*args, color='green', effect='bold')
             time.sleep(0.005)
 
+    def get_estim(self):
+        t1 = time.perf_counter()
+        random_list = []
+        for i in range(len(self.byte_array)):
+            byte = self.byte_array[i]
+            calc = ((byte + ord(self.password[i % self.password_len])) + self.shift) % 256
+            random_list.append(calc)
+            break
+        return (time.perf_counter()-t1) * len(self.byte_array)
 
     def encode_byte(self, byte_array=bytearray(), password='', shift=0):
         self.byte_result = bytearray()
         verif = self.verif_byte(byte_array=byte_array, password=password, shift=shift)
         if verif:
             return verif
+        self.estim = self.get_estim()
         for i in range(len(self.byte_array)):
             byte = self.byte_array[i]
             try:
                 self.debug("normal")
                 calc = ((byte + ord(self.password[i % self.password_len])) + self.shift) % 256
                 self.int_result += str(calc)
                 encoding = calc
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/encodings2_1.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/encodings3.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,58 +24,55 @@
         self.upper = s.ascii_uppercase
         self.rot = rot
         self.string = string
 
     def __str__(self):
         return self.string
 
-
     def verif(self, rot, string):
         if string:
             self.string = string
         if not self.string:
             raise Error("No string")
         if rot:
             self.rot = rot
         if not isinstance(self.rot, int):
             try:
                 self.rot = int(self.rot)
             except:
                 raise Error("La rotation doit être un nombre /!\\")
-        if self.rot > 26:
-            raise Error("La rotation ne doit pas dépasser 26")
 
-    def encode(self, rot=0, string=''):
+    def encode(self, string='', rot=0):
         self.result = ''
         self.verif(rot=rot, string=string)
         for i in range(len(self.string)):
             char = no_accent_char(char=self.string[i])
             try:
                 if char in self.lower:
-                    self.result += self.lower[self.lower.index(char) + self.rot % 26]
+                    self.result += self.lower[(self.lower.index(char) + self.rot) % 26]
                 elif char in self.upper:
-                    self.result += self.upper[self.upper.index(char) + self.rot % 26]
+                    self.result += self.upper[(self.upper.index(char) + self.rot) % 26]
                 else:
                     self.result += char
             except:
                 if char in self.lower:
                     self.result += f"[ERROR string:'{self.lower.index(char)}', rot:'{self.rot}']"
                 elif char in self.upper:
                     self.result += f"[ERROR string:'{self.upper.index(char)}', rot:'{self.rot}']"
         return Cesar(rot=self.rot, string=self.result)
 
-    def decode(self, rot=0, string=''):
+    def decode(self, string='', rot=0):
         self.result = ''
         self.verif(rot=rot, string=string)
         for i in range(len(self.string)):
             char = no_accent_char(char=self.string[i])
             if char in self.lower:
-                self.result += self.lower[self.lower.index(char) - self.rot % 26]
+                self.result += self.lower[(self.lower.index(char) - self.rot) % 26]
             elif char in self.upper:
-                self.result += self.upper[self.upper.index(char) - self.rot % 26]
+                self.result += self.upper[(self.upper.index(char) - self.rot) % 26]
             else:
                 self.result += char
 
         return Cesar(rot=self.rot, string=self.result)
 
 
 class ROT:
@@ -131,14 +128,15 @@
             except:
                 self.error(f"[ERROR string:'{s.printable.index(char)}', password:'{self.password[i % len(self.password)]}']", fatal_error=f"[FATAL ERROR: '{char}']")
         return ROT(password=self.password, string=self.result)
 
     def decode(self, string='', password=''):
         self.result = ''
         self.verif(string=string, password=password)
+
         for i in range(len(self.string)):
             char = self.string[i]
             try:
                 if char not in s.printable:
                     char = no_accent_char(char=char)
                 self.result += s.printable[(s.printable.index(char) - s.printable.index(self.password[i % len(self.password)])) % len(s.printable)]
             except:
@@ -209,27 +207,29 @@
                     self.result += char
             except:
                 self.error(f"[ERROR string:'{'non'}', password:'{self.password[i % len(self.password)]}']", fatal_error=f"[FATAL ERROR: '{char}']")
         return ROT_OLD(password=self.password, string=self.result)
 
 
 class DayEncoding:
-    def __init__(self, password: str, string='', byte_array=bytearray() ,shift=0, hexa=True, debug=False, error_input=False):
+    def __init__(self, password: str, string='', byte_array=bytearray(), shift=0, hexa=True, debug=False, error_input=False):
         self.result = ''
         self.byte_result = bytearray()
         self.int_result = ''
         self.password_len = len(password)
         self.string = ''.join(str(i) for i in string) if isinstance(string, str) or isinstance(string, list) else string
         self.byte_array = byte_array
         self.password = password
         self.shift = shift
+        self.count = 0
         if hexa:
             self.hexa = True
         else:
             self.hexa = False
+        self.check_error = False
         self.debug_var = debug
         self.error_input = error_input
         self.debug(f"DayEncoding vient d'être appelée, result = {type(self.result)} = {self.result}")
         self.debug(hexa)
         if not isinstance(shift, int):
             try:
                 self.shift = int(shift)
@@ -325,14 +325,15 @@
             self.debug("added")
         if isinstance(to_be_add, str):
             to_be_add += string
             self.debug("added")
         return to_be_add
 
     def error(self, error, fatal_error="[FATAL ERROR]"):
+        self.check_error = True
         try:
             if self.error_input:
                 self.result = self.add_instance(self.result, error)
             else:
                 print_color(error, color='red', effect='underline')
         except:
             if self.error_input:
@@ -343,68 +344,74 @@
             raise Error(error)
 
     def debug(self, *args):
         if self.debug_var:
             print_color(*args, color='green', effect='bold')
             time.sleep(0.005)
 
+    def get_estim(self):
+        t1 = time.perf_counter()
+        random_list = []
+        for i in range(len(self.byte_array)):
+            byte = self.byte_array[i]
+            calc = ((byte + ord(self.password[i % self.password_len])) + self.shift) % 256
+            random_list.append(calc)
+            break
+        return (time.perf_counter()-t1) * len(self.byte_array)
 
     def encode_byte(self, byte_array=bytearray(), password='', shift=0):
         self.byte_result = bytearray()
         verif = self.verif_byte(byte_array=byte_array, password=password, shift=shift)
         if verif:
             return verif
+        self.estim = self.get_estim()
         for i in range(len(self.byte_array)):
             byte = self.byte_array[i]
             try:
                 self.debug("normal")
                 calc = ((byte + ord(self.password[i % self.password_len])) + self.shift) % 256
                 self.int_result += str(calc)
                 encoding = calc
                 self.debug(encoding)
 
                 self.byte_result.append(encoding)
             except:
                 self.error(f"[ERROR byte:'{byte}', password:'{self.password[i % self.password_len]}']",
                            fatal_error=f"[FATAL ERROR '{byte}']")
-        return self.return_(self.byte_result)
+            self.count += 1
+            yield self.count
+        yield self.return_(self.byte_result)
 
 
     def encode(self, string='', password='', shift=0):
         self.result = ''
         verif = self.verif(password=password, string=string, shift=shift)
         if verif:
             return verif
-        if self.hexa:
-            for i in range(len(self.string)):
-                char = self.string[i]
-                try:
+        for i in range(len(self.string)):
+            char = self.string[i]
+            try:
+                if self.hexa:
                     self.debug("hexa")
                     self.result = tuple(self.result)
                     encoding = hex((ord(char) + ord(self.password[i % self.password_len])) + self.shift % 1114111)
                     self.debug(
                         f"'{char}' / {hex(ord(char))} == '{chr((ord(char) + ord(self.password[i % self.password_len])) + self.shift % 1114111)}' / {encoding}")
-
-                    self.result = self.add_instance(self.result, encoding)
-                except:
-                    self.error(f"[ERROR string:'{char}', password:'{self.password[i % self.password_len]}']",
-                               fatal_error=f"[FATAL ERROR '{char}']")
-        else:
-            for i in range(len(self.string)):
-                char = self.string[i]
-                try:
+                else:
                     self.debug("normal")
                     encoding = chr((ord(char) + ord(self.password[i % self.password_len])) + self.shift % 1114111)
                     self.debug(encoding)
 
-                    self.result = self.add_instance(self.result, encoding)
-                except:
-                    self.error(f"[ERROR string:'{char}', password:'{self.password[i % self.password_len]}']",
-                               fatal_error=f"[FATAL ERROR '{char}']")
-        return self.return_(self.result)
+                self.result = self.add_instance(self.result, encoding)
+            except:
+                self.error(f"[ERROR string:'{char}', password:'{self.password[i % self.password_len]}']",
+                           fatal_error=f"[FATAL ERROR '{char}']")
+            self.count += 1
+            yield self.count
+        yield self.return_(self.result)
 
     def to_hexa(self, string, to_tuple):
         for hexa in string[2:].split('0x'):
             to_tuple.append('0x' + hexa)
         return to_tuple
 
     def decode_byte(self, byte_array=bytearray(), password='', shift=0):
@@ -417,15 +424,17 @@
             byte = self.byte_array[i]
             try:
                 coding = ((byte - ord(self.password[i % self.password_len])) - self.shift) % 256
                 self.byte_result.append(coding)
                 self.debug(coding)
             except:
                 self.error(f"[ERROR, bytes:'{byte}', password:'{self.password[i % self.password_len]}']", fatal_error=f"[FATAL ERROR '{byte}']")
-        return self.return_(self.byte_result)
+            self.count += 1
+            yield self.count
+        yield self.return_(self.byte_result)
 
     def decode(self, string='', password='', shift=0):
         # Résultat en valeurs hexadecimales
         self.result = ''
         verif = self.verif(password=password, string=string, shift=shift)
         if verif:
             return verif
@@ -445,25 +454,29 @@
                 nbr = 0
                 self.debug(string)
                 for i in string:
                     letter_ord = int(i, 16)
                     self.result = self.add_instance(self.result, chr((letter_ord - ord(self.password[nbr % self.password_len]) - self.shift) % 1114111))
                     self.debug(f"'{chr(int(i, 16))}' / {i} == '{self.result[-1]}' / {hex((letter_ord - self.shift) % 1114111)}\n{self.result}")
                     nbr += 1
-                return self.return_(self.result)
+                    self.count += 1
+                    yield self.count
+                yield self.return_(self.result)
         else:
             for i in range(len(str(self.string))):
                 char = self.string[i]
                 try:
                     coding = chr(((ord(char) - ord(self.password[i % self.password_len])) - self.shift) % 1114111)
                     self.result += coding
                     self.debug(coding)
                 except:
                     self.error(f"[ERROR, string:'{char}', password:'{self.password[i % self.password_len]}']", fatal_error=f"[FATAL ERROR '{char}']")
-        return self.return_(self.result)
+                self.count += 1
+                yield self.count
+        yield self.return_(self.result)
 
 class Custom:
     def __init__(self, password: str, string='', custom=s.ascii_lowercase, error_input=False):
         self.result = ''
         self.password = password
         self.string = string
         self.custom = custom
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/main.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/main.py`

 * *Files identical despite different names*

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/new_encoding.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/new_encoding.py`

 * *Files identical despite different names*

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject/scripts.py` & `DeltacodeProject-0.7.31.1/DeltacodeProject/scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from unidecode import unidecode
+import sys
+from time import sleep
 
 bytes_ext = [
     '.png', '.jpg', '.jpeg', '.gif', '.webp', '.ico',  # Images
     '.mp3', '.wav', '.m4a', '.flac', '.aac', '.ogg', '.3gpp',  # Audio
     '.mp4', '.mov', '.avi', '.mkv',  # Vidéos
     '.pdf', '.doc', '.docx', '.xls', '.xlsx', '.ppt', '.pptx', '.chm',  # Documents
     '.exe', '.dll', '.so', '.o', '.obj', '.pyc', '.msi', '.msix', '.jar', '.rmskin',  # Fichiers binaires
@@ -18,14 +20,27 @@
     '.eml', '.msg', '.pst', '.ost', '.mbox', '.dbx', '.mbx',  # Fichiers de messagerie
     '.avi', '.flv', '.wmv', '.rm', '.rmvb', '.asf', '.mpeg', '.mpg',  # Autres formats de vidéos
     '.mid', '.midi', '.kar', '.rmi', '.m4p', '.m4b',  # Autres formats de musique
     '.cr2', '.nef', '.sr2', '.orf', '.rw2', '.pef', '.arw',  # Formats d'images RAW
     '.lnk'  # Raccourci
 ]
 
+def loading(string: str, time=0.01):
+    for char in string:
+        print(char, flush=True, end='')
+        sleep(time)
+    print()
+
+def signal_handler(signal, frame):
+    if signal == 88:
+        sys.exit(0)
+    else:
+        loading("Sortie du programme...")
+        sys.exit(0)
+
 def get_file_ex(filename):
     ext = filename[filename.index("."):]
     return ext
 
 def chercher(txt, premier, deuxieme, replace=False):
     if deuxieme == "'":
         deuxieme = "' "
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject.egg-info/PKG-INFO` & `DeltacodeProject-0.7.31.1/DeltacodeProject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeltacodeProject
-Version: 0.7.31.0
+Version: 0.7.31.1
 Summary: Encoder et décoder du texte à l'aide de pluisieurs types d'encodages
 Home-page: https://github.com/daisseur/Deltacode_project
 Author: daisseur
 Author-email: daisseur@gmail.com
 License: MIT License
         
         Copyright (c) 2022-2023 DeltacodeProject
```

### Comparing `DeltacodeProject-0.7.31.0/DeltacodeProject.egg-info/SOURCES.txt` & `DeltacodeProject-0.7.31.1/DeltacodeProject.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 DeltacodeProject/DeltacodeNew.py
 DeltacodeProject/__init__.py
 DeltacodeProject/__main__.py
 DeltacodeProject/decode.py
 DeltacodeProject/encode.py
 DeltacodeProject/encodings.py
 DeltacodeProject/encodings2.py
-DeltacodeProject/encodings2_1.py
+DeltacodeProject/encodings3.py
 DeltacodeProject/gui.py
 DeltacodeProject/main.py
+DeltacodeProject/more.py
 DeltacodeProject/new_encoding.py
+DeltacodeProject/open_file.py
 DeltacodeProject/scripts.py
 DeltacodeProject.egg-info/PKG-INFO
 DeltacodeProject.egg-info/SOURCES.txt
 DeltacodeProject.egg-info/dependency_links.txt
 DeltacodeProject.egg-info/top_level.txt
 test/test_DAY_time.py
```

### Comparing `DeltacodeProject-0.7.31.0/LICENSE` & `DeltacodeProject-0.7.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DeltacodeProject-0.7.31.0/PKG-INFO` & `DeltacodeProject-0.7.31.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeltacodeProject
-Version: 0.7.31.0
+Version: 0.7.31.1
 Summary: Encoder et décoder du texte à l'aide de pluisieurs types d'encodages
 Home-page: https://github.com/daisseur/Deltacode_project
 Author: daisseur
 Author-email: daisseur@gmail.com
 License: MIT License
         
         Copyright (c) 2022-2023 DeltacodeProject
```

### Comparing `DeltacodeProject-0.7.31.0/README.md` & `DeltacodeProject-0.7.31.1/README.md`

 * *Files identical despite different names*

### Comparing `DeltacodeProject-0.7.31.0/setup.py` & `DeltacodeProject-0.7.31.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='DeltacodeProject',
-    version='0.7.31.0',
+    version='0.7.31.1',
     author='daisseur',
     author_email='daisseur@gmail.com',
     packages=['DeltacodeProject'],
     url='https://github.com/daisseur/Deltacode_project',
     description="Encoder et décoder du texte à l'aide de pluisieurs types d'encodages",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `DeltacodeProject-0.7.31.0/test/test_DAY_time.py` & `DeltacodeProject-0.7.31.1/test/test_DAY_time.py`

 * *Files identical despite different names*

