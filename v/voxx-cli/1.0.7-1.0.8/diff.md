# Comparing `tmp/voxx-cli-1.0.7.tar.gz` & `tmp/voxx-cli-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxx-cli-1.0.7.tar", last modified: Mon May  1 07:55:29 2023, max compression
+gzip compressed data, was "voxx-cli-1.0.8.tar", last modified: Tue May  2 08:48:00 2023, max compression
```

## Comparing `voxx-cli-1.0.7.tar` & `voxx-cli-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.015932 voxx-cli-1.0.7/
--rw-rw-rw-   0        0        0     1084 2023-05-01 07:55:29.015932 voxx-cli-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-04-30 08:19:16.000000 voxx-cli-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 07:55:29.016433 voxx-cli-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-04-30 04:35:11.000000 voxx-cli-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.006422 voxx-cli-1.0.7/voxx/
--rw-rw-rw-   0        0        0      140 2023-05-01 07:53:35.000000 voxx-cli-1.0.7/voxx/__init__.py
--rw-rw-rw-   0        0        0     3330 2023-04-30 08:05:30.000000 voxx-cli-1.0.7/voxx/__main__.py
--rw-rw-rw-   0        0        0     4065 2023-05-01 07:51:28.000000 voxx-cli-1.0.7/voxx/connection.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.007422 voxx-cli-1.0.7/voxx/css/
--rw-rw-rw-   0        0        0     1247 2023-05-01 06:48:14.000000 voxx-cli-1.0.7/voxx/css/tui.css
--rw-rw-rw-   0        0        0     2333 2023-04-30 00:51:11.000000 voxx-cli-1.0.7/voxx/model.py
--rw-rw-rw-   0        0        0     6441 2023-05-01 07:38:19.000000 voxx-cli-1.0.7/voxx/tui.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:55:29.014933 voxx-cli-1.0.7/voxx_cli.egg-info/
--rw-rw-rw-   0        0        0     1084 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       29 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-01 07:55:28.000000 voxx-cli-1.0.7/voxx_cli.egg-info/top_level.txt
+drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-05-02 08:48:00.331745 voxx-cli-1.0.8/
+-rw-r--r--   0 cyr1en     (501) staff       (20)     1042 2023-05-02 08:48:00.331290 voxx-cli-1.0.8/PKG-INFO
+-rw-r--r--   0 cyr1en     (501) staff       (20)      596 2023-04-30 17:00:35.000000 voxx-cli-1.0.8/README.md
+-rw-r--r--   0 cyr1en     (501) staff       (20)       38 2023-05-02 08:48:00.332023 voxx-cli-1.0.8/setup.cfg
+-rw-r--r--   0 cyr1en     (501) staff       (20)     1456 2023-04-30 17:00:35.000000 voxx-cli-1.0.8/setup.py
+drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-05-02 08:48:00.325187 voxx-cli-1.0.8/voxx/
+-rw-r--r--   0 cyr1en     (501) staff       (20)      136 2023-05-02 08:47:11.000000 voxx-cli-1.0.8/voxx/__init__.py
+-rw-r--r--   0 cyr1en     (501) staff       (20)     3238 2023-04-30 17:00:35.000000 voxx-cli-1.0.8/voxx/__main__.py
+-rw-r--r--   0 cyr1en     (501) staff       (20)     4590 2023-05-02 08:22:05.000000 voxx-cli-1.0.8/voxx/connection.py
+drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-05-02 08:48:00.326295 voxx-cli-1.0.8/voxx/css/
+-rw-r--r--   0 cyr1en     (501) staff       (20)     1173 2023-04-30 17:59:12.000000 voxx-cli-1.0.8/voxx/css/tui.css
+-rw-r--r--   0 cyr1en     (501) staff       (20)     2247 2023-04-30 17:00:35.000000 voxx-cli-1.0.8/voxx/model.py
+-rw-r--r--   0 cyr1en     (501) staff       (20)     6278 2023-05-02 08:22:05.000000 voxx-cli-1.0.8/voxx/tui.py
+drwxr-xr-x   0 cyr1en     (501) staff       (20)        0 2023-05-02 08:48:00.330653 voxx-cli-1.0.8/voxx_cli.egg-info/
+-rw-r--r--   0 cyr1en     (501) staff       (20)     1042 2023-05-02 08:48:00.000000 voxx-cli-1.0.8/voxx_cli.egg-info/PKG-INFO
+-rw-r--r--   0 cyr1en     (501) staff       (20)      308 2023-05-02 08:48:00.000000 voxx-cli-1.0.8/voxx_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 cyr1en     (501) staff       (20)       29 2023-05-02 08:48:00.000000 voxx-cli-1.0.8/voxx_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 cyr1en     (501) staff       (20)       48 2023-05-02 08:48:00.000000 voxx-cli-1.0.8/voxx_cli.egg-info/entry_points.txt
+-rw-r--r--   0 cyr1en     (501) staff       (20)       29 2023-05-02 08:48:00.000000 voxx-cli-1.0.8/voxx_cli.egg-info/requires.txt
+-rw-r--r--   0 cyr1en     (501) staff       (20)        5 2023-05-02 08:48:00.000000 voxx-cli-1.0.8/voxx_cli.egg-info/top_level.txt
```

### Comparing `voxx-cli-1.0.7/setup.py` & `voxx-cli-1.0.8/setup.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from setuptools import setup, find_packages
-from io import open
-from os import path
-from voxx import __app_name__, __description__, __author__, __voxx_version__
-import pathlib
-
-HERE = pathlib.Path(__file__).parent
-
-README = (HERE / "README.md").read_text()
-
-with open(path.join(HERE, 'requirements.txt'), encoding='utf-8') as f:
-    all_reqs = f.read().split('\n')
-
-install_requires = [x.strip() for x in all_reqs if
-                    ('git+' not in x) and (not x.startswith('#')) and (not x.startswith('-'))]
-dependency_links = [x.strip().replace('git+', '') for x in all_reqs if 'git+' not in x]
-
-setup(
-    name=__app_name__,
-    description=__description__,
-    version=__voxx_version__,
-    packages=find_packages(),  # list of all packages
-    install_requires=install_requires,
-    python_requires='>=3.7',  # any python greater than 2.7
-    package_data={'voxx': ['css/*.css']},
-    entry_points=f'''
-        [console_scripts]
-        {__app_name__}=voxx.__main__:main
-    ''',
-    author=__author__,
-    keyword="voxx",
-    long_description=README,
-    long_description_content_type="text/markdown",
-    license='MIT',
-    url='https://github.com/CyR1en/voxx-client-cli',
-    download_url='https://github.com/CyR1en/voxx-client-cli',
-    dependency_links=dependency_links,
-    author_email='ethan.bacurio@ucdenver.edu',
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
-    ]
-)
+from setuptools import setup, find_packages
+from io import open
+from os import path
+from voxx import __app_name__, __description__, __author__, __voxx_version__
+import pathlib
+
+HERE = pathlib.Path(__file__).parent
+
+README = (HERE / "README.md").read_text()
+
+with open(path.join(HERE, 'requirements.txt'), encoding='utf-8') as f:
+    all_reqs = f.read().split('\n')
+
+install_requires = [x.strip() for x in all_reqs if
+                    ('git+' not in x) and (not x.startswith('#')) and (not x.startswith('-'))]
+dependency_links = [x.strip().replace('git+', '') for x in all_reqs if 'git+' not in x]
+
+setup(
+    name=__app_name__,
+    description=__description__,
+    version=__voxx_version__,
+    packages=find_packages(),  # list of all packages
+    install_requires=install_requires,
+    python_requires='>=3.7',  # any python greater than 2.7
+    package_data={'voxx': ['css/*.css']},
+    entry_points=f'''
+        [console_scripts]
+        {__app_name__}=voxx.__main__:main
+    ''',
+    author=__author__,
+    keyword="voxx",
+    long_description=README,
+    long_description_content_type="text/markdown",
+    license='MIT',
+    url='https://github.com/CyR1en/voxx-client-cli',
+    download_url='https://github.com/CyR1en/voxx-client-cli',
+    dependency_links=dependency_links,
+    author_email='ethan.bacurio@ucdenver.edu',
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
+    ]
+)
```

### Comparing `voxx-cli-1.0.7/voxx/__main__.py` & `voxx-cli-1.0.8/voxx/__main__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import argparse
-import re
-import sys
-
-from rich import box
-from rich.box import Box
-from rich.console import Group
-from rich.panel import Panel
-from rich.table import Table
-from rich.text import Text
-
-from voxx.connection import console, close
-from voxx.connection import establish_voxx_connection
-from voxx.tui import start_tui
-from voxx import __voxx_version__, __app_name__, __description__
-
-UNAME_RE = r'^[A-Za-z][A-Za-z0-9_]{3,6}$'
-ADDR_RE = r'(.*):(\d+)'
-
-EMPTY: Box = Box(
-    """\
-    
-    
-    
-    
-    
-    
-    
-    
-"""
-)
-
-
-class VoxxParser(argparse.ArgumentParser):
-    def _print_message(self, message, file=None):
-        console.print(message)
-
-    def format_help(self):
-        out: str
-        table = Table(box=EMPTY,
-                      show_header=False,
-                      show_lines=False,
-                      pad_edge=False)
-
-        table.add_column(min_width=1)
-        table.add_column(min_width=25)
-        table.add_column(min_width=10)
-
-        for action in self._actions:
-            metavar = action.metavar if action.metavar else ''
-            table.add_row(f'[aquamarine1]{action.option_strings[0]}[/aquamarine1]',
-                          f'[cyan3]{action.option_strings[1]}[/cyan3] [gold3]{metavar}[/gold3]',
-                          f'[bright_black]{action.help}[/bright_black]')
-
-        group = Group(
-            Text.assemble('Voxx CLI ', (f'v{__voxx_version__}', 'bold magenta'), justify='center', end='\n\n'),
-            Text.assemble((f'{__description__}', 'bright_black'), justify='center', end='\n\n'),
-            Text.assemble(f' Usage: {__app_name__} [options] ', (f'<arg>', 'bold gold3'), justify='left', end='\n\n'),
-            Panel.fit(table, title='options', title_align='left', border_style='bright_black')
-        )
-        return Panel.fit(group, box=EMPTY)
-
-
-parser = VoxxParser(prog='voxx-cli', description=__description__)
-parser.add_argument('-a', '--address', metavar='ADDRESS', type=str, help='voxx server address',
-                    default='localhost:8008')
-parser.add_argument('-u', '--user', metavar='USERNAME', type=str, help='username to register as', required=True)
-parser.add_argument('-v', '--version', action='version',
-                    version=f'[bold magenta]{__app_name__}[/bold magenta] version {__voxx_version__}')
-
-
-def main():
-    args = parser.parse_args()
-    addr = args.a if hasattr(args, 'a') else args.address
-    user = args.u if hasattr(args, 'u') else args.user
-    if not re.match(ADDR_RE, addr):
-        console.print(f'[warning]Invalid address: [bold red]{args.addr}[/bold red][/warning]')
-        console.print(f'[italic]Address must be in the form of [bold green]host:port[/bold green][/italic]')
-        sys.exit(1)
-    if not re.match(UNAME_RE, user):
-        console.print(f'[warning]Invalid username: [bold red]{args.user}[/bold red][/warning]')
-        console.print(f'[italic]Username must be 4-7 characters long and start with a letter[/italic]')
-        sys.exit(1)
-    with console.status("[bold green]Connecting to server...") as status:
-        addr = tuple(addr.split(':'))
-        establish_voxx_connection(args.user, (addr[0], int(addr[1])))
-    start_tui()
-    close()
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import re
+import sys
+
+from rich import box
+from rich.box import Box
+from rich.console import Group
+from rich.panel import Panel
+from rich.table import Table
+from rich.text import Text
+
+from voxx.connection import console, close
+from voxx.connection import establish_voxx_connection
+from voxx.tui import start_tui
+from voxx import __voxx_version__, __app_name__, __description__
+
+UNAME_RE = r'^[A-Za-z][A-Za-z0-9_]{3,6}$'
+ADDR_RE = r'(.*):(\d+)'
+
+EMPTY: Box = Box(
+    """\
+    
+    
+    
+    
+    
+    
+    
+    
+"""
+)
+
+
+class VoxxParser(argparse.ArgumentParser):
+    def _print_message(self, message, file=None):
+        console.print(message)
+
+    def format_help(self):
+        out: str
+        table = Table(box=EMPTY,
+                      show_header=False,
+                      show_lines=False,
+                      pad_edge=False)
+
+        table.add_column(min_width=1)
+        table.add_column(min_width=25)
+        table.add_column(min_width=10)
+
+        for action in self._actions:
+            metavar = action.metavar if action.metavar else ''
+            table.add_row(f'[aquamarine1]{action.option_strings[0]}[/aquamarine1]',
+                          f'[cyan3]{action.option_strings[1]}[/cyan3] [gold3]{metavar}[/gold3]',
+                          f'[bright_black]{action.help}[/bright_black]')
+
+        group = Group(
+            Text.assemble('Voxx CLI ', (f'v{__voxx_version__}', 'bold magenta'), justify='center', end='\n\n'),
+            Text.assemble((f'{__description__}', 'bright_black'), justify='center', end='\n\n'),
+            Text.assemble(f' Usage: {__app_name__} [options] ', (f'<arg>', 'bold gold3'), justify='left', end='\n\n'),
+            Panel.fit(table, title='options', title_align='left', border_style='bright_black')
+        )
+        return Panel.fit(group, box=EMPTY)
+
+
+parser = VoxxParser(prog='voxx-cli', description=__description__)
+parser.add_argument('-a', '--address', metavar='ADDRESS', type=str, help='voxx server address',
+                    default='localhost:8008')
+parser.add_argument('-u', '--user', metavar='USERNAME', type=str, help='username to register as', required=True)
+parser.add_argument('-v', '--version', action='version',
+                    version=f'[bold magenta]{__app_name__}[/bold magenta] version {__voxx_version__}')
+
+
+def main():
+    args = parser.parse_args()
+    addr = args.a if hasattr(args, 'a') else args.address
+    user = args.u if hasattr(args, 'u') else args.user
+    if not re.match(ADDR_RE, addr):
+        console.print(f'[warning]Invalid address: [bold red]{args.addr}[/bold red][/warning]')
+        console.print(f'[italic]Address must be in the form of [bold green]host:port[/bold green][/italic]')
+        sys.exit(1)
+    if not re.match(UNAME_RE, user):
+        console.print(f'[warning]Invalid username: [bold red]{args.user}[/bold red][/warning]')
+        console.print(f'[italic]Username must be 4-7 characters long and start with a letter[/italic]')
+        sys.exit(1)
+    with console.status("[bold green]Connecting to server...") as status:
+        addr = tuple(addr.split(':'))
+        establish_voxx_connection(args.user, (addr[0], int(addr[1])))
+    start_tui()
+    close()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `voxx-cli-1.0.7/voxx/css/tui.css` & `voxx-cli-1.0.8/voxx/css/tui.css`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-Screen {
-    background: $panel;
-}
-
-MessageBar {
-    height: auto;
-    content-align: left middle;
-    padding: 1;
-    margin: 2;
-    background: $boost;
-    color: $text;
-    border: round #2966cd;
-}
-
-NotificationBar {
-    height: auto;
-    content-align: center middle;
-    padding: 0;
-    margin: 2;
-    background: $boost;
-    color: $secondary;
-    border: hkey #2966cd;
-}
-
-NotificationBar .message {
-    margin: 0 1 0 1;
-    content-align: center middle;
-    color: $secondary;
-}
-
-MessageBar .message {
-    margin: 0 1 0 1;
-    color: #9caccc;
-}
-
-Input {
-    dock: bottom;
-    width: 100%;
-    height: 1;
-    padding: 0 1;
-    margin: 0 1 2 1;
-}
-
-Footer {
-    background: $surface-lighten-1;
-    color: $panel-lighten-3;
-}
-
-Footer > .footer--highlight {
-    background: $surface;
-}
-
-Footer > .footer--highlight-key {
-    background: $secondary;
-    text-style: none;
-}
-
-Footer > .footer--key {
-    text-style: bold;
-    color: $panel-lighten-3;
-    background: $surface;
-}
-
-#results {
-    width: auto;
-    min-height: 100%;
-}
-
-#results-container {
-    background: $background 50%;
-    overflow: auto;
-    margin: 1 2;
-    height: 100%;
-    border: tall #7f8ca6 50%;
+Screen {
+    background: $panel;
+}
+
+MessageBar {
+    height: auto;
+    content-align: left middle;
+    padding: 1;
+    margin: 2;
+    background: $boost;
+    color: $text;
+    border: round #2966cd;
+}
+
+NotificationBar {
+    height: auto;
+    content-align: center middle;
+    padding: 0;
+    margin: 2;
+    background: $boost;
+    color: $secondary;
+    border: hkey #2966cd;
+}
+
+NotificationBar .message {
+    margin: 0 1 0 1;
+    content-align: center middle;
+    color: $secondary;
+}
+
+MessageBar .message {
+    margin: 0 1 0 1;
+    color: #9caccc;
+}
+
+Input {
+    dock: bottom;
+    width: 100%;
+    height: 1;
+    padding: 0 1;
+    margin: 0 1 2 1;
+}
+
+Footer {
+    background: $surface-lighten-1;
+    color: $panel-lighten-3;
+}
+
+Footer > .footer--highlight {
+    background: $surface;
+}
+
+Footer > .footer--highlight-key {
+    background: $secondary;
+    text-style: none;
+}
+
+Footer > .footer--key {
+    text-style: bold;
+    color: $panel-lighten-3;
+    background: $surface;
+}
+
+#results {
+    width: auto;
+    min-height: 100%;
+}
+
+#results-container {
+    background: $background 50%;
+    overflow: auto;
+    margin: 1 2;
+    height: 100%;
+    border: tall #7f8ca6 50%;
 }
```

