# Comparing `tmp/badgie-0.6.2.tar.gz` & `tmp/badgie-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.6.2.tar", last modified: Sun Apr 30 21:30:09 2023, max compression
+gzip compressed data, was "badgie-0.7.0.tar", last modified: Tue May  2 21:33:10 2023, max compression
```

## Comparing `badgie-0.6.2.tar` & `badgie-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 21:30:09.980367 badgie-0.6.2/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-30 21:30:05.000000 badgie-0.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4641 2023-04-30 21:30:09.980367 badgie-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3749 2023-04-30 21:30:05.000000 badgie-0.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 21:30:09.974367 badgie-0.6.2/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-30 21:30:06.000000 badgie-0.6.2/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 21:30:09.978367 badgie-0.6.2/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/badges/codestyle.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6137 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 21:30:09.980367 badgie-0.6.2/badgie/finders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/finders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/finders/files.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/finders/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/finders/pre_commit_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/finders/remotes.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/project.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-04-30 21:30:05.000000 badgie-0.6.2/badgie/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 21:30:09.976367 badgie-0.6.2/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4641 2023-04-30 21:30:09.000000 badgie-0.6.2/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-30 21:30:09.000000 badgie-0.6.2/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 21:30:09.000000 badgie-0.6.2/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-30 21:30:09.000000 badgie-0.6.2/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-30 21:30:09.000000 badgie-0.6.2/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-30 21:30:09.000000 badgie-0.6.2/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-30 21:30:09.981367 badgie-0.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-30 21:30:06.000000 badgie-0.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.239818 badgie-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-02 21:33:05.000000 badgie-0.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-05-02 21:33:10.239818 badgie-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3749 2023-05-02 21:33:05.000000 badgie-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.234818 badgie-0.7.0/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-02 21:33:07.000000 badgie-0.7.0/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.237818 badgie-0.7.0/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/codestyle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6403 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.239818 badgie-0.7.0/badgie/finders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/pre_commit_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/finders/remotes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/project.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-05-02 21:33:05.000000 badgie-0.7.0/badgie/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:33:10.235818 badgie-0.7.0/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 21:33:10.000000 badgie-0.7.0/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-02 21:33:10.240818 badgie-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-02 21:33:07.000000 badgie-0.7.0/setup.py
```

### Comparing `badgie-0.6.2/LICENSE` & `badgie-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/PKG-INFO` & `badgie-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.6.2
+Version: 0.7.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge,template,markdown
 Platform: UNKNOWN
```

### Comparing `badgie-0.6.2/README.md` & `badgie-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/badges/brettops.py` & `badgie-0.7.0/badgie/badges/brettops.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/badges/codestyle.py` & `badgie-0.7.0/badgie/badges/codestyle.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/badges/gitlab.py` & `badgie-0.7.0/badgie/badges/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/badges/precommit.py` & `badgie-0.7.0/badgie/badges/precommit.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/cli.py` & `badgie-0.7.0/badgie/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from . import tokens as to
 from ._version import __version__
 from .badges._base import _BADGES
 from .finders import files, gitlab, pre_commit_config, remotes
 from .models import Badge, Context
 from .parser import parse_text
 from .project import get_project_root
-from .urls import add_to_query
+from .utils import add_to_query, change_directory
 
 
 def to_markdown(badge):
     return f"[![{badge.title}]({badge.image})]({badge.link})"
 
 
 def get_badge_text(badges, format="markdown"):
@@ -50,15 +50,15 @@
         )
 
     def __call__(self, parser, _namespace, _values, _option_string=None):
         init_badges()
         for badge in sorted(_BADGES.values(), key=lambda x: x.name):
             print(
                 "{name}: {description}".format(
-                    name=colored(badge.name, "cyan", attrs=["bold"]),
+                    name=colored(badge.name, "yellow"),
                     description=badge.description.strip(),
                 )
             )
         parser.exit()
 
 
 class DumpAction(argparse.Action):
@@ -118,19 +118,15 @@
 
 def assemble_badge_list(context: Context, style: Optional[str] = None) -> list[Badge]:
     badges = []
     for token, nodelist in context.nodes.items():
         if token in _BADGES:
             badge = _BADGES[token]
             print(
-                colored(
-                    "- adding a {name} badge".format(
-                        name=colored(badge.name, "blue", attrs=["bold"])
-                    )
-                ),
+                "- adding a {name} badge".format(name=colored(badge.name, "yellow")),
                 file=sys.stderr,
             )
             node = nodelist[0]
 
             image = badge.image.format(node=node)
 
             if style:
@@ -149,28 +145,27 @@
             badges.append(finalbadge)
 
     return sorted(badges, key=lambda badge: badge.weight)
 
 
 def build_badge_context() -> Context:
     project_root = get_project_root()
-    os.chdir(project_root)
-
-    init_badges()
 
