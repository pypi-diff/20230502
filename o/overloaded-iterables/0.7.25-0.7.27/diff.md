# Comparing `tmp/overloaded-iterables-0.7.25.tar.gz` & `tmp/overloaded-iterables-0.7.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.25.tar", last modified: Tue May  2 19:09:09 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.27.tar", last modified: Tue May  2 19:12:27 2023, max compression
```

## Comparing `overloaded-iterables-0.7.25.tar` & `overloaded-iterables-0.7.27.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:09:09.866732 overloaded-iterables-0.7.25/
--rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.25/LICENSE
--rw-rw-rw-   0        0        0    10038 2023-05-02 19:09:09.867732 overloaded-iterables-0.7.25/PKG-INFO
--rw-rw-rw-   0        0        0    11888 2023-05-02 18:58:12.000000 overloaded-iterables-0.7.25/README.md
--rw-rw-rw-   0        0        0      116 2023-05-02 19:09:09.872732 overloaded-iterables-0.7.25/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-05-02 19:08:46.000000 overloaded-iterables-0.7.25/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:09:09.828667 overloaded-iterables-0.7.25/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:09:09.836729 overloaded-iterables-0.7.25/src/overloaded_iterables/
--rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.25/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    17403 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.25/src/overloaded_iterables/classes.py
--rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.25/src/overloaded_iterables/exceptions.py
--rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.25/src/overloaded_iterables/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:09:09.865738 overloaded-iterables-0.7.25/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0    10038 2023-05-02 19:09:09.000000 overloaded-iterables-0.7.25/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-05-02 19:09:09.000000 overloaded-iterables-0.7.25/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:09:09.000000 overloaded-iterables-0.7.25/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 19:09:09.000000 overloaded-iterables-0.7.25/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 19:09:09.000000 overloaded-iterables-0.7.25/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.076313 overloaded-iterables-0.7.27/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.27/LICENSE
+-rw-rw-rw-   0        0        0    12615 2023-05-02 19:12:27.079328 overloaded-iterables-0.7.27/PKG-INFO
+-rw-rw-rw-   0        0        0    11888 2023-05-02 18:58:12.000000 overloaded-iterables-0.7.27/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-02 19:12:27.081310 overloaded-iterables-0.7.27/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-05-02 19:12:09.000000 overloaded-iterables-0.7.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.052312 overloaded-iterables-0.7.27/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.059310 overloaded-iterables-0.7.27/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    17403 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/classes.py
+-rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/exceptions.py
+-rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.27/src/overloaded_iterables/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:12:27.075312 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0    12615 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-02 19:12:27.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 19:12:26.000000 overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.25/LICENSE` & `overloaded-iterables-0.7.27/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.25/PKG-INFO` & `overloaded-iterables-0.7.27/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1
-Name: overloaded-iterables
-Version: 0.7.25
-Summary: Overloaded version of the built-in python classes: list and set, to include some extra functionalities.
-Home-page: https://github.com/Arkiralor/overloaded_iterables
-Author: Prithoo Medhi
-Author-email: prithoo11335@gmail.com
-License: MIT
-Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot,queue,stack
-Platform: windows
-Platform: ubuntu-linux
-Platform: mac-os
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Overloaded Iterables
 
-Documentation on how to use `overloaded-iterables`
+Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
+
+An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
+
+## Python Package Index
+
+1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
+2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
 
 ```sh
 python -m pip install overloaded-iterables
 ```
 
@@ -251,8 +240,38 @@
         ```python
             queue = Queue(*args)
             stack = Stack(*args)
             queue.pop(num=num)
             stack.pop(num=num)
         ```
 
+## Development Setup
 
