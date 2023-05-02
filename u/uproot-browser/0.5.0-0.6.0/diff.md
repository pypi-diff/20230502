# Comparing `tmp/uproot_browser-0.5.0.tar.gz` & `tmp/uproot_browser-0.6.0.tar.gz`

## Comparing `uproot_browser-0.5.0.tar` & `uproot_browser-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,37 @@
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/noxfile.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/docs/make_logo.py
--rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/docs/_images/iterm.png
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/docs/_images/uproot-browser-logo.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/_version.pyi
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/dirs.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/exceptions.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/plot.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/plot_mpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/py.typed
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/__init__.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/browser.css
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/browser.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/left_panel.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/src/uproot_browser/tui/right_panel.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/tests/test_dirs.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/tests/test_printouts.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/LICENSE
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/README.md
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 uproot_browser-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/noxfile.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/docs/make_logo.py
+-rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/docs/_images/iterm.png
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/docs/_images/uproot-browser-logo.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/_version.pyi
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/dirs.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/exceptions.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/plot.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/plot_mpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/py.typed
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/_compat/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/_compat/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/browser.css
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/browser.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/header.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/help.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/left_panel.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/src/uproot_browser/tui/right_panel.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/tests/test_dirs.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/tests/test_printouts.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/README.md
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 uproot_browser-0.6.0/PKG-INFO
```

### Comparing `uproot_browser-0.5.0/.pre-commit-config.yaml` & `uproot_browser-0.6.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: "v0.0.262"
+  rev: "v0.0.263"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: v1.2.0
   hooks:
```

### Comparing `uproot_browser-0.5.0/noxfile.py` & `uproot_browser-0.6.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/.github/CONTRIBUTING.md` & `uproot_browser-0.6.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/.github/workflows/ci.yml` & `uproot_browser-0.6.0/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -50,17 +50,14 @@
 
     - name: Test package
       run: python -m pytest -ra
 
   pass:
     if: always()
     needs: [checks]
-    environment: pypi
-    permissions:
-      id-token: write
     runs-on: ubuntu-latest
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
           jobs: ${{ toJSON(needs) }}
 
