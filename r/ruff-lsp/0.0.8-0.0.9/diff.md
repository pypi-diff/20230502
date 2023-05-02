# Comparing `tmp/ruff-lsp-0.0.8.tar.gz` & `tmp/ruff-lsp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruff-lsp-0.0.8.tar", max compression
+gzip compressed data, was "ruff-lsp-0.0.9.tar", max compression
```

## Comparing `ruff-lsp-0.0.8.tar` & `ruff-lsp-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2022-12-23 03:38:56.251890 ruff-lsp-0.0.8/LICENSE
--rw-r--r--   0        0        0     6971 2022-12-23 03:38:56.251890 ruff-lsp-0.0.8/README.md
--rw-r--r--   0        0        0     1809 2022-12-23 03:38:56.251890 ruff-lsp-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      169 2022-12-23 03:38:56.251890 ruff-lsp-0.0.8/ruff_lsp/__init__.py
--rw-r--r--   0        0        0      364 2022-12-23 03:38:56.255890 ruff-lsp-0.0.8/ruff_lsp/__main__.py
--rw-r--r--   0        0        0        0 2022-12-23 03:38:56.255890 ruff-lsp-0.0.8/ruff_lsp/py.typed
--rwxr-xr-x   0        0        0    25246 2022-12-23 03:38:56.255890 ruff-lsp-0.0.8/ruff_lsp/server.py
--rw-r--r--   0        0        0     2494 2022-12-23 03:38:56.255890 ruff-lsp-0.0.8/ruff_lsp/utils.py
--rw-r--r--   0        0        0     8093 2022-12-23 03:39:08.036735 ruff-lsp-0.0.8/setup.py
--rw-r--r--   0        0        0     8332 2022-12-23 03:39:08.037635 ruff-lsp-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2381 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7394 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/README.md
+-rw-r--r--   0        0        0     2007 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      169 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/ruff_lsp/__init__.py
+-rw-r--r--   0        0        0      364 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/ruff_lsp/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/ruff_lsp/py.typed
+-rwxr-xr-x   0        0        0    25241 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/ruff_lsp/server.py
+-rw-r--r--   0        0        0     2494 2022-12-24 02:43:21.504221 ruff-lsp-0.0.9/ruff_lsp/utils.py
+-rw-r--r--   0        0        0     8525 2022-12-24 02:43:34.151327 ruff-lsp-0.0.9/setup.py
+-rw-r--r--   0        0        0     8806 2022-12-24 02:43:34.152151 ruff-lsp-0.0.9/PKG-INFO
```

### Comparing `ruff-lsp-0.0.8/LICENSE` & `ruff-lsp-0.0.9/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Charlie Marsh
+Copyright (c) 2022 Charles Marsh
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -15,7 +15,35 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
+The externally maintained libraries from which parts of the Software is derived
+are:
+
+- vscode-python-tools-extension-template, licensed as follows:
+  """
+    MIT License
+
+    # TODO: Copyright (c) Microsoft Corporation.
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+    SOFTWARE
+  """
```

### Comparing `ruff-lsp-0.0.8/README.md` & `ruff-lsp-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,23 @@
 config = { settings = { args = [] } }
 ```
 
 Upon successful installation, you should see errors surfaced directly in your editor:
 
 ![](https://user-images.githubusercontent.com/1309177/209262106-71e34f8d-73cc-4889-89f7-3f54a4481c52.png)
 
+### Example: Lapce
+
+To use `ruff-lsp` with [Lapce](https://lapce.dev/), install the [`lapce-ruff-lsp`](https://plugins.lapce.dev/plugins/abreumatheus/lapce-ruff-lsp)
+plugin (which wraps `ruff-lsp`) from the Lapce plugins panel.
+
+Upon successful installation, you should see errors surfaced directly in your editor:
+
+![](https://user-images.githubusercontent.com/1309177/209418462-ae106d1f-dbc3-4d53-bae2-66bfccc3e841.png)
+
 ## Settings
 
 The exact mechanism by which settings will be passed to `ruff-lsp` will vary by editor. However,
 the following settings are supported:
 
 | Settings         | Default | Description                                                                              |
 |------------------|---------|------------------------------------------------------------------------------------------|
```

