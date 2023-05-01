# Comparing `tmp/splittr-0.0.2.tar.gz` & `tmp/splittr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splittr-0.0.2.tar", last modified: Mon May  1 15:42:18 2023, max compression
+gzip compressed data, was "splittr-0.0.3.tar", last modified: Mon May  1 22:47:57 2023, max compression
```

## Comparing `splittr-0.0.2.tar` & `splittr-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:42:18.838761 splittr-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 15:42:06.000000 splittr-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 15:42:18.838761 splittr-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 15:42:06.000000 splittr-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:42:18.838761 splittr-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-05-01 15:42:06.000000 splittr-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:42:18.838761 splittr-0.0.2/splittr/
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-01 15:42:06.000000 splittr-0.0.2/splittr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:42:18.838761 splittr-0.0.2/splittr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 15:42:18.000000 splittr-0.0.2/splittr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:47:57.956873 splittr-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 22:47:45.000000 splittr-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 22:47:57.956873 splittr-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 22:47:45.000000 splittr-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 22:47:57.956873 splittr-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3291 2023-05-01 22:47:45.000000 splittr-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:47:57.956873 splittr-0.0.3/splittr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-01 22:47:45.000000 splittr-0.0.3/splittr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:47:57.956873 splittr-0.0.3/splittr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/top_level.txt
```

### Comparing `splittr-0.0.2/LICENSE` & `splittr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splittr-0.0.2/setup.py` & `splittr-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 from pathlib import Path
 import glob
 from glob import glob as re
 try:
 	from pylint.reporters.json_reporter import JSONReporter
 except:
 	pass
-try:
-	from src.information import VERSION, REQ
-except:
-	pass
-try:
-	from information import VERSION, REQ
-except:
-	pass
 
 # endregion
 # region Basic Information
 here = os.path.abspath(os.path.dirname(__file__))
 py_version = sys.version_info[:2]
 NAME = "splittr"
 AUTHOR = 'Miles Frantz'
@@ -31,15 +23,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `splittr-0.0.2/splittr/__init__.py` & `splittr-0.0.3/splittr/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,19 +65,24 @@
 	parser = argparse.ArgumentParser(description=f"Enabling the capability to stretch a single large file into many smaller files")
 	parser.add_argument("-f","--file", help="The name of the file", nargs='*')
 	parser.add_argument("--split", help="Split the file up", action="store_true",default=False)
 	parser.add_argument("--join", help="Recreate the file", action="store_true",default=False)
 	parser.add_argument("--template", help="Create a copy of this file specific to a large file", action="store_true",default=False)
 	return parser.parse_args()
 
+def splitt(foil):
+	hash(foil);split(foil)
+def joinn(foil):
+	join(foil);verify(foil)
+
 def main(foil:str,splitfile:bool=False, joinfile:bool=False):
 	if splitfile:
-		hash(foil);split(foil)
+		splitt(foil)
 	elif joinfile:
-		join(foil);verify(foil)
+		joinn(foil)
 
 if __name__ == '__main__':
 	argz = arguments();workingfoil = argz.file[0]
 	if argz.template:
 		with open(__file__, "r") as reader:
 			with open(workingfoil + ".py", "w+") as writer:
 				for line in reader.readlines():
@@ -88,12 +93,8 @@
 		print(workingfoil + ".py")
 	else:
 		if argz.split and argz.join:
 			print("Cannot use both both split and join")
 		elif not os.path.exists(argz.file[0]):
 			print("The file {file} does not exist".format(file=argz.file[0]))
 		else:
-			main(
-				workingfoil,
-				splitfile=argz.split,
-				joinfile=argz.join,
-			)
+			main(workingfoil, splitfile=argz.split, joinfile=argz.join)
```

