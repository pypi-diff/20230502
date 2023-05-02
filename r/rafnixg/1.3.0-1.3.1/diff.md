# Comparing `tmp/rafnixg-1.3.0.tar.gz` & `tmp/rafnixg-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rafnixg-1.3.0.tar", last modified: Sat Apr 29 04:30:55 2023, max compression
+gzip compressed data, was "rafnixg-1.3.1.tar", last modified: Tue May  2 21:46:07 2023, max compression
```

## Comparing `rafnixg-1.3.0.tar` & `rafnixg-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.688943 rafnixg-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-29 04:30:42.000000 rafnixg-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-29 04:30:55.688943 rafnixg-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-29 04:30:42.000000 rafnixg-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-29 04:30:42.000000 rafnixg-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 04:30:55.688943 rafnixg-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.684943 rafnixg-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.684943 rafnixg-1.3.0/src/rafnixg/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-29 04:30:42.000000 rafnixg-1.3.0/src/rafnixg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-29 04:30:42.000000 rafnixg-1.3.0/src/rafnixg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-29 04:30:42.000000 rafnixg-1.3.0/src/rafnixg/rafnixg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 04:30:55.688943 rafnixg-1.3.0/src/rafnixg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 04:30:55.000000 rafnixg-1.3.0/src/rafnixg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:07.844894 rafnixg-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 21:45:45.000000 rafnixg-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 21:46:07.844894 rafnixg-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 21:45:45.000000 rafnixg-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-02 21:45:45.000000 rafnixg-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:46:07.844894 rafnixg-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:07.840894 rafnixg-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:07.840894 rafnixg-1.3.1/src/rafnixg/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 21:45:45.000000 rafnixg-1.3.1/src/rafnixg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 21:45:45.000000 rafnixg-1.3.1/src/rafnixg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-02 21:45:45.000000 rafnixg-1.3.1/src/rafnixg/rafnixg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:07.844894 rafnixg-1.3.1/src/rafnixg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 21:46:07.000000 rafnixg-1.3.1/src/rafnixg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 21:46:07.000000 rafnixg-1.3.1/src/rafnixg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:46:07.000000 rafnixg-1.3.1/src/rafnixg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 21:46:07.000000 rafnixg-1.3.1/src/rafnixg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 21:46:07.000000 rafnixg-1.3.1/src/rafnixg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:46:07.000000 rafnixg-1.3.1/src/rafnixg.egg-info/top_level.txt
```

### Comparing `rafnixg-1.3.0/LICENSE` & `rafnixg-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rafnixg-1.3.0/PKG-INFO` & `rafnixg-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rafnixg
-Version: 1.3.0
+Version: 1.3.1
 Summary: Rafnix Guzman Personal Card
 Author-email: Rafnix Guzman <rafnixg@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafnix Gabriel Guzmán García @rafnixg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rafnixg-1.3.0/pyproject.toml` & `rafnixg-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rafnixg"
-version = "1.3.0"
+version = "1.3.1"
 description = "Rafnix Guzman Personal Card"
 readme = "README.md"
 authors = [{ name = "Rafnix Guzman", email = "rafnixg@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -25,15 +25,15 @@
 
 [project.urls]
 Homepage = "https://github.com/rafnixg/rafnixg-lib"
 
 [project.scripts]
 rafnixg = "rafnixg.__main__:main"
 [tool.bumpver]
-current_version = "1.3.0"
+current_version = "1.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `rafnixg-1.3.0/src/rafnixg/rafnixg.py` & `rafnixg-1.3.1/src/rafnixg/rafnixg.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,60 +11,29 @@
         self.name = "Rafnix Guzmán"
         self.position = "Python Software Developer"
         self.web = "https://rafnixg.dev"
         self.blog = "https://blog.rafnixg.dev"
         self.cv = "https://rafnixg.dev/resume"
         self.github = "https://github.com/rafnixg"
         self.twitter = "@rafnixg"
-        self.code = {
-            "backend": [
-                "Python",
-                "Odoo",
-                "FastAPI",
-                "Flask",
-                "Django",
-            ],
-            "database": ["PostgreSQL", "MySQL", "SQLite3", "Mongo DB", "Redis"],
-            "devops": [
-                "Docker",
-                "Linux",
-                "Jenkins",
-                "GitHub Actions",
-                "AWS",
-                "Proxmox",
-                "LXC",
-            ],
-            "frontend": ["HTML", "CSS", "JavaScript", "ReactJS", "Svelte", "Boostrap"],
-            "tools": [
-                "GIT",
-                "GitHub",
-                "GitLab",
-                "Pandas",
-                "Jupyter notebook",
-                "SQLAlchemy",
-                "Celery",
-                "Nginx",
-            ],
-            "misc": ["LLMs", "TDD", "SCRUM", "SOLID", "gRPC", "ML", "Tech Writer"],
-        }
-        self.architecture = ["SPA", "MVC", "Serverless", "microservices"]
+        self.about = "Experienced software developer with 10+ years of expertise in designing, developing and implementing web systems across various sectors. Backend specialist skilled in Python, Linux, and Git. Passionate about continuous learning and open-source technology."
+
 
     def __str__(self):
         return f"{self.name} (@{self.username}) - {self.position}"
 
     def display(self):
         """Display personal card"""
         console = Console()
 
         table = Table(
             show_header=False,
             title=str(self),
             highlight=True,
-            title_style="bold magenta"
-
+            title_style="bold magenta",
         )
         table.add_column("Attribute", style="bold", width=16)
         table.add_column("Value")
 
         for key, value in self.__dict__.items():
             if isinstance(value, dict):
                 for sub_key, sub_value in value.items():
```

### Comparing `rafnixg-1.3.0/src/rafnixg.egg-info/PKG-INFO` & `rafnixg-1.3.1/src/rafnixg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rafnixg
-Version: 1.3.0
+Version: 1.3.1
 Summary: Rafnix Guzman Personal Card
 Author-email: Rafnix Guzman <rafnixg@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafnix Gabriel Guzmán García @rafnixg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