+1. `git clone https://<personal-access-token>@github.com/Arkiralor/overloaded_iterables.git`
+2. `cd overloaded_aiterables`
+3. `python -m venv env`
+4. `source env/bin/activate`
+   1. `source env/Scripts/activate` for Windows.
+5. `chmod +x scripts/*`
+6. `sh scripts/install.sh` to install all dependencies.
+   1. `sh scripts/uninstall.sh` to uninstall all dependencies (can be very useful if you forgot to activate the `virtualEnvironment` before running `install.sh`).
+7. `sh scripts/generate_coverage_report` && `sh scripts/run_tests.sh` to make sure everything is working as intended.
+
+## Contribution
+
+If you choose to contribute to this package by addressing any of the issues or tickets listed, kindly follow the following workflow.
+
+1. Assign yourself of ask an administrator to assign yourself to the issue.
+2. Clone/fork the codebase and setup the development environment as shown above.
+3. Checkout to your own branch, which should ideally be named what the ticket number is in a url-safe format i.e, if the ticket name is `WEB_003`, then the branch name will be `web-003`.
+4. `git push --set-upstream origin <branchName>` to pre-create the necessary branch on github.
+5. Make the required changes to the correct files in the `src` directory.
+6. Add any testCases required to the correct module/file/class in the `tests` directory.
+7. `sh scripts/run_tests.sh` to make sure no breaking changes were made.
+   1. __MAKE SURE ALL TESTS PASS BEFORE PROCEEDING TO THE NEXT STEP(S)__
+8. Add and commit your changes to your branch with a relevant commit message.
+9. `git merge origin/master` to pull from the master branch to your branch.
+10. `sh scripts/run_tests.sh` again to make sure nothing was broken by the merge.
+    1. __MAKE SURE ALL TESTS PASS BEFORE PROCEEDING TO THE NEXT STEP(S)__
+11. `git push` to push the changes to the remote branch.
+12. Create a Pull Request from your remote branch to `master`.
+    1. If any code changes were requested, execute them as requested and restart from step #6.
```

### Comparing `overloaded-iterables-0.7.25/README.md` & `overloaded-iterables-0.7.27/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: overloaded-iterables
+Version: 0.7.27
+Summary: Overloaded version of the built-in python classes: list and set, to include some extra functionalities.
+Home-page: https://github.com/Arkiralor/overloaded_iterables
+Author: Prithoo Medhi
+Author-email: prithoo11335@gmail.com
+License: MIT
+Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot,queue,stack
+Platform: windows
+Platform: ubuntu-linux
+Platform: mac-os
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Overloaded Iterables
 
 Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
 
 An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
 
 ## Python Package Index
@@ -271,7 +289,9 @@
 8. Add and commit your changes to your branch with a relevant commit message.
 9. `git merge origin/master` to pull from the master branch to your branch.
 10. `sh scripts/run_tests.sh` again to make sure nothing was broken by the merge.
     1. __MAKE SURE ALL TESTS PASS BEFORE PROCEEDING TO THE NEXT STEP(S)__
 11. `git push` to push the changes to the remote branch.
 12. Create a Pull Request from your remote branch to `master`.
     1. If any code changes were requested, execute them as requested and restart from step #6.
+
+
```

### Comparing `overloaded-iterables-0.7.25/setup.py` & `overloaded-iterables-0.7.27/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from dotenv import load_dotenv
 from setuptools import setup, find_packages
 
 _ = load_dotenv(dotenv_path='.env', verbose=True, override=True)
 
 
