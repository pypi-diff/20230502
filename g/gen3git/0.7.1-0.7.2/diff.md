# Comparing `tmp/gen3git-0.7.1.tar.gz` & `tmp/gen3git-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3git-0.7.1.tar", last modified: Fri Apr 14 18:24:26 2023, max compression
+gzip compressed data, was "gen3git-0.7.2.tar", last modified: Tue May  2 18:20:31 2023, max compression
```

## Comparing `gen3git-0.7.1.tar` & `gen3git-0.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-14 18:24:26.822392 gen3git-0.7.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-04-14 18:23:33.000000 gen3git-0.7.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2023-04-14 18:23:33.000000 gen3git-0.7.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2023-04-14 18:23:33.000000 gen3git-0.7.1/NOTICE
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-04-14 18:24:26.818390 gen3git-0.7.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2023-04-14 18:23:33.000000 gen3git-0.7.1/Pipfile
--rw-r--r--   0 travis    (2000) travis    (2000)    27222 2023-04-14 18:23:48.000000 gen3git-0.7.1/Pipfile.lock
--rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2023-04-14 18:23:33.000000 gen3git-0.7.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-14 18:24:26.818390 gen3git-0.7.1/gen3git.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    20714 2023-04-14 18:23:33.000000 gen3git-0.7.1/gen3git.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-14 18:24:26.822392 gen3git-0.7.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      928 2023-04-14 18:24:10.000000 gen3git-0.7.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-02 18:20:31.588682 gen3git-0.7.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-05-02 18:19:39.000000 gen3git-0.7.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2023-05-02 18:19:39.000000 gen3git-0.7.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      558 2023-05-02 18:19:39.000000 gen3git-0.7.2/NOTICE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-05-02 18:20:31.588682 gen3git-0.7.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      177 2023-05-02 18:19:39.000000 gen3git-0.7.2/Pipfile
+-rw-r--r--   0 travis    (2000) travis    (2000)    27197 2023-05-02 18:19:53.000000 gen3git-0.7.2/Pipfile.lock
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2023-05-02 18:19:39.000000 gen3git-0.7.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-02 18:20:31.588682 gen3git-0.7.2/gen3git.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-05-02 18:20:31.000000 gen3git-0.7.2/gen3git.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-05-02 18:20:31.000000 gen3git-0.7.2/gen3git.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-02 18:20:31.000000 gen3git-0.7.2/gen3git.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-05-02 18:20:31.000000 gen3git-0.7.2/gen3git.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2023-05-02 18:20:31.000000 gen3git-0.7.2/gen3git.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-02 18:20:31.000000 gen3git-0.7.2/gen3git.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20715 2023-05-02 18:19:39.000000 gen3git-0.7.2/gen3git.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-05-02 18:20:31.588682 gen3git-0.7.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      928 2023-05-02 18:20:15.000000 gen3git-0.7.2/setup.py
```

### Comparing `gen3git-0.7.1/LICENSE` & `gen3git-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3git-0.7.1/NOTICE` & `gen3git-0.7.2/NOTICE`

 * *Files identical despite different names*

### Comparing `gen3git-0.7.1/Pipfile.lock` & `gen3git-0.7.2/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975490196078431%*

 * *Differences: {"'default'": "{'requests': {'hashes': "*

 * *              "['sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b', "*

 * *              "'sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059'], "*

 * *              '\'markers\': "python_version >= \'3.7\'", \'version\': \'==2.29.0\'}}'}*

```diff
@@ -274,19 +274,19 @@
                 "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.5.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b",
+                "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.29.0"
         },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
             "markers": "python_version >= '3.6'",
```

### Comparing `gen3git-0.7.1/README.md` & `gen3git-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `gen3git-0.7.1/gen3git.py` & `gen3git-0.7.2/gen3git.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,15 @@
                 if line.startswith("Bumps"):
                     release_notes.setdefault(category, []).append(
                         "%s (#%s)" % (line, ref)
                     )
             return release_notes
 
         for line in body.splitlines():
-            if line.startswith("###"):
+            if line.startswith("### "):
                 category = line.replace("###", "").strip().lower()
                 if category not in release_notes:
                     release_notes[category] = []
             elif line:
                 line = parse_line(line)
                 if line:
                     release_notes[category].append("%s (%s)" % (line, ref_link))
```

### Comparing `gen3git-0.7.1/setup.py` & `gen3git-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,14 @@
             "distribution; please either download the source from PyPI, or check out "
             "from GitHub and make sure that the git CLI is available."
         )
 
 
 setup(
     name="gen3git",
-    version='0.7.1',
+    version='0.7.2',
     description="Helps with release.",
     license="Apache",
     py_modules=["gen3git"],
     install_requires=['enum;python_version<"3.4"', "PyGithub", "requests", "gitpython"],
     entry_points={"console_scripts": ["gen3git=gen3git:main"]},
 )
```

