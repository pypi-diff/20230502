# Comparing `tmp/ansible_vault_rotate-1.1.2.tar.gz` & `tmp/ansible_vault_rotate-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_vault_rotate-1.1.2.tar", max compression
+gzip compressed data, was "ansible_vault_rotate-2.0.0.tar", max compression
```

## Comparing `ansible_vault_rotate-1.1.2.tar` & `ansible_vault_rotate-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1069 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/LICENSE
--rw-r--r--   0        0        0     2975 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/README.md
--rw-r--r--   0        0        0       22 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/__init__.py
--rw-r--r--   0        0        0       21 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/__init__.py
--rw-r--r--   0        0        0     1828 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/cli_args.py
--rw-r--r--   0        0        0     1529 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/config.py
--rw-r--r--   0        0        0      480 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/glob.py
--rw-r--r--   0        0        0      624 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/logging.py
--rw-r--r--   0        0        0     1546 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/rotator.py
--rw-r--r--   0        0        0     1130 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/run.py
--rw-r--r--   0        0        0       60 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/match/__init__.py
--rw-r--r--   0        0        0      940 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/match/find.py
--rw-r--r--   0        0        0     1378 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/match/test_find.py
--rw-r--r--   0        0        0      179 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/__init__.py
--rw-r--r--   0        0        0      310 2023-03-23 16:54:34.401031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/detect.py
--rw-r--r--   0        0        0     1155 2023-03-23 16:54:34.405031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/file.py
--rw-r--r--   0        0        0     1727 2023-03-23 16:54:34.405031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/string.py
--rw-r--r--   0        0        0      646 2023-03-23 16:54:34.405031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/util.py
--rw-r--r--   0        0        0     1294 2023-03-23 16:54:34.405031 ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/vault_source.py
--rw-r--r--   0        0        0     1465 2023-03-23 16:54:34.405031 ansible_vault_rotate-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4071 1970-01-01 00:00:00.000000 ansible_vault_rotate-1.1.2/setup.py
--rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 ansible_vault_rotate-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-02 15:19:57.342443 ansible_vault_rotate-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2975 2023-05-02 15:19:57.342443 ansible_vault_rotate-2.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-02 15:19:57.342443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-02 15:19:57.342443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/cli_args.py
+-rw-r--r--   0        0        0     2184 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/config.py
+-rw-r--r--   0        0        0      480 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/glob.py
+-rw-r--r--   0        0        0      624 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/logging.py
+-rw-r--r--   0        0        0     1546 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/rotator.py
+-rw-r--r--   0        0        0     1570 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/run.py
+-rw-r--r--   0        0        0     3463 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/tui.py
+-rw-r--r--   0        0        0       60 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/match/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/match/find.py
+-rw-r--r--   0        0        0     1378 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/match/test_find.py
+-rw-r--r--   0        0        0      179 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/detect.py
+-rw-r--r--   0        0        0     1155 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/file.py
+-rw-r--r--   0        0        0     1727 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/string.py
+-rw-r--r--   0        0        0      646 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/util.py
+-rw-r--r--   0        0        0     1294 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/vault_source.py
+-rw-r--r--   0        0        0     1487 2023-05-02 15:19:57.346443 ansible_vault_rotate-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 ansible_vault_rotate-2.0.0/setup.py
+-rw-r--r--   0        0        0     4239 1970-01-01 00:00:00.000000 ansible_vault_rotate-2.0.0/PKG-INFO
```

### Comparing `ansible_vault_rotate-1.1.2/LICENSE` & `ansible_vault_rotate-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/README.md` & `ansible_vault_rotate-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/cli_args.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/cli_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from argparse import ArgumentParser, Namespace
 from os import getcwd
+import sys
 
 from ansible_vault_rotate import __VERSION__
 
 parser = ArgumentParser()
 parser.add_argument('--version',
                     action='version',
                     version=f'%(prog)s {__VERSION__}',
@@ -31,9 +32,13 @@
                     default=getcwd())
 parser.add_argument("--update-source-secret",
                     action="store_true",
                     help="Should the source secret be updated (not supported for text source)",
                     default=False)
 
 
+def has_cli_args():
+    return len(sys.argv) != 1
+
+
 def parse_args() -> Namespace:
     return parser.parse_args()