### Comparing `ruff-lsp-0.0.8/pyproject.toml` & `ruff-lsp-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ruff-lsp"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Language Server Protocol implementation for Ruff."
 authors = ["Charlie Marsh <charlie.r.marsh@gmail.com>"]
 maintainers = ["Charlie Marsh <charlie.r.marsh@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/charliermarsh/ruff-lsp"
 keywords = ["ruff", "lsp", "language-server", "language-server-protocol", "python"]
@@ -17,14 +17,15 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities",
 ]
@@ -37,36 +38,41 @@
 pygls = ">1.0.0a3"
 ruff = ">0.0.150"
 typing_extensions = "*"
 
 [tool.poetry.dev-dependencies]
 black = "==22.12.0"
 mypy = "==0.991"
+python-jsonrpc-server = "==0.4.0"
 
 [tool.ruff]
 line-length = 88
 select = [
     "E",
     "F",
     "W",
     "Q",
     "UP",
     "I",
     "N",
 ]
 target-version = "py37"
+extend-exclude = ["tests/data"]
 
 [tool.black]
 line-length = 88
+extend-exclude = "tests/data"
 
 [tool.mypy]
-files = "ruff_lsp"
+files = ["ruff_lsp", "tests"]
+exclude = "tests/data"
 no_implicit_optional = true
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = [
     "debugpy.*",
     "lsprotocol.*",
     "pygls.*",
+    "pyls_jsonrpc.*",
 ]
 ignore_missing_imports = true