@@ -78,9 +75,23 @@
     - uses: actions/upload-artifact@v3
       with:
         path: dist
 
     - name: Check products
       run: pipx run twine check dist/*
 
+  publish:
+    name: Publish
+    environment: pypi
+    permissions:
+      id-token: write
+    needs: [dist]
+    if: github.event_name == 'release' && github.event.action == 'published'
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/download-artifact@v3
+      with:
+        path: dist
+        name: archive
+
     - uses: pypa/gh-action-pypi-publish@v1.8.5
-      if: github.event_name == 'release' && github.event.action == 'published'
```

### Comparing `uproot_browser-0.5.0/docs/make_logo.py` & `uproot_browser-0.6.0/docs/make_logo.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/docs/_images/iterm.png` & `uproot_browser-0.6.0/docs/_images/iterm.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/docs/_images/uproot-browser-logo.png` & `uproot_browser-0.6.0/docs/_images/uproot-browser-logo.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/src/uproot_browser/__main__.py` & `uproot_browser-0.6.0/src/uproot_browser/__main__.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/src/uproot_browser/dirs.py` & `uproot_browser-0.6.0/src/uproot_browser/dirs.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/src/uproot_browser/plot.py` & `uproot_browser-0.6.0/src/uproot_browser/plot.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/src/uproot_browser/plot_mpl.py` & `uproot_browser-0.6.0/src/uproot_browser/plot_mpl.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/src/uproot_browser/tree.py` & `uproot_browser-0.6.0/src/uproot_browser/tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,25 @@
 Display tools for TTrees.
 """
 
 from __future__ import annotations
 
 import dataclasses
 import functools
-import sys
 from pathlib import Path
 from typing import Any
 
 import uproot
 import uproot.reading
 from rich.console import Console
 from rich.markup import escape
 from rich.text import Text
 from rich.tree import Tree
 
-if sys.version_info < (3, 8):
-    from typing_extensions import TypedDict
-else:
-    from typing import TypedDict
+from ._compat.typing import TypedDict
 
 console = Console()
 
 __all__ = (
     "make_tree",
     "process_item",
     "print_tree",
```

### Comparing `uproot_browser-0.5.0/src/uproot_browser/tui/browser.css` & `uproot_browser-0.6.0/src/uproot_browser/tui/browser.css`

 * *Files 18% similar despite different names*

```diff
@@ -60,7 +60,25 @@
     background: $secondary-darken-3;
     text-style: bold;
 }
 
 Footer{
     background: $secondary;
 }
+
+HelpScreen {
+    align: center middle;
+}
+
+.dialog {
+    padding: 0 1;
+    width: 80%;
+    height: 90%;
+    border: thick $background 80%;
+    background: $surface;
+}
+
+#help-buttons {
+    align: right middle;
+    height: 3;
+    background: $surface-lighten-1;
+}
```

### Comparing `uproot_browser-0.5.0/src/uproot_browser/tui/browser.py` & `uproot_browser-0.6.0/src/uproot_browser/tui/browser.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sys
 from pathlib import Path
 from typing import Any
 
 import plotext as plt
 import rich.syntax
 import textual.app
+import textual.binding
 import textual.containers
 import textual.events
 import textual.widgets
 from textual.reactive import var
 
 with contextlib.suppress(AttributeError):
     light_background = 0xF5, 0xF5, 0xF5
@@ -30,14 +31,16 @@
     # pylint: disable-next=protected-access
     plt._dict.themes["dark"][1] = dark_background
     # pylint: disable-next=protected-access
     plt._dict.themes["dark"][2] = dark_text
 
 from uproot_browser.exceptions import EmptyTreeError
 
+from .header import Header
+from .help import HelpScreen
 from .left_panel import UprootSelected, UprootTree
 from .right_panel import (
     EmptyWidget,
     Error,
     ErrorWidget,
     LogoWidget,
     Plotext,
@@ -47,70 +50,77 @@
 
 
 class Browser(textual.app.App[None]):
     """A basic implementation of the uproot-browser TUI"""
 
     CSS_PATH = "browser.css"
     BINDINGS = [
-        ("b", "toggle_files", "Toggle sidebar"),
-        ("q", "quit", "Quit"),
-        ("d", "quit_with_dump", "Quit with dump"),
-        ("t", "toggle_theme", "Toggle light/dark theme"),
+        textual.binding.Binding("b", "toggle_files", "Navbar"),
+        textual.binding.Binding("q", "quit", "Quit"),
+        textual.binding.Binding("d", "quit_with_dump", "Dump & Quit"),
+        textual.binding.Binding("t", "toggle_theme", "Theme"),
+        textual.binding.Binding("f1", "help", "Help"),
+        textual.binding.Binding("?", "help", "Help", show=False),
     ]
 
     show_tree = var(True)
 
-    def watch_show_tree(self, show_tree: bool) -> None:
-        """Called when show_tree is modified."""
-        self.set_class(show_tree, "-show-tree")
-
     def __init__(self, path: Path, **kwargs: Any) -> None:
         self.path = path
         super().__init__(**kwargs)
 
-        # self.uptree = UprootTree(self.path)
+        self.plot_widget = PlotWidget(id="plot")
+        self.error_widget = ErrorWidget(id="error")
 
     def compose(self) -> textual.app.ComposeResult:
         """Compose our UI."""
-        yield textual.widgets.Header()
+        yield Header("uproot-browser")
         with textual.containers.Container():
             # left_panel
             yield UprootTree(self.path, id="tree-view")
             # right_panel
             yield textual.widgets.ContentSwitcher(
                 LogoWidget(id="logo"),
-                PlotWidget(id="plot"),
-                ErrorWidget(id="error"),
+                self.plot_widget,
+                self.error_widget,
                 EmptyWidget(id="empty"),
                 id="main-view",
                 initial="logo",
             )
         yield textual.widgets.Footer()
 
     def on_mount(self, _event: textual.events.Mount) -> None:
         self.query_one("#tree-view", UprootTree).focus()
 
+    def watch_show_tree(self, show_tree: bool) -> None:
+        """Called when show_tree is modified."""
+        self.set_class(show_tree, "-show-tree")
+
+    def action_help(self) -> None:
+        self.push_screen(HelpScreen())
+
     def action_toggle_files(self) -> None:
         """Called in response to key binding."""
         self.show_tree = not self.show_tree
 
     def action_quit_with_dump(self) -> None:
         """Dump the current state of the application."""
 
         content_switcher = self.query_one("#main-view", textual.widgets.ContentSwitcher)
-        plot_widget = content_switcher.query_one("#plot", PlotWidget)
         err_widget = content_switcher.query_one("#error", ErrorWidget)
 
         msg = f'\nimport uproot\nuproot_file = uproot.open("{self.path}")'
 
         items: list[Plotext | Error] = []
         if content_switcher.current == "plot":
-            assert plot_widget.item
-            msg += f'\nitem = uproot_file["{plot_widget.item.selection.lstrip("/")}"]'
-            items = [plot_widget.item]
+            assert self.plot_widget.item
+            msg += (
+                f'\nitem = uproot_file["{self.plot_widget.item.selection.lstrip("/")}"]'
+            )
+            items = [self.plot_widget.item]
         elif content_switcher.current == "error":
             assert err_widget.exc
             items = [err_widget.exc]
 
         theme = "rrt" if self.dark else "default"
 
         results = rich.console.Group(
@@ -119,40 +129,36 @@
         )
 
         self.exit(message=results)
 
     def action_toggle_theme(self) -> None:
         """An action to toggle dark mode."""
         self.dark = not self.dark
-        content_switcher = self.query_one("#main-view", textual.widgets.ContentSwitcher)
-        plot_widget = content_switcher.query_one("#plot", PlotWidget)
-        if plot_widget.item:
-            plot_widget.item.theme = "dark" if self.dark else "default"
-            plot_widget.refresh()
+        if self.plot_widget.item:
+            self.plot_widget.item.theme = "dark" if self.dark else "default"
+            self.plot_widget.refresh()
 
     def on_uproot_selected(self, message: UprootSelected) -> None:
         """A message sent by the tree when a file is clicked."""
 
         content_switcher = self.query_one("#main-view", textual.widgets.ContentSwitcher)
 
         try:
             theme = "dark" if self.dark else "default"
             make_plot(message.upfile[message.path], theme, 20)
-            plot_widget = content_switcher.query_one("#plot", PlotWidget)
-            plot_widget.item = Plotext(message.upfile, message.path, theme)
+            self.plot_widget.item = Plotext(message.upfile, message.path, theme)
             content_switcher.current = "plot"
 
         except EmptyTreeError:
             content_switcher.current = "empty"
 
         except Exception:
-            error_widget = content_switcher.query_one("#error", ErrorWidget)
             exc = sys.exc_info()
             assert exc[1]
-            error_widget.exc = Error(exc)
+            self.error_widget.exc = Error(exc)
             content_switcher.current = "error"
 
 
 if __name__ in {"<run_path>", "__main__"}:
     import uproot_browser.dirs
 
     fname = uproot_browser.dirs.filename(
```

### Comparing `uproot_browser-0.5.0/src/uproot_browser/tui/right_panel.py` & `uproot_browser-0.6.0/src/uproot_browser/tui/right_panel.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/tests/test_printouts.py` & `uproot_browser-0.6.0/tests/test_printouts.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/.gitignore` & `uproot_browser-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/LICENSE` & `uproot_browser-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.5.0/README.md` & `uproot_browser-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 **`browse` command:**
 
 ```bash
 uproot-browser browse ../scikit-hep-testdata/src/skhep_testdata/data/uproot-Event.root
 ```
 
-![GIF of the TUI functionality](https://github.com/scikit-hep/uproot-browser/releases/download/v0.3.0/tui.gif)
+![GIF of the TUI functionality](https://github.com/scikit-hep/uproot-browser/releases/download/v0.5.0/tui.gif)
 
 **`plot` command:**
 
 ```bash
 uproot-browser plot ../scikit-hep-testdata/src/skhep_testdata/data/uproot-Event.root:hstat
                         hstat -- Entries: 1000
     ┌───────────────────────────────────────────────────────────────┐
```

### Comparing `uproot_browser-0.5.0/pyproject.toml` & `uproot_browser-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -33,24 +33,25 @@
   "Programming Language :: Python :: 3.11",
   "Development Status :: 4 - Beta",
   "Typing :: Typed",
 ]
 
 dynamic = ["version"]
 dependencies = [
-  "awkward >=1",
-  "click >=8",
-  "lz4",
-  "numpy >=1.13.3",
-  "rich >=12.0.0",
-  "uproot >=4.2.1",
-  "plotext >=5.2.2",
-  "hist >=2.4",
-  "textual >=0.18.0",
-  'typing_extensions; python_version<"3.8"'
+  'awkward >=1',
+  'click >=8',
+  'hist >=2.4',
+  'importlib_resources; python_version<"3.9"',
+  'lz4',
+  'numpy >=1.13.3',
+  'plotext >=5.2.2',
+  'rich >=12.0.0',
+  'textual >=0.18.0',
+  'typing_extensions; python_version<"3.8"',
+  'uproot >=4.2.1',
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "scikit-hep-testdata",
 ]
@@ -147,14 +148,15 @@
     "E501",
     "E722",
     "RUF001",  # Unicode chars
     "PLR",
 ]
 target-version = "py37"
 src = ["src"]
+typing-modules = ["uproot_browser._compat.typing"]
 unfixable = [
   "T20",    # Removes print statements
   "F841",   # Removes unused variables
   "SIM118", # Dict .keys() removal (uproot)
 ]
 exclude = []
```

### Comparing `uproot_browser-0.5.0/PKG-INFO` & `uproot_browser-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uproot_browser
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools to inspect ROOT files with uproot
 Project-URL: homepage, https://github.com/scikit-hep/uproot-browser
 Project-URL: repository, https://github.com/scikit-hep/uproot-browser
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -50,14 +50,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: awkward>=1
 Requires-Dist: click>=8
 Requires-Dist: hist>=2.4
+Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: lz4
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: plotext>=5.2.2
 Requires-Dist: rich>=12.0.0
 Requires-Dist: textual>=0.18.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: uproot>=4.2.1
@@ -118,15 +119,15 @@
 
 **`browse` command:**
 
 ```bash
 uproot-browser browse ../scikit-hep-testdata/src/skhep_testdata/data/uproot-Event.root
 ```
 
-![GIF of the TUI functionality](https://github.com/scikit-hep/uproot-browser/releases/download/v0.3.0/tui.gif)
+![GIF of the TUI functionality](https://github.com/scikit-hep/uproot-browser/releases/download/v0.5.0/tui.gif)
 
 **`plot` command:**
 
 ```bash
 uproot-browser plot ../scikit-hep-testdata/src/skhep_testdata/data/uproot-Event.root:hstat
                         hstat -- Entries: 1000
     ┌───────────────────────────────────────────────────────────────┐
```