```

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/config.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,19 +29,32 @@
 
         return patterns
 
     def __has_arg(self, name: str) -> bool:
         return name in self.args and self.args[name] is not None
 
     def switch_to_pwd(self) -> "CliConfig":
-        if self.__has_arg("pwd"):
+        if self.has_custom_pwd():
             chdir(self.args['pwd'])
 
         return self
 
+    def has_custom_pwd(self):
+        return self.__has_arg("pwd")
+
+    def to_cli_call_string(self):
+        return "ansible-vault-rotate " + " ".join([
+            " ".join(map(lambda pattern : f"--file-glob-pattern '{pattern}'",self.file_glob_patterns)),
+            f"--old-vault-secret-source '{self.args['old_vault_secret_source']}'",
+            f"--new-vault-secret-source '{self.args['new_vault_secret_source']}'",
+            "--ignore-errors" if self.ignore_errors else "",
+            "--update-source-secret" if self.update_source_secret else "",
+            f"--pwd '{self.args['pwd']}'" if self.has_custom_pwd() else ""
+        ]).strip()
+
     def parse_vaults(self) -> "CliConfig":
         self.source_vault = build_vault_source(self.args['old_vault_secret_source'])
         self.source_vault_passphrase = self.source_vault.read()
 
         self.target_vault = build_vault_source(self.args['new_vault_secret_source'])
         self.target_vault_passphrase = self.target_vault.read()
```

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/logging.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/logging.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/rotator.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/rotator.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/cli/run.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/cli/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import sys
 import logging
 
 from .logging import FormattingConsoleLogHandler
-from .cli_args import parse_args
+from .cli_args import parse_args, has_cli_args
 from .config import CliConfig
 from .rotator import AnsibleVaultRotator
+from .tui import prompt_tui
 
 
 def run() -> None:
     """
     Entrypoint for CLI
     """
     logging.basicConfig(level=logging.INFO, handlers=[FormattingConsoleLogHandler()])
+    if has_cli_args():
+        args = parse_args()
+        args = args.__dict__
+        is_interactive = False
+    else:
+        args = prompt_tui()
+        is_interactive = True
+        print()
 
-    args = parse_args()
     logging.debug("Arguments provided: %s", args)
 
-    config = CliConfig(args.__dict__)
+    config = CliConfig(args)
     config.switch_to_pwd()
 
     try:
         config.parse_vaults()
     except Exception as e:
         logging.error("Failed to load vault sources: %s", e)
         sys.exit(2)
@@ -35,7 +43,12 @@
                  f"Errors: {rotator.error_count}, "
                  f"Rekeyed secrets: {rotator.rekey_secrets_count}, "
                  f"Rekeyed files: {rotator.rekeyed_files_count}")
 
     if config.update_source_secret:
         logging.info("Try to update source secret")
         config.source_vault.write(config.target_vault_passphrase)
+
+    if is_interactive:
+        print("")
+        print("\033[1mThe options you chose resulted in the following CLI call. You can use that for automation as well.\033[0m")
+        print(f"  \033[3m{config.to_cli_call_string()}\033[0m")
```

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/match/find.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/match/find.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/match/test_find.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/match/test_find.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/file.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/file.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/string.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/string.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/util.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/util.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/ansible_vault_rotate/vault/vault_source.py` & `ansible_vault_rotate-2.0.0/ansible_vault_rotate/vault/vault_source.py`

 * *Files identical despite different names*