```

### Comparing `ruff-lsp-0.0.8/ruff_lsp/server.py` & `ruff-lsp-0.0.9/ruff_lsp/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Implementation of the LSP server for Ruff."""
 
+
 from __future__ import annotations
 
 import copy
 import json
 import os
 import pathlib
 import re
@@ -511,15 +512,15 @@
 ###
 
 
 @LSP_SERVER.feature(INITIALIZE)
 def initialize(params: InitializeParams) -> None:
     """LSP handler for initialize request."""
     # Extract `settings` from the initialization options.
-    user_settings = params.initialization_options.get(  # type: ignore[attr-defined]
+    user_settings = (params.initialization_options or {}).get(  # type: ignore
         "settings",
     )
     if isinstance(user_settings, dict):
         # In Sublime Text, Neovim, and probably others, we're passed a single
         # `settings`, which we'll treat as defaults for any future files.
         USER_DEFAULTS.update(user_settings)
         settings = [user_settings]
```

### Comparing `ruff-lsp-0.0.8/ruff_lsp/utils.py` & `ruff-lsp-0.0.9/ruff_lsp/utils.py`

 * *Files identical despite different names*

### Comparing `ruff-lsp-0.0.8/setup.py` & `ruff-lsp-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['pygls>1.0.0a3', 'ruff>0.0.150', 'typing_extensions']
 
 entry_points = \
 {'console_scripts': ['ruff-lsp = ruff_lsp.__main__:main']}
 
 setup_kwargs = {
     'name': 'ruff-lsp',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A Language Server Protocol implementation for Ruff.',
-    'long_description': '# ruff-lsp\n\nA [Language Server Protocol](https://microsoft.github.io/language-server-protocol/) implementation for\n[Ruff](https://github.com/charliermarsh/ruff), an extremely fast Python linter and code transformation\ntool, written in Rust.\n\nEnables Ruff to be used in any editor that supports the LSP, including [Neovim](#example-neovim),\n[Sublime Text](#example-sublime-text), Emacs and more.\n\nFor Visual Studio Code, check out the [Ruff VS Code extension](https://github.com/charliermarsh/ruff-vscode).\n\n## Highlights\n\n### "Quick Fix" actions for auto-fixable violations (like unused imports)\n\n![](https://user-images.githubusercontent.com/1309177/205176932-44cfc03a-120f-4bad-b710-612bdd7765d6.gif)\n\n### "Fix all": automatically fix all auto-fixable violations\n\n![](https://user-images.githubusercontent.com/1309177/205175763-cf34871d-5c05-4abf-9916-440afc82dbf8.gif)\n\n### "Organize Imports": `isort`-compatible import sorting\n\n![](https://user-images.githubusercontent.com/1309177/205175987-82e23e21-14bb-467d-9ef0-027f24b75865.gif)\n\n## Installation and Usage\n\n`ruff-lsp` is available as [`ruff-lsp`](https://pypi.org/project/ruff-lsp/) on PyPI:\n\n```shell\npip install ruff-lsp\n```\n\nFrom there, `ruff-lsp` can be used with any editor that supports the Language Server Protocol,\nincluding Neovim, Emacs, Sublime Text, and more.\n\n### Example: Neovim\n\nFor example, to use `ruff-lsp` with Neovim, install `ruff-lsp` from PyPI along with\n[`nvim-lspconfig`](https://github.com/neovim/nvim-lspconfig). Then, add something like the following\nto your `init.lua`:\n\n```lua\n-- See: https://github.com/neovim/nvim-lspconfig/tree/54eb2a070a4f389b1be0f98070f81d23e2b1a715#suggested-configuration\nlocal opts = { noremap=true, silent=true }\nvim.keymap.set(\'n\', \'<space>e\', vim.diagnostic.open_float, opts)\nvim.keymap.set(\'n\', \'[d\', vim.diagnostic.goto_prev, opts)\nvim.keymap.set(\'n\', \']d\', vim.diagnostic.goto_next, opts)\nvim.keymap.set(\'n\', \'<space>q\', vim.diagnostic.setloclist, opts)\n\n-- Use an on_attach function to only map the following keys\n-- after the language server attaches to the current buffer\nlocal on_attach = function(client, bufnr)\n  -- Enable completion triggered by <c-x><c-o>\n  vim.api.nvim_buf_set_option(bufnr, \'omnifunc\', \'v:lua.vim.lsp.omnifunc\')\n\n  -- Mappings.\n  -- See `:help vim.lsp.*` for documentation on any of the below functions\n  local bufopts = { noremap=true, silent=true, buffer=bufnr }\n  vim.keymap.set(\'n\', \'gD\', vim.lsp.buf.declaration, bufopts)\n  vim.keymap.set(\'n\', \'gd\', vim.lsp.buf.definition, bufopts)\n  vim.keymap.set(\'n\', \'K\', vim.lsp.buf.hover, bufopts)\n  vim.keymap.set(\'n\', \'gi\', vim.lsp.buf.implementation, bufopts)\n  vim.keymap.set(\'n\', \'<C-k>\', vim.lsp.buf.signature_help, bufopts)\n  vim.keymap.set(\'n\', \'<space>wa\', vim.lsp.buf.add_workspace_folder, bufopts)\n  vim.keymap.set(\'n\', \'<space>wr\', vim.lsp.buf.remove_workspace_folder, bufopts)\n  vim.keymap.set(\'n\', \'<space>wl\', function()\n    print(vim.inspect(vim.lsp.buf.list_workspace_folders()))\n  end, bufopts)\n  vim.keymap.set(\'n\', \'<space>D\', vim.lsp.buf.type_definition, bufopts)\n  vim.keymap.set(\'n\', \'<space>rn\', vim.lsp.buf.rename, bufopts)\n  vim.keymap.set(\'n\', \'<space>ca\', vim.lsp.buf.code_action, bufopts)\n  vim.keymap.set(\'n\', \'gr\', vim.lsp.buf.references, bufopts)\n  vim.keymap.set(\'n\', \'<space>f\', function() vim.lsp.buf.format { async = true } end, bufopts)\nend\n\n-- Configure `ruff-lsp`.\nlocal configs = require \'lspconfig.configs\'\nif not configs.ruff_lsp then\n  configs.ruff_lsp = {\n    default_config = {\n      cmd = { \'ruff-lsp\' },\n      filetypes = { \'python\' },\n      root_dir = require(\'lspconfig\').util.find_git_ancestor,\n      init_options = {\n        settings = {\n          args = {}\n        }\n      } \n    }\n  }\nend\nrequire(\'lspconfig\').ruff_lsp.setup {\n  on_attach = on_attach,\n}\n```\n\nUpon successful installation, you should see Ruff\'s diagnostics surfaced directly in your editor:\n\n![Code Actions available in Neovim](https://user-images.githubusercontent.com/1309177/208278707-25fa37e4-079d-4597-ad35-b95dba066960.png)\n\nRuff also integrates with [`coc.nvim`](https://github.com/neoclide/coc.nvim/wiki/Language-servers#using-ruff-lsp):\n\n```json\n"languageserver": {\n  "ruff-lsp": {\n    "command": "ruff-lsp",\n    "filetypes": ["python"]\n  }\n}\n```\n\n### Example: Sublime Text\n\nTo use `ruff-lsp` with Sublime Text, install Sublime Text\'s [LSP](https://github.com/sublimelsp/LSP)\npackage, then add something like the following to `LSP.sublime-settings`:\n\n```json\n{\n  "clients": {\n    "ruff-lsp": {\n      "command": ["ruff-lsp"],\n      "enabled": true,\n      "selector": "source.python",\n      "initializationOptions": {\n        "settings": {\n          "args": []\n        }\n      }\n    }\n  }\n}\n```\n\nUpon successful installation, you should see errors surfaced directly in your editor:\n\n![Code Actions available in Sublime Text](https://user-images.githubusercontent.com/1309177/208266375-331ad8e5-8ac1-4735-bca8-07734eb38536.png)\n\n### Example: Helix\n\nTo use `ruff-lsp` with [Helix](https://helix-editor.com/), add something like the following to\n`~/.config/helix/languages.toml`:\n\n```toml\n[[language]]\nname = "python"\nscope = "source.python"\nlanguage-server = { command = "ruff-lsp" }\nconfig = { settings = { args = [] } }\n```\n\nUpon successful installation, you should see errors surfaced directly in your editor:\n\n![](https://user-images.githubusercontent.com/1309177/209262106-71e34f8d-73cc-4889-89f7-3f54a4481c52.png)\n\n## Settings\n\nThe exact mechanism by which settings will be passed to `ruff-lsp` will vary by editor. However,\nthe following settings are supported:\n\n| Settings         | Default | Description                                                                              |\n|------------------|---------|------------------------------------------------------------------------------------------|\n| args             | `[]`    | Custom arguments passed to `ruff`. E.g `"args": ["--config=/path/to/pyproject.toml"]`.   |\n| logLevel         | `error` | Sets the tracing level for the extension.                                                |\n| path             | `[]`    | Setting to provide custom `ruff` executables, to try in order. E.g. `["/path/to/ruff"]`. |\n| interpreter      | `[]`    | Path to a Python interpreter to use to run the linter server.                            |\n| showNotification | `off`   | Setting to control when a notification is shown.                                         |\n| organizeImports  | `true`  | Whether to register Ruff as capable of handling `source.organizeImports` actions.        |\n| fixAll           | `true`  | Whether to register Ruff as capable of handling `source.fixAll` actions.                 |\n\n## Development\n\n`ruff-lsp` uses Poetry for environment management and packaging. To get started, clone the\nrepository, install Poetry, and run `poetry install`.\n\nTo automatically format the codebase, run: `make format`.\n\nTo run lint and type checks, run: `make check`.\n\n## License\n\nMIT\n',
+    'long_description': '# ruff-lsp\n\nA [Language Server Protocol](https://microsoft.github.io/language-server-protocol/) implementation for\n[Ruff](https://github.com/charliermarsh/ruff), an extremely fast Python linter and code transformation\ntool, written in Rust.\n\nEnables Ruff to be used in any editor that supports the LSP, including [Neovim](#example-neovim),\n[Sublime Text](#example-sublime-text), Emacs and more.\n\nFor Visual Studio Code, check out the [Ruff VS Code extension](https://github.com/charliermarsh/ruff-vscode).\n\n## Highlights\n\n### "Quick Fix" actions for auto-fixable violations (like unused imports)\n\n![](https://user-images.githubusercontent.com/1309177/205176932-44cfc03a-120f-4bad-b710-612bdd7765d6.gif)\n\n### "Fix all": automatically fix all auto-fixable violations\n\n![](https://user-images.githubusercontent.com/1309177/205175763-cf34871d-5c05-4abf-9916-440afc82dbf8.gif)\n\n### "Organize Imports": `isort`-compatible import sorting\n\n![](https://user-images.githubusercontent.com/1309177/205175987-82e23e21-14bb-467d-9ef0-027f24b75865.gif)\n\n## Installation and Usage\n\n`ruff-lsp` is available as [`ruff-lsp`](https://pypi.org/project/ruff-lsp/) on PyPI:\n\n```shell\npip install ruff-lsp\n```\n\nFrom there, `ruff-lsp` can be used with any editor that supports the Language Server Protocol,\nincluding Neovim, Emacs, Sublime Text, and more.\n\n### Example: Neovim\n\nFor example, to use `ruff-lsp` with Neovim, install `ruff-lsp` from PyPI along with\n[`nvim-lspconfig`](https://github.com/neovim/nvim-lspconfig). Then, add something like the following\nto your `init.lua`:\n\n```lua\n-- See: https://github.com/neovim/nvim-lspconfig/tree/54eb2a070a4f389b1be0f98070f81d23e2b1a715#suggested-configuration\nlocal opts = { noremap=true, silent=true }\nvim.keymap.set(\'n\', \'<space>e\', vim.diagnostic.open_float, opts)\nvim.keymap.set(\'n\', \'[d\', vim.diagnostic.goto_prev, opts)\nvim.keymap.set(\'n\', \']d\', vim.diagnostic.goto_next, opts)\nvim.keymap.set(\'n\', \'<space>q\', vim.diagnostic.setloclist, opts)\n\n-- Use an on_attach function to only map the following keys\n-- after the language server attaches to the current buffer\nlocal on_attach = function(client, bufnr)\n  -- Enable completion triggered by <c-x><c-o>\n  vim.api.nvim_buf_set_option(bufnr, \'omnifunc\', \'v:lua.vim.lsp.omnifunc\')\n\n  -- Mappings.\n  -- See `:help vim.lsp.*` for documentation on any of the below functions\n  local bufopts = { noremap=true, silent=true, buffer=bufnr }\n  vim.keymap.set(\'n\', \'gD\', vim.lsp.buf.declaration, bufopts)\n  vim.keymap.set(\'n\', \'gd\', vim.lsp.buf.definition, bufopts)\n  vim.keymap.set(\'n\', \'K\', vim.lsp.buf.hover, bufopts)\n  vim.keymap.set(\'n\', \'gi\', vim.lsp.buf.implementation, bufopts)\n  vim.keymap.set(\'n\', \'<C-k>\', vim.lsp.buf.signature_help, bufopts)\n  vim.keymap.set(\'n\', \'<space>wa\', vim.lsp.buf.add_workspace_folder, bufopts)\n  vim.keymap.set(\'n\', \'<space>wr\', vim.lsp.buf.remove_workspace_folder, bufopts)\n  vim.keymap.set(\'n\', \'<space>wl\', function()\n    print(vim.inspect(vim.lsp.buf.list_workspace_folders()))\n  end, bufopts)\n  vim.keymap.set(\'n\', \'<space>D\', vim.lsp.buf.type_definition, bufopts)\n  vim.keymap.set(\'n\', \'<space>rn\', vim.lsp.buf.rename, bufopts)\n  vim.keymap.set(\'n\', \'<space>ca\', vim.lsp.buf.code_action, bufopts)\n  vim.keymap.set(\'n\', \'gr\', vim.lsp.buf.references, bufopts)\n  vim.keymap.set(\'n\', \'<space>f\', function() vim.lsp.buf.format { async = true } end, bufopts)\nend\n\n-- Configure `ruff-lsp`.\nlocal configs = require \'lspconfig.configs\'\nif not configs.ruff_lsp then\n  configs.ruff_lsp = {\n    default_config = {\n      cmd = { \'ruff-lsp\' },\n      filetypes = { \'python\' },\n      root_dir = require(\'lspconfig\').util.find_git_ancestor,\n      init_options = {\n        settings = {\n          args = {}\n        }\n      } \n    }\n  }\nend\nrequire(\'lspconfig\').ruff_lsp.setup {\n  on_attach = on_attach,\n}\n```\n\nUpon successful installation, you should see Ruff\'s diagnostics surfaced directly in your editor:\n\n![Code Actions available in Neovim](https://user-images.githubusercontent.com/1309177/208278707-25fa37e4-079d-4597-ad35-b95dba066960.png)\n\nRuff also integrates with [`coc.nvim`](https://github.com/neoclide/coc.nvim/wiki/Language-servers#using-ruff-lsp):\n\n```json\n"languageserver": {\n  "ruff-lsp": {\n    "command": "ruff-lsp",\n    "filetypes": ["python"]\n  }\n}\n```\n\n### Example: Sublime Text\n\nTo use `ruff-lsp` with Sublime Text, install Sublime Text\'s [LSP](https://github.com/sublimelsp/LSP)\npackage, then add something like the following to `LSP.sublime-settings`:\n\n```json\n{\n  "clients": {\n    "ruff-lsp": {\n      "command": ["ruff-lsp"],\n      "enabled": true,\n      "selector": "source.python",\n      "initializationOptions": {\n        "settings": {\n          "args": []\n        }\n      }\n    }\n  }\n}\n```\n\nUpon successful installation, you should see errors surfaced directly in your editor:\n\n![Code Actions available in Sublime Text](https://user-images.githubusercontent.com/1309177/208266375-331ad8e5-8ac1-4735-bca8-07734eb38536.png)\n\n### Example: Helix\n\nTo use `ruff-lsp` with [Helix](https://helix-editor.com/), add something like the following to\n`~/.config/helix/languages.toml`:\n\n```toml\n[[language]]\nname = "python"\nscope = "source.python"\nlanguage-server = { command = "ruff-lsp" }\nconfig = { settings = { args = [] } }\n```\n\nUpon successful installation, you should see errors surfaced directly in your editor:\n\n![](https://user-images.githubusercontent.com/1309177/209262106-71e34f8d-73cc-4889-89f7-3f54a4481c52.png)\n\n### Example: Lapce\n\nTo use `ruff-lsp` with [Lapce](https://lapce.dev/), install the [`lapce-ruff-lsp`](https://plugins.lapce.dev/plugins/abreumatheus/lapce-ruff-lsp)\nplugin (which wraps `ruff-lsp`) from the Lapce plugins panel.\n\nUpon successful installation, you should see errors surfaced directly in your editor:\n\n![](https://user-images.githubusercontent.com/1309177/209418462-ae106d1f-dbc3-4d53-bae2-66bfccc3e841.png)\n\n## Settings\n\nThe exact mechanism by which settings will be passed to `ruff-lsp` will vary by editor. However,\nthe following settings are supported:\n\n| Settings         | Default | Description                                                                              |\n|------------------|---------|------------------------------------------------------------------------------------------|\n| args             | `[]`    | Custom arguments passed to `ruff`. E.g `"args": ["--config=/path/to/pyproject.toml"]`.   |\n| logLevel         | `error` | Sets the tracing level for the extension.                                                |\n| path             | `[]`    | Setting to provide custom `ruff` executables, to try in order. E.g. `["/path/to/ruff"]`. |\n| interpreter      | `[]`    | Path to a Python interpreter to use to run the linter server.                            |\n| showNotification | `off`   | Setting to control when a notification is shown.                                         |\n| organizeImports  | `true`  | Whether to register Ruff as capable of handling `source.organizeImports` actions.        |\n| fixAll           | `true`  | Whether to register Ruff as capable of handling `source.fixAll` actions.                 |\n\n## Development\n\n`ruff-lsp` uses Poetry for environment management and packaging. To get started, clone the\nrepository, install Poetry, and run `poetry install`.\n\nTo automatically format the codebase, run: `make format`.\n\nTo run lint and type checks, run: `make check`.\n\n## License\n\nMIT\n',
     'author': 'Charlie Marsh',
     'author_email': 'charlie.r.marsh@gmail.com',
     'maintainer': 'Charlie Marsh',
     'maintainer_email': 'charlie.r.marsh@gmail.com',
     'url': 'https://github.com/charliermarsh/ruff-lsp',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ruff-lsp-0.0.8/PKG-INFO` & `ruff-lsp-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ruff-lsp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Language Server Protocol implementation for Ruff.
 Home-page: https://github.com/charliermarsh/ruff-lsp
 License: MIT
 Keywords: ruff,lsp,language-server,language-server-protocol,python
 Author: Charlie Marsh
 Author-email: charlie.r.marsh@gmail.com
 Maintainer: Charlie Marsh
 Maintainer-email: charlie.r.marsh@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
@@ -181,14 +182,23 @@
 config = { settings = { args = [] } }
 ```
 
 Upon successful installation, you should see errors surfaced directly in your editor:
 
 ![](https://user-images.githubusercontent.com/1309177/209262106-71e34f8d-73cc-4889-89f7-3f54a4481c52.png)
 
+### Example: Lapce
+
+To use `ruff-lsp` with [Lapce](https://lapce.dev/), install the [`lapce-ruff-lsp`](https://plugins.lapce.dev/plugins/abreumatheus/lapce-ruff-lsp)
+plugin (which wraps `ruff-lsp`) from the Lapce plugins panel.
+
+Upon successful installation, you should see errors surfaced directly in your editor:
+
+![](https://user-images.githubusercontent.com/1309177/209418462-ae106d1f-dbc3-4d53-bae2-66bfccc3e841.png)
+
 ## Settings
 
 The exact mechanism by which settings will be passed to `ruff-lsp` will vary by editor. However,
 the following settings are supported:
 
 | Settings         | Default | Description                                                                              |
 |------------------|---------|------------------------------------------------------------------------------------------|
```

