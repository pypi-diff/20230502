# Comparing `tmp/crackerjack-0.1.7.tar.gz` & `tmp/crackerjack-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.1.7.tar", last modified: Wed Apr 26 14:50:27 2023, max compression
+gzip compressed data, was "crackerjack-0.1.8.tar", last modified: Mon May  1 23:09:00 2023, max compression
```

## Comparing `crackerjack-0.1.7.tar` & `crackerjack-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.1.7/LICENSE
--rw-r--r--   0        0        0     2856 2023-04-26 12:28:28.914334 crackerjack-0.1.7/README.md
--rw-r--r--   0        0        0      171 2023-04-26 14:49:09.680121 crackerjack-0.1.7/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-04-26 14:49:09.713961 crackerjack-0.1.7/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2055 2023-04-26 14:49:09.696832 crackerjack-0.1.7/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.1.7/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.1.7/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.1.7/crackerjack/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-26 12:28:28.914593 crackerjack-0.1.7/crackerjack/__main__.py
--rw-r--r--   0        0        0     4354 2023-04-26 14:43:54.841161 crackerjack-0.1.7/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1655 2023-04-26 14:49:09.729506 crackerjack-0.1.7/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     5606 2023-04-25 20:30:39.178113 crackerjack-0.1.7/crackerjack/test1.py
--rw-r--r--   0        0        0     1655 2023-04-26 14:50:27.747998 crackerjack-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 crackerjack-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2856 2023-04-26 12:28:28.914334 crackerjack-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 23:08:28.495079 crackerjack-0.1.8/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      197 2023-05-01 23:08:32.884162 crackerjack-0.1.8/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-05-01 23:08:28.479220 crackerjack-0.1.8/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2055 2023-05-01 23:08:32.884329 crackerjack-0.1.8/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.1.8/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.1.8/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.1.8/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1099 2023-05-01 23:08:32.884408 crackerjack-0.1.8/crackerjack/__main__.py
+-rw-r--r--   0        0        0     4966 2023-05-01 23:08:32.884487 crackerjack-0.1.8/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1708 2023-05-01 23:08:32.884579 crackerjack-0.1.8/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     5606 2023-04-25 20:30:39.178113 crackerjack-0.1.8/crackerjack/test1.py
+-rw-r--r--   0        0        0     1705 2023-05-01 23:09:00.904627 crackerjack-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 crackerjack-0.1.8/PKG-INFO
```

### Comparing `crackerjack-0.1.7/LICENSE` & `crackerjack-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.7/README.md` & `crackerjack-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.7/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.1.8/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.7/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.1.8/crackerjack/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: v0.0.263
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
-    rev: v2.6.0
+    rev: v2.6.1
     hooks:
       - id: creosote
         args:
           - --venv=__pypackages__/3.11/lib
           - --paths=crackerjack
   #          - --deps-file=pyproject.toml
   #          - --sections=project.dependencies
```

### Comparing `crackerjack-0.1.7/crackerjack/crackerjack.py` & `crackerjack-0.1.8/crackerjack/crackerjack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,137 @@
 import sys
+import typing as t
 from subprocess import call
 from subprocess import check_output
 from subprocess import run
 
 import pdm_bump
 import pdoc
 from acb.actions import dump
 from acb.actions import load
-from addict import Dict as adict
-from aiopath import AsyncPath
-from pydantic import BaseModel
+from addict import Dict
 from aioconsole import ainput
+from aiopath import AsyncPath
 from inflection import underscore
+from pydantic import BaseModel
 
-for mod in (pdm_bump, pdoc):
+for mod in (pdm_bump, pdoc):  # look ruff / isort to get rid of this
     pass
 
 
 # Crackerjack
 
 
 class Crakerjack(BaseModel):
-    path: AsyncPath = AsyncPath(__file__)
+    our_path: AsyncPath = AsyncPath(__file__)
     pkg_path: AsyncPath = AsyncPath.cwd()
+    pkg_dir: t.Optional[AsyncPath] = None
     pkg_name: str = "crackerjack"
+    our_toml: t.Optional[dict] = None
+    pkg_toml: t.Optional[dict] = None
+    our_toml_path: t.Optional[AsyncPath] = None
+    pkg_toml_path: t.Optional[AsyncPath] = None
     poetry_pip_env: bool = False
 
-    class Config:
-        extra = "allow"
+    async def update_pyproject_configs(self) -> None:
+        our_toml_config = await load.toml(self.our_toml_path)
+        pkg_toml_config = await load.toml(self.pkg_toml_path)
+        if self.poetry_pip_env:
+            del pkg_toml_config.tool.poetry
+        old_deps = pkg_toml_config.tool.pdm["dev-dependencies"]
+        pkg_toml_config.tool = our_toml_config.tool
+        pkg_toml_config.tool.pdm["dev-dependencies"] = old_deps
+        await dump.toml(pkg_toml_config, self.pkg_toml_path)
 
     async def clean_poetry_pip_env(self) -> None:
         root_files = [
             file
             async for file in self.pkg_path.iterdir()
             if ("poetry" or "Pip") in file.name
         ]
         if root_files:
             self.poetry_pip_env = True
             for file in root_files:
                 await file.unlink()
 