-def read(fname: str = 'DESCRIPTION.md'):
+def read(fname: str = 'README.md'):
     file_path = path.join(path.dirname(__file__), fname)
     with open(
         file=file_path,
         mode="rt",
         encoding="utf-8"
     )as file_obj:
         data = file_obj.read()
     return data
 
 setup(
     name='overloaded-iterables',
-    version='0.7.25',
+    version='0.7.27',
     description='Overloaded version of the built-in python classes: list and set, to include some extra functionalities.',
-    long_description=read('DESCRIPTION.md'),
+    long_description=read('README.md'),
     long_description_content_type='text/markdown',
     license='MIT',
     author='Prithoo Medhi',
     author_email='prithoo11335@gmail.com',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/Arkiralor/overloaded_iterables',
```

### Comparing `overloaded-iterables-0.7.25/src/overloaded_iterables/__init__.py` & `overloaded-iterables-0.7.27/src/overloaded_iterables/__init__.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.25/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.27/src/overloaded_iterables/classes.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.25/src/overloaded_iterables/exceptions.py` & `overloaded-iterables-0.7.27/src/overloaded_iterables/exceptions.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.25/src/overloaded_iterables/utils.py` & `overloaded-iterables-0.7.27/src/overloaded_iterables/utils.py`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.25/src/overloaded_iterables.egg-info/PKG-INFO` & `overloaded-iterables-0.7.27/src/overloaded_iterables.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overloaded-iterables
-Version: 0.7.25
+Version: 0.7.27
 Summary: Overloaded version of the built-in python classes: list and set, to include some extra functionalities.
 Home-page: https://github.com/Arkiralor/overloaded_iterables
 Author: Prithoo Medhi
 Author-email: prithoo11335@gmail.com
 License: MIT
 Keywords: python,built-in overloading,sequence,overloading,median,rms,root-mean-square,mean,sort,graph,histogram,scatterplot,line-plot,queue,stack
 Platform: windows
@@ -14,15 +14,22 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Overloaded Iterables
 
-Documentation on how to use `overloaded-iterables`
+Overloaded versions of the built-in python classes: `<list>` and `<set>`, to include some extra functionalities as an experiment.
+
+An experimental Python package to extend the methods found in Python's built-in list and set classes to add some extra functionality that I, personally find useful in my day-to-day implementations and was too lazy to keep writing/copy-pasting again and again.
+
+## Python Package Index
+
+1. [Project Homepage](https://pypi.org/project/overloaded-iterables/)
+2. [Contents](https://pypi.org/project/overloaded-iterables/#files)
 
 ## Installation
 
 ```sh
 python -m pip install overloaded-iterables
 ```
 
@@ -251,8 +258,40 @@
         ```python
             queue = Queue(*args)
             stack = Stack(*args)
             queue.pop(num=num)
             stack.pop(num=num)
         ```
 
+## Development Setup
+
+1. `git clone https://<personal-access-token>@github.com/Arkiralor/overloaded_iterables.git`
+2. `cd overloaded_aiterables`
+3. `python -m venv env`
+4. `source env/bin/activate`
+   1. `source env/Scripts/activate` for Windows.
+5. `chmod +x scripts/*`
+6. `sh scripts/install.sh` to install all dependencies.
+   1. `sh scripts/uninstall.sh` to uninstall all dependencies (can be very useful if you forgot to activate the `virtualEnvironment` before running `install.sh`).
+7. `sh scripts/generate_coverage_report` && `sh scripts/run_tests.sh` to make sure everything is working as intended.
+
+## Contribution
+
+If you choose to contribute to this package by addressing any of the issues or tickets listed, kindly follow the following workflow.
+
+1. Assign yourself of ask an administrator to assign yourself to the issue.
+2. Clone/fork the codebase and setup the development environment as shown above.
+3. Checkout to your own branch, which should ideally be named what the ticket number is in a url-safe format i.e, if the ticket name is `WEB_003`, then the branch name will be `web-003`.
+4. `git push --set-upstream origin <branchName>` to pre-create the necessary branch on github.
+5. Make the required changes to the correct files in the `src` directory.
+6. Add any testCases required to the correct module/file/class in the `tests` directory.
+7. `sh scripts/run_tests.sh` to make sure no breaking changes were made.
+   1. __MAKE SURE ALL TESTS PASS BEFORE PROCEEDING TO THE NEXT STEP(S)__
+8. Add and commit your changes to your branch with a relevant commit message.
+9. `git merge origin/master` to pull from the master branch to your branch.
+10. `sh scripts/run_tests.sh` again to make sure nothing was broken by the merge.
+    1. __MAKE SURE ALL TESTS PASS BEFORE PROCEEDING TO THE NEXT STEP(S)__
+11. `git push` to push the changes to the remote branch.
+12. Create a Pull Request from your remote branch to `master`.
+    1. If any code changes were requested, execute them as requested and restart from step #6.
+
```