-    context = Context(path=project_root)
+    with change_directory(project_root):
+        init_badges()
 
-    context.run(files)
-    context.run(remotes)
-    if to.GITLAB in context.nodes:
-        context.run(gitlab)
-    if to.PRE_COMMIT_CONFIG in context.nodes:
-        context.run(pre_commit_config)
+        context = Context(path=project_root)
+        context.run(files)
+        context.run(remotes)
+        if to.GITLAB in context.nodes:
+            context.run(gitlab)
+        if to.PRE_COMMIT_CONFIG in context.nodes:
+            context.run(pre_commit_config)
 
-    return context
+        return context
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-l", "--list", action=ListAction, help="list available badges")
     parser.add_argument("--dump-badge-data", action=DumpAction, help="dump badge data")
     parser.add_argument(
@@ -181,41 +176,45 @@
         "--style",
         choices=["plastic", "flat", "flat-square", "for-the-badge", "social"],
         help="change badge style",
     )
     parser.add_argument(
         "-V", "--version", action="version", version=f"%(prog)s {__version__}"
     )
-    parser.add_argument(
-        "input",
-    )
+    parser.add_argument("files", nargs="+", metavar="FILE", help="input files")
 
     args = parser.parse_args()
 
     logging.basicConfig(level=logging.WARNING)
 
-    text = open(args.input, "r").read()
+    for file in args.files:
+        if not Path(file).exists() or not Path(file).is_file():
+            parser.error(f"Unable to find file: {file}")
 
     print(
-        colored("Hi, I'm", "cyan", attrs=["bold"]),
-        colored("Badgie!", "white", attrs=["bold"]),
-        colored("Let's add some badges! 🐦\n", "cyan", attrs=["bold"]),
+        colored("Hi, I'm", "white", attrs=["bold"]),
+        colored("Badgie!", "yellow", attrs=["bold"]),
+        colored("Let's add some badges!", "white", attrs=["bold"]),
+        colored("🐦\n", "cyan", attrs=["bold"]),
         file=sys.stderr,
     )
 
     context = build_badge_context()
     badges = assemble_badge_list(context, style=args.style)
     badge_text = get_badge_text(badges=badges)
-    output = parse_text(text, badge_text=badge_text)
 
     print(
-        colored("\nThat's like", "cyan", attrs=["bold"]),
-        colored(f"{len(badges)} badges!", "white", attrs=["bold"]),
-        colored("Good job! 🐦", "cyan", attrs=["bold"]),
+        colored("\nThat's like", "white", attrs=["bold"]),
+        colored(f"{len(badges)} badges!", "yellow", attrs=["bold"]),
+        colored("Good job!", "white", attrs=["bold"]),
+        colored("🐦", "cyan", attrs=["bold"]),
         file=sys.stderr,
     )
 
-    if args.write:
-        with open(args.input, "w") as handle:
-            handle.write(output)
-    else:
-        print(output)
+    for file in args.files:
+        text = open(file, "r").read()
+        output = parse_text(text, badge_text=badge_text)
+        if args.write:
+            with open(file, "w") as handle:
+                handle.write(output)
+        else:
+            print(output)
```

### Comparing `badgie-0.6.2/badgie/finders/files.py` & `badgie-0.7.0/badgie/finders/files.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/finders/gitlab.py` & `badgie-0.7.0/badgie/finders/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/finders/pre_commit_config.py` & `badgie-0.7.0/badgie/finders/pre_commit_config.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/finders/remotes.py` & `badgie-0.7.0/badgie/finders/remotes.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/models.py` & `badgie-0.7.0/badgie/models.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/parser.py` & `badgie-0.7.0/badgie/parser.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/project.py` & `badgie-0.7.0/badgie/project.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie/tokens.py` & `badgie-0.7.0/badgie/tokens.py`

 * *Files identical despite different names*

### Comparing `badgie-0.6.2/badgie.egg-info/PKG-INFO` & `badgie-0.7.0/badgie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.6.2
+Version: 0.7.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge,template,markdown
 Platform: UNKNOWN
```

### Comparing `badgie-0.6.2/badgie.egg-info/SOURCES.txt` & `badgie-0.7.0/badgie.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 badgie/cli.py
 badgie/constants.py
 badgie/models.py
 badgie/parser.py
 badgie/project.py
 badgie/py.typed
 badgie/tokens.py
-badgie/urls.py
+badgie/utils.py
 badgie.egg-info/PKG-INFO
 badgie.egg-info/SOURCES.txt
 badgie.egg-info/dependency_links.txt
 badgie.egg-info/entry_points.txt
 badgie.egg-info/requires.txt
 badgie.egg-info/top_level.txt
 badgie/badges/__init__.py
```

### Comparing `badgie-0.6.2/setup.py` & `badgie-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