-    async def update_pyproject_configs(self) -> None:
-        toml = await load.toml(self.toml_path)
-        pkg_toml = await load.toml(self.pkg_toml_path)
-        if self.poetry_pip_env:
-            del pkg_toml.tool.poetry
-        old_deps = pkg_toml.tool.pdm["dev-dependencies"]
-        pkg_toml.tool = toml.tool
-        pkg_toml.tool.pdm["dev-dependencies"] = old_deps
-        await dump.toml(pkg_toml, self.pkg_toml_path)
-
     async def copy_configs(self) -> None:
         for config in (
             ".gitignore",
             ".pre-commit-config.yaml",
             ".libcst.codemod.yaml",
-            "pyproject.toml",
+            ".crackerjack-config.yaml",
         ):
-            config_path = self.path.parent / config
+            config_path = self.our_path.parent / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
             run(["git", "add", str(pkg_config_path)])
             if self.pkg_path.stem == "crackerjack":
                 await config_path.write_text(await pkg_config_path.read_text())
-            elif config != "pyproject.toml":
-                # if poetry_pip_env:
-                #     await config_pkg_path.unlink()
-                config_text = await config_path.read_text()
-                await pkg_config_path.write_text(
-                    config_text.replace("crackerjack", self.pkg_name)
-                )
+            # if poetry_pip_env:
+            #     await config_pkg_path.unlink()
+            config_text = await config_path.read_text()
+            await pkg_config_path.write_text(
+                config_text.replace("crackerjack", self.pkg_name)
+            )
+
+    @staticmethod
+    async def run_interactive(hook: str) -> None:
+        success = False
+        while not success:
+            fail = call(["pre-commit", "run", hook.lower()])
+            if fail > 0:
+                retry = await ainput(f"\n{hook} failed. Retry? (y/n): ")
+                if retry.lower() == "y":
+                    continue
+                sys.exit()
+            success = True
 
     async def update_pkg_configs(self) -> None:
-        # await self.clean_poetry_pip_env()
+        await self.clean_poetry_pip_env()
         await self.copy_configs()
         toml_file = "pyproject.toml"
-        self.toml_path = self.path.parent / toml_file
+        self.our_toml_path = self.our_path.parent / toml_file
         self.pkg_toml_path = self.pkg_path / toml_file
         if not await self.pkg_toml_path.exists():
             run(["pdm", "init"])
+            run(["git", "add", "pyproject.toml"])
+            # run(["git", "add", "pdm.lock"])
         installed_pkgs = check_output(
             ["pdm", "list", "--freeze"],
             universal_newlines=True,
         ).splitlines()
         if not len([pkg for pkg in installed_pkgs if "pre-commit" in pkg]):
             run(["pdm", "add", "-d", "pre_commit"])
             run(["pre-commit", "install"])
+            run(["git", "add", "pdm.lock"])
         await self.update_pyproject_configs()
 
     async def process(
         self,
-        options: adict[str, str | bool],
+        options: Dict[str, str | bool],
     ) -> None:
         imp_dir = self.pkg_path / "__pypackages__"
         sys.path.append(str(imp_dir))
         self.pkg_name = underscore(self.pkg_path.stem.lower())
+        self.pkg_dir = self.pkg_path / self.pkg_name
+        await self.pkg_dir.mkdir(exist_ok=True)
         print("\nCrackerjacking...\n")
         if self.pkg_path.stem == "crackerjack":
-            check_output(["pre-commit", "autoupdate"])
-        await self.update_pkg_configs()
+            run(["pre-commit", "autoupdate"])
+        if not options.do_not_update_configs:
+            await self.update_pkg_configs()
         if options.interactive:
-            success = False
-            while not success:
-                fail = call(["pre-commit", "run", "mypy", "--all-files"])
-                if fail > 0:
-                    retry = await ainput("\nMyPy failed. Retry? (y/n): ")
-                    if retry.lower == ("y"):
-                        continue
-                    sys.exit()
-                success = True
-        check_all = call(["pre-commit", "run", "--all-files"])
+            for hook in ("ruff", "mypy"):
+                await self.run_interactive(hook)
+        check_all = call(["pre-commit", "run"])
         if check_all > 0:
             call(["pre-commit", "run", "--all-files"])
         if options.publish:
             check_output(["pdm", "bump", options.publish])
-            if options.commit:
-                commit_msg = input("Commit message: ")
-                call(["git", "commit", "-m", f"'{commit_msg}'", "--", "."])
-                call(["git", "push", "origin", "main"])
             run(["pdm", "publish"])
+        if options.commit:
+            commit_msg = input("Commit message: ")
+            call(["git", "commit", "-m", f"'{commit_msg}'", "--", "."])
+            call(["git", "push", "origin", "main"])
 
 
 crackerjack_it = Crakerjack().process
```

### Comparing `crackerjack-0.1.7/crackerjack/pyproject.toml` & `crackerjack-0.1.8/crackerjack/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,25 @@
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
 [tool.mypy]
-strict = true
+strict = false
 pretty = true
+ignore_missing_imports = false
+exclude = "tests"
+
 
 [tool.refurb]
 enable_all = true
 
+
+
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "Crackerjack"
```

### Comparing `crackerjack-0.1.7/crackerjack/test1.py` & `crackerjack-0.1.8/crackerjack/test1.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.7/pyproject.toml` & `crackerjack-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,28 +23,30 @@
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
 [tool.mypy]
-strict = true
+strict = false
 pretty = true
+ignore_missing_imports = false
+exclude = "tests"
 
 [tool.refurb]
 enable_all = true
 
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "Crackerjack"
-version = "0.1.7"
+version = "0.1.8"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.1.7/PKG-INFO` & `crackerjack-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.1.7
+Version: 0.1.8
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

