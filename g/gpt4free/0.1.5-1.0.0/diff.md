# Comparing `tmp/gpt4free-0.1.5.tar.gz` & `tmp/gpt4free-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-ebfjqjqa\gpt4free-0.1.5.tar", last modified: Mon May  1 19:06:23 2023, max compression
+gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-j6w1vz7a\gpt4free-1.0.0.tar", last modified: Mon May  1 20:19:49 2023, max compression
```

## Comparing `gpt4free-0.1.5.tar` & `gpt4free-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 19:06:23.088523 gpt4free-0.1.5/
--rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-0.1.5/AUTHORS.md
--rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-0.1.5/CONTRIBUTING.md
--rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-0.1.5/HISTORY.md
--rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1440 2023-05-01 19:06:23.088523 gpt4free-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-04-27 08:34:50.000000 gpt4free-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 19:06:23.049525 gpt4free-0.1.5/gpt4free/
--rw-rw-rw-   0        0        0     2068 2023-05-01 19:05:12.000000 gpt4free-0.1.5/gpt4free/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:06:23.082528 gpt4free-0.1.5/gpt4free/forefront/
--rw-rw-rw-   0        0        0     6503 2023-05-01 02:16:04.000000 gpt4free-0.1.5/gpt4free/forefront/__init__.py
--rw-rw-rw-   0        0        0      437 2023-05-01 02:16:04.000000 gpt4free-0.1.5/gpt4free/forefront/typing.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:06:23.084524 gpt4free-0.1.5/gpt4free/theb/
--rw-rw-rw-   0        0        0     1887 2023-05-01 02:16:04.000000 gpt4free-0.1.5/gpt4free/theb/__init__.py
--rw-rw-rw-   0        0        0      106 2023-05-01 02:16:04.000000 gpt4free-0.1.5/gpt4free/theb/theb_test.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:06:23.086524 gpt4free-0.1.5/gpt4free/usesless/
--rw-rw-rw-   0        0        0     1744 2023-05-01 02:16:04.000000 gpt4free-0.1.5/gpt4free/usesless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:06:23.087522 gpt4free-0.1.5/gpt4free/you/
--rw-rw-rw-   0        0        0     4037 2023-05-01 02:16:04.000000 gpt4free-0.1.5/gpt4free/you/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:06:23.056523 gpt4free-0.1.5/gpt4free.egg-info/
--rw-rw-rw-   0        0        0     1440 2023-05-01 19:06:22.000000 gpt4free-0.1.5/gpt4free.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-05-01 19:06:22.000000 gpt4free-0.1.5/gpt4free.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 19:06:22.000000 gpt4free-0.1.5/gpt4free.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 19:06:22.000000 gpt4free-0.1.5/gpt4free.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      142 2023-05-01 19:06:22.000000 gpt4free-0.1.5/gpt4free.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 19:06:22.000000 gpt4free-0.1.5/gpt4free.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-05-01 19:06:23.090522 gpt4free-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2147 2023-05-01 19:03:15.000000 gpt4free-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:19:49.257777 gpt4free-1.0.0/
+-rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-1.0.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-1.0.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-1.0.0/HISTORY.md
+-rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3533 2023-05-01 20:19:49.257777 gpt4free-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2116 2023-05-01 19:39:48.000000 gpt4free-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 20:19:49.239786 gpt4free-1.0.0/gpt4free/
+-rw-rw-rw-   0        0        0     2068 2023-05-01 19:05:12.000000 gpt4free-1.0.0/gpt4free/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:19:49.251779 gpt4free-1.0.0/gpt4free/forefront/
+-rw-rw-rw-   0        0        0     6503 2023-05-01 02:16:04.000000 gpt4free-1.0.0/gpt4free/forefront/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-05-01 02:16:04.000000 gpt4free-1.0.0/gpt4free/forefront/typing.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:19:49.253778 gpt4free-1.0.0/gpt4free/theb/
+-rw-rw-rw-   0        0        0     1887 2023-05-01 02:16:04.000000 gpt4free-1.0.0/gpt4free/theb/__init__.py
+-rw-rw-rw-   0        0        0      106 2023-05-01 02:16:04.000000 gpt4free-1.0.0/gpt4free/theb/theb_test.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:19:49.255780 gpt4free-1.0.0/gpt4free/usesless/
+-rw-rw-rw-   0        0        0     1744 2023-05-01 02:16:04.000000 gpt4free-1.0.0/gpt4free/usesless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:19:49.256778 gpt4free-1.0.0/gpt4free/you/
+-rw-rw-rw-   0        0        0     4037 2023-05-01 02:16:04.000000 gpt4free-1.0.0/gpt4free/you/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:19:49.248784 gpt4free-1.0.0/gpt4free.egg-info/
+-rw-rw-rw-   0        0        0     3533 2023-05-01 20:19:49.000000 gpt4free-1.0.0/gpt4free.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-05-01 20:19:49.000000 gpt4free-1.0.0/gpt4free.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:19:49.000000 gpt4free-1.0.0/gpt4free.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 20:19:48.000000 gpt4free-1.0.0/gpt4free.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      142 2023-05-01 20:19:49.000000 gpt4free-1.0.0/gpt4free.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 20:19:49.000000 gpt4free-1.0.0/gpt4free.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-05-01 20:19:49.259776 gpt4free-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2215 2023-05-01 20:09:56.000000 gpt4free-1.0.0/setup.py
```

### Comparing `gpt4free-0.1.5/CONTRIBUTING.md` & `gpt4free-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.5/LICENSE` & `gpt4free-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.5/gpt4free/__init__.py` & `gpt4free-1.0.0/gpt4free/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.5/gpt4free/forefront/__init__.py` & `gpt4free-1.0.0/gpt4free/forefront/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.5/gpt4free/theb/__init__.py` & `gpt4free-1.0.0/gpt4free/theb/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.5/gpt4free/usesless/__init__.py` & `gpt4free-1.0.0/gpt4free/usesless/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.5/gpt4free/you/__init__.py` & `gpt4free-1.0.0/gpt4free/you/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-0.1.5/setup.py` & `gpt4free-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Reza Shakeri",
     author_email='rzashakeri@gmail.com',
     python_requires='>=3.6',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-    description="decentralising the Ai Industry, free gpt-4/3.5 scripts through several reverse engineered api's",
+    description="decentralising the Ai Industry, just some language model api's...",
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords=[
         "gpt4free",
@@ -55,18 +55,18 @@
         "FreeChatGPT",
         "Ai"
     ],
     name='gpt4free',
     packages=find_packages(include=['gpt4free', 'gpt4free.*']),
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/rzashakeri/gpt4free',
-    version='0.1.5',
+    url='https://github.com/rzashakeri/gpt4free-python-package',
+    version='1.0.0',
     zip_safe=False,
     project_urls={
-        "Homepage": "https://github.com/rzashakeri/gpt4free",
-        "Issue tracker": "https://github.com/rzashakeri/gpt4free/issues",
-        "Release notes": "https://github.com/rzashakeri/gpt4free/releases",
-        "Source": "https://github.com/rzashakeri/gpt4free",
-        "Discussions": "https://github.com/rzashakeri/gpt4free/discussions",
+        "Homepage": "https://github.com/rzashakeri/gpt4free-python-package",
+        "Issue tracker": "https://github.com/rzashakeri/gpt4free-python-package/issues",
+        "Release notes": "https://github.com/rzashakeri/gpt4free-python-package/releases",
+        "Source": "https://github.com/rzashakeri/gpt4free-python-package",
+        "Discussions": "https://github.com/rzashakeri/gpt4free-python-package/discussions",
     },
 )
```

