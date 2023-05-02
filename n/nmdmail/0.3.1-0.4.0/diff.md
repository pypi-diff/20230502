# Comparing `tmp/nmdmail-0.3.1.tar.gz` & `tmp/nmdmail-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmdmail-0.3.1.tar", max compression
+gzip compressed data, was "nmdmail-0.4.0.tar", max compression
```

## Comparing `nmdmail-0.3.1.tar` & `nmdmail-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1281 2023-02-05 11:42:46.217450 nmdmail-0.3.1/LICENSE
--rw-r--r--   0        0        0     5619 2023-02-05 11:42:46.217450 nmdmail-0.3.1/README.md
--rw-r--r--   0        0        0       73 2023-02-05 11:42:46.217450 nmdmail-0.3.1/nmdmail/__init__.py
--rw-r--r--   0        0        0     4905 2023-02-05 11:42:46.217450 nmdmail-0.3.1/nmdmail/api.py
--rwxr-xr-x   0        0        0     2643 2023-02-05 11:42:46.217450 nmdmail-0.3.1/nmdmail/cli.py
--rw-r--r--   0        0        0      901 2023-02-05 11:42:46.217450 nmdmail-0.3.1/nmdmail/default.css
--rw-r--r--   0        0        0      711 2023-02-05 11:42:46.217450 nmdmail-0.3.1/nmdmail/helpers.py
--rw-r--r--   0        0        0        0 2023-02-05 11:42:46.217450 nmdmail-0.3.1/nmdmail/py.typed
--rw-r--r--   0        0        0     1009 2023-02-05 11:42:46.217450 nmdmail-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 nmdmail-0.3.1/setup.py
--rw-r--r--   0        0        0     6648 1970-01-01 00:00:00.000000 nmdmail-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1281 2023-05-02 11:29:36.768328 nmdmail-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5624 2023-05-02 11:29:36.768328 nmdmail-0.4.0/README.md
+-rw-r--r--   0        0        0       73 2023-05-02 11:29:36.768328 nmdmail-0.4.0/nmdmail/__init__.py
+-rw-r--r--   0        0        0     4930 2023-05-02 11:29:36.768328 nmdmail-0.4.0/nmdmail/api.py
+-rwxr-xr-x   0        0        0     2685 2023-05-02 11:29:36.768328 nmdmail-0.4.0/nmdmail/cli.py
+-rw-r--r--   0        0        0      901 2023-05-02 11:29:36.768328 nmdmail-0.4.0/nmdmail/default.css
+-rw-r--r--   0        0        0      697 2023-05-02 11:29:36.768328 nmdmail-0.4.0/nmdmail/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:29:36.768328 nmdmail-0.4.0/nmdmail/py.typed
+-rw-r--r--   0        0        0     1354 2023-05-02 11:29:36.768328 nmdmail-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6603 1970-01-01 00:00:00.000000 nmdmail-0.4.0/PKG-INFO
```

### Comparing `nmdmail-0.3.1/LICENSE` & `nmdmail-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nmdmail-0.3.1/README.md` & `nmdmail-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 Fork of https://github.com/yejianye/mdmail, which looks dead.
 
 [![PyPI version](https://badge.fury.io/py/nmdmail.svg)](https://pypi.org/project/nmdmail)
 [![Tests](https://github.com/nim65s/nmdmail/actions/workflows/test.yml/badge.svg)](https://github.com/nim65s/nmdmail/actions/workflows/test.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nim65s/nmdmail/main.svg)](https://results.pre-commit.ci/latest/github/nim65s/nmdmail/main)
 [![codecov](https://codecov.io/gh/nim65s/nmdmail/branch/main/graph/badge.svg?token=BLGISGCYKG)](https://codecov.io/gh/nim65s/nmdmail)
-[![Maintainability](https://api.codeclimate.com/v1/badges/6737a84239590ddc0d1e/maintainability)](https://codeclimate.com/github/nim65s/nmdmail/maintainability)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 
 nMdmail sends emails written in Markdown. It could be used as a standalone command-line script or as a python module. The features includes
 
 - Have a sane default CSS style and support CSS customization
 - Support local images as inline images
```

### Comparing `nmdmail-0.3.1/nmdmail/api.py` & `nmdmail-0.4.0/nmdmail/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from bs4 import BeautifulSoup  # type: ignore
 
 from nmdmail.helpers import sanitize_email_address
 
 
 class EmailContent:
     def __init__(self, content, css=None, image_root="."):
-        """Constructor
+        """Constructor.
 
         Args:
+        ----
             content (str): Markdown text
             css (str): Custom CSS style. If not set, use default CSS style.
             image_root (str): Root directory for inline images.
         """
         self._md = markdown.Markdown(
-            extensions=["markdown.extensions.tables", "markdown.extensions.meta"]
+            extensions=["markdown.extensions.tables", "markdown.extensions.meta"],
         )
         self._html = None
         self._inline_images = None
         self._convert(content, css, image_root)
 
     def _replace_inline_images(self, html, image_root):
         soup = BeautifulSoup(html, "lxml")
@@ -95,17 +96,18 @@
     from_email: Optional[str] = None,
     to_email: Optional[Union[str, List[str]]] = None,
     cc: Optional[Union[str, List[str]]] = None,
     bcc: Optional[Union[str, List[str]]] = None,
     reply_to: Optional[str] = None,
     smtp: Optional[Dict[str, str]] = None,
 ):
-    """Send markdown email
+    """Send markdown email.
 
     Args:
+    ----
         email (str/obj): A markdown string or EmailContent object
         subject (str): subject line
         from_email (str): sender email address
         to_email (str/list): recipient email addresses
         cc (str/list): CC email addresses (string or a list)
         bcc (str/list): BCC email addresses (string or a list)
         reply_to (str): Reply-to email address
```

### Comparing `nmdmail-0.3.1/nmdmail/cli.py` & `nmdmail-0.4.0/nmdmail/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #!/usr/bin/env python
-"""Send email written in Markdown.
-"""
+"""Send email written in Markdown."""
 
 import os
 import sys
 from argparse import ArgumentParser, RawTextHelpFormatter
 
 import nmdmail
 from nmdmail.helpers import to_bool
 
 
 def main(cli_args=None):
     parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
     parser.add_argument(
-        "file", nargs="?", help="Markdown file for email content. " "Default to STDIN."
+        "file",
+        nargs="?",
+        help="Markdown file for email content. " "Default to STDIN.",
     )
     parser.add_argument("--subject", "-s", help="Subject line")
     parser.add_argument("--from", "-f", dest="from_", help="From address")
     parser.add_argument("--to", "-t", help="To addresses, separated by comma")
     parser.add_argument("--cc", "-c", help="CC addresses, separated by comma")
     parser.add_argument("--bcc", "-b", help="Bcc address, separated by comma")
     parser.add_argument("--reply-to", "-r", help="Reply-to address")
     parser.add_argument("--css", help="Use a custom CSS file")
     parser.add_argument(
-        "--print-only", "-p", action="store_true", help="Only print out rendered html"
+        "--print-only",
+        "-p",
+        action="store_true",
+        help="Only print out rendered html",
     )
     if cli_args:
         args = parser.parse_args(cli_args)
     else:
         args = parser.parse_args()
 
     if args.file:
@@ -44,15 +48,15 @@
     else:
         css = None
 
     email_content = nmdmail.EmailContent(content, css=css, image_root=image_root)
 
     if not args.from_:
         from_email = email_content.headers.get("from") or os.environ.get(
-            "MDMAIL_DEFAULT_SENDER"
+            "MDMAIL_DEFAULT_SENDER",
         )
     else:
         from_email = args.from_
 
     smtp = {
         "host": os.environ.get("MDMAIL_HOST", "localhost"),
         "port": int(os.environ.get("MDMAIL_PORT", 25)),
```

### Comparing `nmdmail-0.3.1/nmdmail/default.css` & `nmdmail-0.4.0/nmdmail/default.css`

 * *Files identical despite different names*

### Comparing `nmdmail-0.3.1/nmdmail/helpers.py` & `nmdmail-0.4.0/nmdmail/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
     address = address.strip()
 
     match = re.match("^(.*)<(.*)>$", address)
     if match:
         name, address = match.groups()
         return name.strip(), address.strip()
-    else:
-        return address
+    return address
 
 
 def to_bool(val) -> bool:
     if isinstance(val, str):
         return val.lower() in ("1", "true", "yes", "y")
     return bool(val)
```

### Comparing `nmdmail-0.3.1/pyproject.toml` & `nmdmail-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,63 @@
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
+
+[tool.black]
+target-version = ['py38']
+
+[tool.coverage.run]
+source = ["nmdmail"]
+
+[tool.isort]
+profile = "black"
+
 [tool.poetry]
-name = "nmdmail"
-version = "0.3.1"
-description = "Send emails written in Markdown"
 authors = [
-    "Guilhem Saurel <guilhem.saurel@laas.fr>",
-    "Jianye Ye <yejianye@gmail.com>"
+  "Guilhem Saurel <guilhem.saurel@laas.fr>",
+  "Jianye Ye <yejianye@gmail.com>"
 ]
+description = "Send emails written in Markdown"
+homepage = 'https://github.com/nim65s/nmdmail'
+keywords = ['email', 'html', 'inline css', 'markdown']
 license = "BSD-2-Clause"
+name = "nmdmail"
 readme = "README.md"
-keywords = ['markdown', 'html', 'email', 'inline css']
-homepage = 'https://github.com/nim65s/nmdmail'
 repository = "https://github.com/nim65s/nmdmail.git"
-
-[tool.poetry.urls]
-changelog = "https://github.com/nim65s/nmdmail/blob/main/CHANGELOG.md"
-
-[tool.poetry.scripts]
-nmdmail = 'nmdmail.cli:main'
+version = "0.4.0"
 
 [tool.poetry.dependencies]
-python = "^3.7"
 Markdown = "^3.4.1"
-premailer = "^3.10.0"
+beautifulsoup4 = "^4.11.1"
 emails = "^0.6"
 lxml = "^4.9.1"
-beautifulsoup4 = "^4.11.1"
+premailer = "^3.10.0"
+python = "^3.8"
+
+[tool.poetry.group.tests]
+optional = true
 
 [tool.poetry.group.tests.dependencies]
-mock = "^4.0.3"
-coverage = "^6.5.0"
+coverage = {extras = ["toml"], version = "^7.2.5"}
+mock = "^5.0.2"
+
+[tool.poetry.group.tools]
+optional = true
 
 [tool.poetry.group.tools.dependencies]
-black = "^22.10.0"
+black = "^23.3.0"
+mypy = "^1.2.0"
 pyupgrade = "^3.1.0"
 types-markdown = "^3.4.2.1"
-mypy = "^0.982"
 
-[tool.black]
-target-version = ['py37']
+[tool.poetry.scripts]
+nmdmail = 'nmdmail.cli:main'
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry.urls]
+changelog = "https://github.com/nim65s/nmdmail/blob/main/CHANGELOG.md"
+
+[tool.ruff]
+extend-select = ["A", "B", "C", "COM", "EM", "EXE", "G", "N", "RET", "RUF", "UP", "W", "YTT"]
+target-version = "py38"
+
+[tool.tomlsort]
+all = true
```

### Comparing `nmdmail-0.3.1/setup.py` & `nmdmail-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,206 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['nmdmail']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Markdown>=3.4.1,<4.0.0',
- 'beautifulsoup4>=4.11.1,<5.0.0',
- 'emails>=0.6,<0.7',
- 'lxml>=4.9.1,<5.0.0',
- 'premailer>=3.10.0,<4.0.0']
-
-entry_points = \
-{'console_scripts': ['nmdmail = nmdmail.cli:main']}
-
-setup_kwargs = {
-    'name': 'nmdmail',
-    'version': '0.3.1',
-    'description': 'Send emails written in Markdown',
-    'long_description': '# nMdmail: Send emails written in Markdown\n\nFork of https://github.com/yejianye/mdmail, which looks dead.\n\n[![PyPI version](https://badge.fury.io/py/nmdmail.svg)](https://pypi.org/project/nmdmail)\n[![Tests](https://github.com/nim65s/nmdmail/actions/workflows/test.yml/badge.svg)](https://github.com/nim65s/nmdmail/actions/workflows/test.yml)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nim65s/nmdmail/main.svg)](https://results.pre-commit.ci/latest/github/nim65s/nmdmail/main)\n[![codecov](https://codecov.io/gh/nim65s/nmdmail/branch/main/graph/badge.svg?token=BLGISGCYKG)](https://codecov.io/gh/nim65s/nmdmail)\n[![Maintainability](https://api.codeclimate.com/v1/badges/6737a84239590ddc0d1e/maintainability)](https://codeclimate.com/github/nim65s/nmdmail/maintainability)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\nnMdmail sends emails written in Markdown. It could be used as a standalone command-line script or as a python module. The features includes\n\n- Have a sane default CSS style and support CSS customization\n- Support local images as inline images\n\nScreenshot of an email sent via nmdmail viewed in Google Inbox\n\n<img src="screenshot.png" height="640"></img>\n\nTo install nmdmail\n\n```bash\n$ python -m pip install nmdmail\n```\n\n## Send Email in Command-line\n\nWhen sending emails from command-line, the body of the email could be read from a file or stdin.\n\nEmail headers such as subject, from/to, cc etc could be specified at the beginning of the markdown file, Or be specified in command-line arguments.\n\nHere is an example of Markdown file with email headers\n\n```\nSubject: Sample Email\nFrom: foo@xyz.com\nTo: bar@xyz.com\nCc: baz@xyz.com\n\n# Sample Email\n\n-\n\n![Embed local image](../assets/image.jpg)\n```\n\nTo send this email with nmdmail\n\n```bash\n$ nmdmail sample_email.md\n```\n\nHere is an example of specifying subject, from/to in command-line\n\n```bash\n$ nmdmail --from=foo@xyz.com --to=bar@xyz.com --subject=\'Sample\' sample_email.md\n```\n\nTo read email content from stdin,\n\n```bash\n$ echo \'# Sample Email\' | nmdmail --from=foo@xyz.com --to=bar@xyz.com --subject=\'Sample\'\n```\n\nSMTP server configurations are read from the following environment variables\n\n```bash\nexport MDMAIL_HOST="" # default: localhost\nexport MDMAIL_PORT="" # default: 25\nexport MDMAIL_USE_TLS="" # default: false\nexport MDMAIL_USE_SSL="" # default: false\nexport MDMAIL_USERNAME="" # default: None\nexport MDMAIL_PASSWORD="" # default: None\nexport MDMAIL_DEFAULT_SENDER="" # default: None\n```\n\nFull help of `nmdmail` command-line script\n\n```bash\nusage: nmdmail [-h] [--subject SUBJECT] [--from FROM_] [--to TO] [--cc CC]\n               [--bcc BCC] [--reply-to REPLY_TO] [--css CSS] [--print-only]\n               [file]\n\nSend email written in Markdown.\n\npositional arguments:\n  file                  Markdown file for email content. Default to STDIN.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --subject SUBJECT, -s SUBJECT\n                        Subject line\n  --from FROM, -f FROM\n                        From address\n  --to TO, -t TO        To addresses, separated by comma\n  --cc CC, -c CC        CC address, separated by comma\n  --bcc BCC, -b BCC     Bcc address, separated by comma\n  --reply-to REPLY_TO, -r REPLY_TO\n                        Reply-to address\n  --css CSS             Use a custom CSS file\n  --print-only, -p      Only print out rendered html\n```\n\n## Send Email in Python Code\n\nSending emails in python is straight-forward.\n\n```python\nimport nmdmail\n\nemail="""\n# Sample Email\n\n- Python is awesome\n- Markdown is cool\n\n![Embed local image](../assets/image.jpg)\n"""\n\nnmdmail.send(email, subject=\'Sample Email\',\n            from_email=\'foo@example.com\', to_email=\'bar@example.com\')\n```\n\nBy default, it will use SMTP server on localhost. You could specify a SMTP server as well.\n\n```python\n# Specify SMTP server\nsmtp = {\n  \'host: \'my-mailserver.com\',\n  \'port\': 25,\n  \'tls\': False,\n  \'ssl\': False,\n  \'user: \'\',\n  \'password\': \'\',\n}\n\nnmdmail.send(content,\n             subject=\'Sample Email\',\n             from_email=\'foo@example.com\',\n             to_email=\'bar@example.com\',\n             smtp=smtp)\n```\n\n\n### API documentation `nmdmail.send`\n\n- **email** (str/obj): A markdown string or EmailContent object\n- **subject** (str): subject line\n- **from_email** (str): sender email address\n- **to_email** (str/list): recipient email addresses\n- **cc** (str/list): CC email addresses (string or a list)\n- **bcc** (str/list): BCC email addresses (string or a list)\n- **reply_to** (str): Reply-to email address\n- **smtp** (dict): SMTP configuration with following keys\n    - *host* (str): SMTP server host. Default: localhost\n    - *port* (int): SMTP server port. Default: 25\n    - *tls* (bool): Use TLS. Default: False\n    - *ssl* (bool): Use SSL. Default: False\n    - *user* (bool): SMTP login user. Default empty\n    - *password* (bool): SMTP login password. Default empty\n\n## Use nmdmail with Vim and Emacs\n\nSince `nmdmail` can read from stdin and support email headers such as subject/from/to in the markdown file itself,\nintegrating nmdmail with Vim, Emacs or other text editors is easy.\n\nTo use nmdmail in Vim, just write a markdown email with headers, and then execute `w !nmdmail` command, which will send\ncurrent buffer as stdin to nmdmail.\n\nIn Emacs, you could write a small function to do the same thing\n\n```lisp\n(defun nmdmail-send-buffer ()\n  (interactive)\n  (shell-command-on-region (point-min) (point-max) "nmdmail"))\n```\n\nThen `M-x nmdmail-send-buffer` will send current buffer to nmdmail.\n',
-    'author': 'Guilhem Saurel',
-    'author_email': 'guilhem.saurel@laas.fr',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nim65s/nmdmail',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+Metadata-Version: 2.1
+Name: nmdmail
+Version: 0.4.0
+Summary: Send emails written in Markdown
+Home-page: https://github.com/nim65s/nmdmail
+License: BSD-2-Clause
+Keywords: email,html,inline css,markdown
+Author: Guilhem Saurel
+Author-email: guilhem.saurel@laas.fr
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Markdown (>=3.4.1,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: emails (>=0.6,<0.7)
+Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: premailer (>=3.10.0,<4.0.0)
+Project-URL: Repository, https://github.com/nim65s/nmdmail.git
+Project-URL: changelog, https://github.com/nim65s/nmdmail/blob/main/CHANGELOG.md
+Description-Content-Type: text/markdown
+
+# nMdmail: Send emails written in Markdown
+
+Fork of https://github.com/yejianye/mdmail, which looks dead.
+
+[![PyPI version](https://badge.fury.io/py/nmdmail.svg)](https://pypi.org/project/nmdmail)
+[![Tests](https://github.com/nim65s/nmdmail/actions/workflows/test.yml/badge.svg)](https://github.com/nim65s/nmdmail/actions/workflows/test.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nim65s/nmdmail/main.svg)](https://results.pre-commit.ci/latest/github/nim65s/nmdmail/main)
+[![codecov](https://codecov.io/gh/nim65s/nmdmail/branch/main/graph/badge.svg?token=BLGISGCYKG)](https://codecov.io/gh/nim65s/nmdmail)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+
+
+nMdmail sends emails written in Markdown. It could be used as a standalone command-line script or as a python module. The features includes
+
+- Have a sane default CSS style and support CSS customization
+- Support local images as inline images
+
+Screenshot of an email sent via nmdmail viewed in Google Inbox
+
+<img src="screenshot.png" height="640"></img>
+
+To install nmdmail
+
+```bash
+$ python -m pip install nmdmail
+```
+
+## Send Email in Command-line
+
+When sending emails from command-line, the body of the email could be read from a file or stdin.
+
+Email headers such as subject, from/to, cc etc could be specified at the beginning of the markdown file, Or be specified in command-line arguments.
+
+Here is an example of Markdown file with email headers
+
+```
+Subject: Sample Email
+From: foo@xyz.com
+To: bar@xyz.com
+Cc: baz@xyz.com
+
+# Sample Email
+
+-
+
+![Embed local image](../assets/image.jpg)
+```
+
+To send this email with nmdmail
+
+```bash
+$ nmdmail sample_email.md
+```
+
+Here is an example of specifying subject, from/to in command-line
+
+```bash
+$ nmdmail --from=foo@xyz.com --to=bar@xyz.com --subject='Sample' sample_email.md
+```
+
+To read email content from stdin,
+
+```bash
+$ echo '# Sample Email' | nmdmail --from=foo@xyz.com --to=bar@xyz.com --subject='Sample'
+```
+
+SMTP server configurations are read from the following environment variables
+
+```bash
+export MDMAIL_HOST="" # default: localhost
+export MDMAIL_PORT="" # default: 25
+export MDMAIL_USE_TLS="" # default: false
+export MDMAIL_USE_SSL="" # default: false
+export MDMAIL_USERNAME="" # default: None
+export MDMAIL_PASSWORD="" # default: None
+export MDMAIL_DEFAULT_SENDER="" # default: None
+```
+
+Full help of `nmdmail` command-line script
+
+```bash
+usage: nmdmail [-h] [--subject SUBJECT] [--from FROM_] [--to TO] [--cc CC]
+               [--bcc BCC] [--reply-to REPLY_TO] [--css CSS] [--print-only]
+               [file]
+
+Send email written in Markdown.
+
+positional arguments:
+  file                  Markdown file for email content. Default to STDIN.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --subject SUBJECT, -s SUBJECT
+                        Subject line
+  --from FROM, -f FROM
+                        From address
+  --to TO, -t TO        To addresses, separated by comma
+  --cc CC, -c CC        CC address, separated by comma
+  --bcc BCC, -b BCC     Bcc address, separated by comma
+  --reply-to REPLY_TO, -r REPLY_TO
+                        Reply-to address
+  --css CSS             Use a custom CSS file
+  --print-only, -p      Only print out rendered html
+```
+
+## Send Email in Python Code
+
+Sending emails in python is straight-forward.
+
+```python
+import nmdmail
+
+email="""
+# Sample Email
+
+- Python is awesome
+- Markdown is cool
+
+![Embed local image](../assets/image.jpg)
+"""
+
+nmdmail.send(email, subject='Sample Email',
+            from_email='foo@example.com', to_email='bar@example.com')
+```
+
+By default, it will use SMTP server on localhost. You could specify a SMTP server as well.
+
+```python
+# Specify SMTP server
+smtp = {
+  'host: 'my-mailserver.com',
+  'port': 25,
+  'tls': False,
+  'ssl': False,
+  'user: '',
+  'password': '',
 }
 
+nmdmail.send(content,
+             subject='Sample Email',
+             from_email='foo@example.com',
+             to_email='bar@example.com',
+             smtp=smtp)
+```
+
+
+### API documentation `nmdmail.send`
+
+- **email** (str/obj): A markdown string or EmailContent object
+- **subject** (str): subject line
+- **from_email** (str): sender email address
+- **to_email** (str/list): recipient email addresses
+- **cc** (str/list): CC email addresses (string or a list)
+- **bcc** (str/list): BCC email addresses (string or a list)
+- **reply_to** (str): Reply-to email address
+- **smtp** (dict): SMTP configuration with following keys
+    - *host* (str): SMTP server host. Default: localhost
+    - *port* (int): SMTP server port. Default: 25
+    - *tls* (bool): Use TLS. Default: False
+    - *ssl* (bool): Use SSL. Default: False
+    - *user* (bool): SMTP login user. Default empty
+    - *password* (bool): SMTP login password. Default empty
+
+## Use nmdmail with Vim and Emacs
+
+Since `nmdmail` can read from stdin and support email headers such as subject/from/to in the markdown file itself,
+integrating nmdmail with Vim, Emacs or other text editors is easy.
+
+To use nmdmail in Vim, just write a markdown email with headers, and then execute `w !nmdmail` command, which will send
+current buffer as stdin to nmdmail.
+
+In Emacs, you could write a small function to do the same thing
+
+```lisp
+(defun nmdmail-send-buffer ()
+  (interactive)
+  (shell-command-on-region (point-min) (point-max) "nmdmail"))
+```
+
+Then `M-x nmdmail-send-buffer` will send current buffer to nmdmail.
 
-setup(**setup_kwargs)
```