### Comparing `ansible_vault_rotate-1.1.2/pyproject.toml` & `ansible_vault_rotate-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ansible-vault-rotate"
-version = "1.1.2"
+version = "2.0.0"
 description = "Advanced Python CLI to rotate the secret used for ansible vault inline secrets and files in a project"
 authors = [
     "Timo Reymann <Timo.Reymann@trustedshops.de>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/trustedshops-public/python-ansible-vault-rotate"
@@ -28,14 +28,15 @@
 include = [
     "LICENSE"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ansible-core = "^2.9.0"
+inquirerpy = "^0.3.4"
 
 [tool.poetry.scripts]
 ansible-vault-rotate = 'ansible_vault_rotate.cli.run:run'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 coverage = "^7.0.4"
```

### Comparing `ansible_vault_rotate-1.1.2/setup.py` & `ansible_vault_rotate-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
  'ansible_vault_rotate.match',
  'ansible_vault_rotate.vault']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ansible-core>=2.9.0,<3.0.0']
+['ansible-core>=2.9.0,<3.0.0', 'inquirerpy>=0.3.4,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['ansible-vault-rotate = ansible_vault_rotate.cli.run:run']}
 
 setup_kwargs = {
     'name': 'ansible-vault-rotate',
-    'version': '1.1.2',
+    'version': '2.0.0',
     'description': 'Advanced Python CLI to rotate the secret used for ansible vault inline secrets and files in a project',
     'long_description': 'python-ansible-vault-rotate\n===\n[![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://github.com/trustedshops-public/spring-boot-starter-keycloak-path-based-resolver/blob/main/LICENSE)\n[![pre-commit](https://img.shields.io/badge/%E2%9A%93%20%20pre--commit-enabled-success)](https://pre-commit.com/)\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/trustedshops-public/python-ansible-vault-rotate/tree/main.svg?style=shield&circle-token=9c1ea1cc46c804b46f457772637c8481717b511a)](https://dl.circleci.com/status-badge/redirect/gh/trustedshops-public/python-ansible-vault-rotate/tree/main)\n[![PyPI version](https://badge.fury.io/py/ansible-vault-rotate.svg)](https://pypi.org/project/ansible-vault-rotate)\n[![codecov](https://codecov.io/gh/trustedshops-public/python-ansible-vault-rotate/branch/main/graph/badge.svg?token=6PJ1GJzIcB)](https://codecov.io/gh/trustedshops-public/python-ansible-vault-rotate)\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=trustedshops-public_python-ansible-vault-rotate&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=trustedshops-public_python-ansible-vault-rotate)\n[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=trustedshops-public_python-ansible-vault-rotate&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=trustedshops-public_python-ansible-vault-rotate)\n[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=trustedshops-public_python-ansible-vault-rotate&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=trustedshops-public_python-ansible-vault-rotate)\n\nAdvanced Python CLI to rotate the secret used for ansible vault inline secrets and files in a project\n\n## Features\n\n- Reencrypt vault files\n- Reencrypt inline vaulted secrets\n\n## Installation\n\nIt is strongly recommended to use pipx instead of pip if possible:\n\n```sh\npipx install ansible-vault-rotate\n```\n\nOtherwise you can also use plain pip, but be warned that this might\ncollide with your ansible installation globally!\n\n```sh\npip install ansible-vault-rotate\n```\n\n## Usage\n\n### Rekey given vault secret with new secret specified on CLI\n\n```sh\nansible-vault-rotate --old-vault-secret-source file://my-vault-password \\\n                     --new-vault-secret-source my-new-secret \\\n                     --update-source-secret\n```\n\n## Rekey only specific files (e.g. when using multiple keys per stage)\n\n```sh\nansible-vault-rotate --old-vault-secret-source file://my-vault-password-<stage> \\\n                     --new-vault-secret-source my-new-secret \\\n                     --file-glob-pattern group_vars/<stage>/*.yml \\\n                     --update-source-secret\n```\n\n## Getting help about all args\n\n```sh\nansible-vault-rotate --help\n```\n\n## Development\n\nFor development, you will need:\n\n- Python 3.9 or greater\n- Poetry\n\n### Install\n\n```\npoetry install\n```\n\n### Run tests\n\n```\npoetry run pytest\n```\n',
     'author': 'Timo Reymann',
     'author_email': 'Timo.Reymann@trustedshops.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/trustedshops-public/python-ansible-vault-rotate',
```

### Comparing `ansible_vault_rotate-1.1.2/PKG-INFO` & `ansible_vault_rotate-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-vault-rotate
-Version: 1.1.2
+Version: 2.0.0
 Summary: Advanced Python CLI to rotate the secret used for ansible vault inline secrets and files in a project
 Home-page: https://github.com/trustedshops-public/python-ansible-vault-rotate
 License: MIT
 Author: Timo Reymann
 Author-email: Timo.Reymann@trustedshops.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansible-core (>=2.9.0,<3.0.0)
+Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Project-URL: Bug Tracker, https://github.com/trustedshops-public/python-ansible-vault-rotate/issues
 Project-URL: Repository, https://github.com/trustedshops-public/python-ansible-vault-rotate
 Description-Content-Type: text/markdown
 
 python-ansible-vault-rotate
 ===
 [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://github.com/trustedshops-public/spring-boot-starter-keycloak-path-based-resolver/blob/main/LICENSE)
```

