# Comparing `tmp/cz_conventional_gitmoji-0.1.2.tar.gz` & `tmp/cz_conventional_gitmoji-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_conventional_gitmoji-0.1.2.tar", max compression
+gzip compressed data, was "cz_conventional_gitmoji-0.1.3.tar", max compression
```

## Comparing `cz_conventional_gitmoji-0.1.2.tar` & `cz_conventional_gitmoji-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     2506 2022-12-27 13:45:34.777631 cz_conventional_gitmoji-0.1.2/README.md
--rw-r--r--   0        0        0     1969 2022-12-27 13:45:34.777631 cz_conventional_gitmoji-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       85 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/cz_gitmoji/__init__.py
--rw-r--r--   0        0        0     1285 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/cz_gitmoji/conventional_gitmojis_info.txt
--rw-r--r--   0        0        0    13515 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/cz_gitmoji/main.py
--rw-r--r--   0        0        0        0 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/gitmojify/__init__.py
--rw-r--r--   0        0        0     1669 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/gitmojify/mojify.py
--rw-r--r--   0        0        0        0 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/shared/__init__.py
--rw-r--r--   0        0        0     2667 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/shared/gitmojis.py
--rw-r--r--   0        0        0      406 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/shared/model.py
--rw-r--r--   0        0        0    10608 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/shared/spec.py
--rw-r--r--   0        0        0      817 2022-12-27 13:45:34.781631 cz_conventional_gitmoji-0.1.2/src/shared/utils.py
--rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.1.2/setup.py
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2506 2022-12-25 17:16:10.733756 cz_conventional_gitmoji-0.1.3/README.md
+-rw-r--r--   0        0        0     2371 2023-05-02 09:19:44.196072 cz_conventional_gitmoji-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       85 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/__init__.py
+-rw-r--r--   0        0        0     1285 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/conventional_gitmojis_info.txt
+-rw-r--r--   0        0        0    13515 2022-12-27 13:40:50.852366 cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/main.py
+-rw-r--r--   0        0        0        0 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/gitmojify/__init__.py
+-rw-r--r--   0        0        0     1669 2022-12-27 01:28:48.481457 cz_conventional_gitmoji-0.1.3/src/gitmojify/mojify.py
+-rw-r--r--   0        0        0        0 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/shared/__init__.py
+-rw-r--r--   0        0        0     2667 2022-12-23 22:03:29.325029 cz_conventional_gitmoji-0.1.3/src/shared/gitmojis.py
+-rw-r--r--   0        0        0      406 2022-12-22 20:59:18.556559 cz_conventional_gitmoji-0.1.3/src/shared/model.py
+-rw-r--r--   0        0        0    10608 2022-12-27 01:28:48.481457 cz_conventional_gitmoji-0.1.3/src/shared/spec.py
+-rw-r--r--   0        0        0      817 2022-12-27 01:28:48.481457 cz_conventional_gitmoji-0.1.3/src/shared/utils.py
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.1.3/PKG-INFO
```

### Comparing `cz_conventional_gitmoji-0.1.2/README.md` & `cz_conventional_gitmoji-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.2/pyproject.toml` & `cz_conventional_gitmoji-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cz-conventional-gitmoji"
-version = "0.1.2"
+version = "0.1.3"
 description = "A commitizen plugin that combines gitmoji and conventional."
 authors = ["ljnsn <82611987+ljnsn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "shared", from = "src"},
   {include = "cz_gitmoji", from = "src"},
@@ -13,50 +13,63 @@
 repository = "https://github.com/ljnsn/cz-conventional-gitmoji"
 
 [tool.poetry.scripts]
 gitmojify = "gitmojify.mojify:run"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-commitizen = "^2.38.0"
-attrs = "^22.2.0"
+commitizen = "^2.42.0"
+attrs = "^23.1.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
+black = ">=22.12,<24.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
-isort = "^5.11.4"
 coverage = {extras = ["toml"], version = "^7.0.1"}
-ruff = "^0.0.194"
+ruff = ">=0.0.246,<0.0.264"
 
 [tool.commitizen]
 name = "cz_gitmoji"
-version = "0.1.2"
+version = "0.1.3"
 bump_message = "🔖 bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 update_changelog_on_bump = true
 
 [tool.black]
-target-version = ["py37", "py38", "py39", "py310"]
-
-[tool.isort]
-profile = "black"
+target-version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.ruff]
-extend-ignore = [
+ignore = [
   # Line too long
   "E501",
   # unable to detect undefined names
   "F403",
   # may be undefined or defined from star imports
   "F405",
 ]
+fix = true
+unfixable = ["F401", "F841"]
 src = ["src", "test"]
 
+[tool.ruff.per-file-ignores]
+# ignore usage of `assert` in tests
+"*/tests/*" = ["S101"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.flake8-tidy-imports]
+# Disallow all relative imports.
+ban-relative-imports = "all"
+
+[tool.ruff.pep8-naming]
+# Allow Pydantic's `@validator` decorator to trigger class method treatment.
+classmethod-decorators = ["classmethod", "pydantic.validator"]
+
 [tool.coverage.run]
 branch = true
 parallel = true
 command_line = "--module pytest"
 data_file = "reports/.coverage"
 source = ["src"]
```

### Comparing `cz_conventional_gitmoji-0.1.2/src/cz_gitmoji/conventional_gitmojis_info.txt` & `cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/conventional_gitmojis_info.txt`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.2/src/cz_gitmoji/main.py` & `cz_conventional_gitmoji-0.1.3/src/cz_gitmoji/main.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.2/src/gitmojify/mojify.py` & `cz_conventional_gitmoji-0.1.3/src/gitmojify/mojify.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.2/src/shared/gitmojis.py` & `cz_conventional_gitmoji-0.1.3/src/shared/gitmojis.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.2/src/shared/spec.py` & `cz_conventional_gitmoji-0.1.3/src/shared/spec.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.2/src/shared/utils.py` & `cz_conventional_gitmoji-0.1.3/src/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.1.2/setup.py` & `cz_conventional_gitmoji-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,87 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cz-conventional-gitmoji
+Version: 0.1.3
+Summary: A commitizen plugin that combines gitmoji and conventional.
+Home-page: https://github.com/ljnsn/cz-conventional-gitmoji
+License: MIT
+Author: ljnsn
+Author-email: 82611987+ljnsn@users.noreply.github.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: commitizen (>=2.42.0,<3.0.0)
+Project-URL: Repository, https://github.com/ljnsn/cz-conventional-gitmoji
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src', 'cz_gitmoji': 'src/cz_gitmoji', 'gitmojify': 'src/gitmojify'}
+# cz-conventional-gitmoji
 
-packages = \
-['cz_gitmoji', 'gitmojify', 'shared']
+A [commitizen](https://github.com/commitizen-tools/commitizen) plugin that combines [gitmoji](https://gitmoji.dev/) and [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/).
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=22.2.0,<23.0.0', 'commitizen>=2.38.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['gitmojify = gitmojify.mojify:run']}
-
-setup_kwargs = {
-    'name': 'cz-conventional-gitmoji',
-    'version': '0.1.2',
-    'description': 'A commitizen plugin that combines gitmoji and conventional.',
-    'long_description': '# cz-conventional-gitmoji\n\nA [commitizen](https://github.com/commitizen-tools/commitizen) plugin that combines [gitmoji](https://gitmoji.dev/) and [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/).\n\n## Installation\n\n```bash\npoetry add cz-conventional-gitmoji\n```\n\nor with pip:\n\n```bash\npip install cz-conventional-gitmoji\n```\n\n## Usage\n\nThis package can be used as a normal `commitizen` plugin, either by specifying the name on the command line\n\n```bash\ncz --name cz_gitmoji commit\n```\n\nor by setting it in your **pyproject.toml**\n\n```toml\n[tool.commitizen]\nname = "cz_gitmoji"\n```\n\nThis will make `commitizen` use the commit message parsing rules defined by this plugin, which are 100% compatible with [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/). As such, the gitmojis are completely optional and all commands will continue to validate commit messages in conventional format just fine. This is useful if you\'re transitioning an existing repo to `contentional-gitmoji` or you work in a team in which some colleagues don\'t like gitmojis.\n\n### gitmojify\n\nApart from the conventional-gitmoji rules, this package provides the `gitmojify` command which is also available as a pre-commit hook. The command reads a commit message either from cli or a commit message file and prepends the correct gitmoji based on the type. If the message already has a gitmoji, it is returned as is.\n\n```bash\n$ gitmojify -m "init: initial version"\n🎉 init: initial version\n```\n\nTo use it as a pre-commit hook, install this packages as well as `commitizen` and put the following into your **.pre-commit-config.yaml**\n\n```yaml\nrepos:\n  - repo: https://github.com/ljnsn/cz-conventional-gitmoji\n    rev: main\n    hooks:\n      - id: conventional-gitmoji\n```\n\nCommit with a message in conventional format that contains a valid type mapped by conventional gitmoji and the gitmoji will automagically be added.\n\n## Features\n\n- [x] Enable conventional gitmoji commit messages via `cz commit`.\n- [ ] Add `--simple-emojis` option to use only the emojis relating to `cz_conventional_commits` types.\n- [ ] Add `--simple-types` option to use only the types used by `cz_conventional_commits`.\n- [ ] Add `--conventional` option to put the emoji in the commit message, making it compatible with `cz_conventional_commits`.\n- [x] Add hook to automatically prepend the appropriate gitmoji for the commit\'s type.\n\n## Inspiration\n\n- [`commitizen-emoji`](https://github.com/marcelomaia/commitizen-emoji)\n',
-    'author': 'ljnsn',
-    'author_email': '82611987+ljnsn@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ljnsn/cz-conventional-gitmoji',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## Installation
 
+```bash
+poetry add cz-conventional-gitmoji
+```
+
+or with pip:
+
+```bash
+pip install cz-conventional-gitmoji
+```
+
+## Usage
+
+This package can be used as a normal `commitizen` plugin, either by specifying the name on the command line
+
+```bash
+cz --name cz_gitmoji commit
+```
+
+or by setting it in your **pyproject.toml**
+
+```toml
+[tool.commitizen]
+name = "cz_gitmoji"
+```
+
+This will make `commitizen` use the commit message parsing rules defined by this plugin, which are 100% compatible with [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/). As such, the gitmojis are completely optional and all commands will continue to validate commit messages in conventional format just fine. This is useful if you're transitioning an existing repo to `contentional-gitmoji` or you work in a team in which some colleagues don't like gitmojis.
+
+### gitmojify
+
+Apart from the conventional-gitmoji rules, this package provides the `gitmojify` command which is also available as a pre-commit hook. The command reads a commit message either from cli or a commit message file and prepends the correct gitmoji based on the type. If the message already has a gitmoji, it is returned as is.
+
+```bash
+$ gitmojify -m "init: initial version"
+🎉 init: initial version
+```
+
+To use it as a pre-commit hook, install this packages as well as `commitizen` and put the following into your **.pre-commit-config.yaml**
+
+```yaml
+repos:
+  - repo: https://github.com/ljnsn/cz-conventional-gitmoji
+    rev: main
+    hooks:
+      - id: conventional-gitmoji
+```
+
+Commit with a message in conventional format that contains a valid type mapped by conventional gitmoji and the gitmoji will automagically be added.
+
+## Features
+
+- [x] Enable conventional gitmoji commit messages via `cz commit`.
+- [ ] Add `--simple-emojis` option to use only the emojis relating to `cz_conventional_commits` types.
+- [ ] Add `--simple-types` option to use only the types used by `cz_conventional_commits`.
+- [ ] Add `--conventional` option to put the emoji in the commit message, making it compatible with `cz_conventional_commits`.
+- [x] Add hook to automatically prepend the appropriate gitmoji for the commit's type.
+
+## Inspiration
+
+- [`commitizen-emoji`](https://github.com/marcelomaia/commitizen-emoji)
 
-setup(**setup_kwargs)
```

