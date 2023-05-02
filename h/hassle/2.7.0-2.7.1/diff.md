# Comparing `tmp/hassle-2.7.0.tar.gz` & `tmp/hassle-2.7.1.tar.gz`

## Comparing `hassle-2.7.0.tar` & `hassle-2.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 hassle-2.7.0/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/index.html
--rw-r--r--   0        0        0    42579 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/search.js
--rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   122450 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   112334 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165766 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/new_project.html
--rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.7.0/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/new_project.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.7.0/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.7.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.7.0/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.7.0/README.md
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 hassle-2.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/index.html
+-rw-r--r--   0        0        0    42729 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/search.js
+-rw-r--r--   0        0        0    93051 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   122922 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   112334 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165006 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    52052 2020-02-02 00:00:00.000000 hassle-2.7.1/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/new_project.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 hassle-2.7.1/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.7.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.7.1/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.7.1/README.md
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 hassle-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0    22508 2020-02-02 00:00:00.000000 hassle-2.7.1/PKG-INFO
```

### Comparing `hassle-2.7.0/CHANGELOG.md` & `hassle-2.7.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,40 @@
 # Changelog
 
-## 2.5.0 (2023-04-15)
+## 2.7.0 (2023-04-28)
+
+#### Refactorings
+
+* add a pause to manually prune the changelog before committing the autoupdate
+
+
+## v2.6.0 (2023-04-15)
+
+#### Refactorings
+
+* return minimum py version as string
+* extract getting project code into separate function
+* extract vermin scan into separate function
+#### Others
+
+* build v2.6.0
+
+
+## v2.5.0 (2023-04-15)
 
 #### Fixes
 
 * fix already exist error by switching pathlib to pathier
 #### Refactorings
 
 * replace pathlib, os.chdir, and shutil calls with pathier
 #### Others
 
+* build v2.5.0
+* update changelog
 * prune dependencies
 
 
 ## v2.4.0 (2023-04-07)
 
 #### New Features
```

### Comparing `hassle-2.7.0/docs/hassle.html` & `hassle-2.7.1/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/docs/search.js` & `hassle-2.7.1/docs/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -897,23 +897,23 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.get_answer",
         "modulename": "hassle.new_project",
         "qualname": "get_answer",
         "kind": "function",
-        "doc": "<p>Repeatedly ask the user a yes/no question\nuntil a 'y' or a 'n' is received.</p>\n",
+        "doc": "<p>Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">question</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.check_pypi_for_name",
         "modulename": "hassle.new_project",
         "qualname": "check_pypi_for_name",
         "kind": "function",
-        "doc": "<p>Check if a package with package_name\nalready exists on pypi.org .\nReturns True if package name exists.\nOnly checks the first page of results.</p>\n",
+        "doc": "<p>Check if a package with package_name already exists on <code>pypi.org</code>.\nReturns <code>True</code> if package name exists.\nOnly checks the first page of results.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">package_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">bool</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.check_pypi_for_name_cli",
         "modulename": "hassle.new_project",
         "qualname": "check_pypi_for_name_cli",
         "kind": "function",
@@ -921,55 +921,55 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_pyproject_file",
         "modulename": "hassle.new_project",
         "qualname": "create_pyproject_file",
         "kind": "function",
-        "doc": "<p>Create pyproject.toml in ./{project_name} from args,\npyproject_template, and hassle_config.</p>\n",
+        "doc": "<p>Create <code>pyproject.toml</code> in <code>./{project_name}</code> from args, pyproject_template, and hassle_config.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_source_files",
         "modulename": "hassle.new_project",
         "qualname": "create_source_files",
         "kind": "function",
-        "doc": "<p>Generate empty source files in ./{package_name}/src/{package_name}/</p>\n",
+        "doc": "<p>Generate empty source files in <code>./{package_name}/src/{package_name}/</code></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">srcdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">filelist</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_readme",
         "modulename": "hassle.new_project",
         "qualname": "create_readme",
         "kind": "function",
-        "doc": "<p>Create README.md in ./{package_name}\nfrom readme_template and args.</p>\n",
+        "doc": "<p>Create <code>README.md</code> in <code>./{package_name}</code> from readme_template and args.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_license",
         "modulename": "hassle.new_project",
         "qualname": "create_license",
         "kind": "function",
-        "doc": "<p>Add MIT license file to ./{package_name} .</p>\n",
+        "doc": "<p>Add MIT license file to <code>./{package_name}</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_gitignore",
         "modulename": "hassle.new_project",
         "qualname": "create_gitignore",
         "kind": "function",
-        "doc": "<p>Add .gitignore to ./{package_name}</p>\n",
+        "doc": "<p>Add <code>.gitignore</code> to <code>./{package_name}</code></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.create_vscode_settings",
         "modulename": "hassle.new_project",
         "qualname": "create_vscode_settings",
         "kind": "function",
-        "doc": "<p>Add settings.json to ./.vscode</p>\n",
+        "doc": "<p>Add <code>settings.json</code> to <code>./.vscode</code></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">targetdir</span><span class=\"p\">:</span> <span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "hassle.new_project.main",
         "modulename": "hassle.new_project",
         "qualname": "main",
         "kind": "function",
```

### Comparing `hassle-2.7.0/docs/hassle/generate_tests.html` & `hassle-2.7.1/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/docs/hassle/hassle.html` & `hassle-2.7.1/docs/hassle/hassle.html`

 * *Files 1% similar despite different names*

```diff
@@ -239,55 +239,57 @@
 </span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
 </span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
 </span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
 </span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
 </span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="p">)</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="c1"># commit changelog first</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="nb">input</span><span class="p">(</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="p">)</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="c1"># Vermin isn&#39;t taking into account the minimum version of dependencies.</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="c1"># Removing from now and defaulting to &gt;=3.10</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="c1"># hassle_utilities.update_minimum_python_version(pyproject_path)</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="c1"># commit changelog first</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="nb">input</span><span class="p">(</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>            <span class="p">)</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -484,51 +486,53 @@
 </span><span id="main-181"><a href="#main-181"><span class="linenos">181</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">build</span><span class="p">:</span>
 </span><span id="main-182"><a href="#main-182"><span class="linenos">182</span></a>        <span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s2">&quot;dist&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
 </span><span id="main-183"><a href="#main-183"><span class="linenos">183</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;black </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="main-184"><a href="#main-184"><span class="linenos">184</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;isort </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="main-185"><a href="#main-185"><span class="linenos">185</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_dependencies</span><span class="p">(</span>
 </span><span id="main-186"><a href="#main-186"><span class="linenos">186</span></a>            <span class="n">pyproject_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">overwrite_dependencies</span>
 </span><span id="main-187"><a href="#main-187"><span class="linenos">187</span></a>        <span class="p">)</span>
-</span><span id="main-188"><a href="#main-188"><span class="linenos">188</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_minimum_python_version</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="main-189"><a href="#main-189"><span class="linenos">189</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-190"><a href="#main-190"><span class="linenos">190</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-191"><a href="#main-191"><span class="linenos">191</span></a>
-</span><span id="main-192"><a href="#main-192"><span class="linenos">192</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
-</span><span id="main-193"><a href="#main-193"><span class="linenos">193</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
-</span><span id="main-194"><a href="#main-194"><span class="linenos">194</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
-</span><span id="main-195"><a href="#main-195"><span class="linenos">195</span></a>        <span class="c1"># commit changelog first</span>
-</span><span id="main-196"><a href="#main-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-197"><a href="#main-197"><span class="linenos">197</span></a>            <span class="nb">input</span><span class="p">(</span>
-</span><span id="main-198"><a href="#main-198"><span class="linenos">198</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
-</span><span id="main-199"><a href="#main-199"><span class="linenos">199</span></a>            <span class="p">)</span>
-</span><span id="main-200"><a href="#main-200"><span class="linenos">200</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-201"><a href="#main-201"><span class="linenos">201</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
-</span><span id="main-202"><a href="#main-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
-</span><span id="main-203"><a href="#main-203"><span class="linenos">203</span></a>
-</span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
-</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
-</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
-</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>
-</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
-</span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>
-</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
-</span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>
-</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
-</span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
-</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>
-</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
-</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
-</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
-</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
+</span><span id="main-188"><a href="#main-188"><span class="linenos">188</span></a>        <span class="c1"># Vermin isn&#39;t taking into account the minimum version of dependencies.</span>
+</span><span id="main-189"><a href="#main-189"><span class="linenos">189</span></a>        <span class="c1"># Removing from now and defaulting to &gt;=3.10</span>
+</span><span id="main-190"><a href="#main-190"><span class="linenos">190</span></a>        <span class="c1"># hassle_utilities.update_minimum_python_version(pyproject_path)</span>
+</span><span id="main-191"><a href="#main-191"><span class="linenos">191</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">generate_docs</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-192"><a href="#main-192"><span class="linenos">192</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py -m build </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-193"><a href="#main-193"><span class="linenos">193</span></a>
+</span><span id="main-194"><a href="#main-194"><span class="linenos">194</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">:</span>
+</span><span id="main-195"><a href="#main-195"><span class="linenos">195</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">update_changelog</span><span class="p">(</span><span class="n">pyproject_path</span><span class="p">)</span>
+</span><span id="main-196"><a href="#main-196"><span class="linenos">196</span></a>        <span class="c1"># If we&#39;re going to add tag for current version</span>
+</span><span id="main-197"><a href="#main-197"><span class="linenos">197</span></a>        <span class="c1"># commit changelog first</span>
+</span><span id="main-198"><a href="#main-198"><span class="linenos">198</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="main-199"><a href="#main-199"><span class="linenos">199</span></a>            <span class="nb">input</span><span class="p">(</span>
+</span><span id="main-200"><a href="#main-200"><span class="linenos">200</span></a>                <span class="s2">&quot;Press enter to continue after optionally pruning the updated changelog...&quot;</span>
+</span><span id="main-201"><a href="#main-201"><span class="linenos">201</span></a>            <span class="p">)</span>
+</span><span id="main-202"><a href="#main-202"><span class="linenos">202</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-203"><a href="#main-203"><span class="linenos">203</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add CHANGELOG.md&quot;</span><span class="p">)</span>
+</span><span id="main-204"><a href="#main-204"><span class="linenos">204</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s1">&#39;git commit CHANGELOG.md -m &quot;chore: update changelog&quot;&#39;</span><span class="p">)</span>
+</span><span id="main-205"><a href="#main-205"><span class="linenos">205</span></a>
+</span><span id="main-206"><a href="#main-206"><span class="linenos">206</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="p">:</span>
+</span><span id="main-207"><a href="#main-207"><span class="linenos">207</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-208"><a href="#main-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">==</span> <span class="s2">&quot;build&quot;</span><span class="p">:</span>
+</span><span id="main-209"><a href="#main-209"><span class="linenos">209</span></a>            <span class="n">version</span> <span class="o">=</span> <span class="n">pyproject_path</span><span class="o">.</span><span class="n">loads</span><span class="p">()[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="main-210"><a href="#main-210"><span class="linenos">210</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">commit_all</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;chore: build v</span><span class="si">{</span><span class="n">version</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-211"><a href="#main-211"><span class="linenos">211</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git add .&quot;</span><span class="p">)</span>
+</span><span id="main-212"><a href="#main-212"><span class="linenos">212</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;git commit -m &quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">commit_all</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="main-213"><a href="#main-213"><span class="linenos">213</span></a>
+</span><span id="main-214"><a href="#main-214"><span class="linenos">214</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">tag_version</span><span class="p">:</span>
+</span><span id="main-215"><a href="#main-215"><span class="linenos">215</span></a>        <span class="n">hassle_utilities</span><span class="o">.</span><span class="n">tag_version</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-216"><a href="#main-216"><span class="linenos">216</span></a>
+</span><span id="main-217"><a href="#main-217"><span class="linenos">217</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">publish</span><span class="p">:</span>
+</span><span id="main-218"><a href="#main-218"><span class="linenos">218</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;twine upload </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span> <span class="o">/</span> <span class="s1">&#39;dist&#39;</span> <span class="o">/</span> <span class="s1">&#39;*&#39;</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="main-219"><a href="#main-219"><span class="linenos">219</span></a>
+</span><span id="main-220"><a href="#main-220"><span class="linenos">220</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">install</span><span class="p">:</span>
+</span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pip install </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2"> --no-deps --upgrade --no-cache-dir&quot;</span><span class="p">)</span>
+</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>
+</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">sync</span><span class="p">:</span>
+</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">)</span>
+</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git pull --tags origin main&quot;</span><span class="p">)</span>
+</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git push origin main:main --tags&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -199,58 +199,61 @@
 180    if args.build:
 181        (args.package / "dist").delete()
 182        os.system(f"black {args.package}")
 183        os.system(f"isort {args.package}")
 184        hassle_utilities.update_dependencies(
 185            pyproject_path, args.overwrite_dependencies
 186        )
-187        hassle_utilities.update_minimum_python_version(pyproject_path)
-188        hassle_utilities.generate_docs(args.package)
-189        os.system(f"py -m build {args.package}")
-190
-191    if args.update_changelog:
-192        hassle_utilities.update_changelog(pyproject_path)
-193        # If we're going to add tag for current version
-194        # commit changelog first
-195        if args.tag_version:
-196            input(
-197                "Press enter to continue after optionally pruning the
+187        # Vermin isn't taking into account the minimum version of
+dependencies.
+188        # Removing from now and defaulting to >=3.10
+189        # hassle_utilities.update_minimum_python_version(pyproject_path)
+190        hassle_utilities.generate_docs(args.package)
+191        os.system(f"py -m build {args.package}")
+192
+193    if args.update_changelog:
+194        hassle_utilities.update_changelog(pyproject_path)
+195        # If we're going to add tag for current version
+196        # commit changelog first
+197        if args.tag_version:
+198            input(
+199                "Press enter to continue after optionally pruning the
 updated changelog..."
-198            )
-199            os.chdir(args.package)
-200            os.system("git add CHANGELOG.md")
-201            os.system('git commit CHANGELOG.md -m "chore: update
+200            )
+201            os.chdir(args.package)
+202            os.system("git add CHANGELOG.md")
+203            os.system('git commit CHANGELOG.md -m "chore: update
 changelog"')
-202
-203    if args.commit_all:
-204        os.chdir(args.package)
-205        if args.commit_all == "build":
-206            version = pyproject_path.loads()["project"]["version"]
-207            args.commit_all = f"chore: build v{version}"
-208        os.system("git add .")
-209        os.system(f'git commit -m "{args.commit_all}"')
-210
-211    if args.tag_version:
-212        hassle_utilities.tag_version(args.package)
-213
-214    if args.publish:
-215        os.system(f"twine upload {args.package / 'dist' / '*'}")
-216
-217    if args.install:
-218        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+204
+205    if args.commit_all:
+206        os.chdir(args.package)
+207        if args.commit_all == "build":
+208            version = pyproject_path.loads()["project"]["version"]
+209            args.commit_all = f"chore: build v{version}"
+210        os.system("git add .")
+211        os.system(f'git commit -m "{args.commit_all}"')
+212
+213    if args.tag_version:
+214        hassle_utilities.tag_version(args.package)
+215
+216    if args.publish:
+217        os.system(f"twine upload {args.package / 'dist' / '*'}")
+218
+219    if args.install:
+220        os.system(f"pip install {args.package} --no-deps --upgrade --no-
 cache-dir")
-219
-220    if args.sync:
-221        os.chdir(args.package)
-222        os.system(f"git pull --tags origin main")
-223        os.system(f"git push origin main:main --tags")
-224
-225
-226if __name__ == "__main__":
-227    main(get_args())
+221
+222    if args.sync:
+223        os.chdir(args.package)
+224        os.system(f"git pull --tags origin main")
+225        os.system(f"git push origin main:main --tags")
+226
+227
+228if __name__ == "__main__":
+229    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
 _14def get_args() -> argparse.Namespace:
 _15    parser = argparse.ArgumentParser()
 _16
 _17    parser.add_argument(
 _18        "package",
@@ -427,48 +430,51 @@
 181    if args.build:
 182        (args.package / "dist").delete()
 183        os.system(f"black {args.package}")
 184        os.system(f"isort {args.package}")
 185        hassle_utilities.update_dependencies(
 186            pyproject_path, args.overwrite_dependencies
 187        )
-188        hassle_utilities.update_minimum_python_version(pyproject_path)
-189        hassle_utilities.generate_docs(args.package)
-190        os.system(f"py -m build {args.package}")
-191
-192    if args.update_changelog:
-193        hassle_utilities.update_changelog(pyproject_path)
-194        # If we're going to add tag for current version
-195        # commit changelog first
-196        if args.tag_version:
-197            input(
-198                "Press enter to continue after optionally pruning the
+188        # Vermin isn't taking into account the minimum version of
+dependencies.
+189        # Removing from now and defaulting to >=3.10
+190        # hassle_utilities.update_minimum_python_version(pyproject_path)
+191        hassle_utilities.generate_docs(args.package)
+192        os.system(f"py -m build {args.package}")
+193
+194    if args.update_changelog:
+195        hassle_utilities.update_changelog(pyproject_path)
+196        # If we're going to add tag for current version
+197        # commit changelog first
+198        if args.tag_version:
+199            input(
+200                "Press enter to continue after optionally pruning the
 updated changelog..."
-199            )
-200            os.chdir(args.package)
-201            os.system("git add CHANGELOG.md")
-202            os.system('git commit CHANGELOG.md -m "chore: update
+201            )
+202            os.chdir(args.package)
+203            os.system("git add CHANGELOG.md")
+204            os.system('git commit CHANGELOG.md -m "chore: update
 changelog"')
-203
-204    if args.commit_all:
-205        os.chdir(args.package)
-206        if args.commit_all == "build":
-207            version = pyproject_path.loads()["project"]["version"]
-208            args.commit_all = f"chore: build v{version}"
-209        os.system("git add .")
-210        os.system(f'git commit -m "{args.commit_all}"')
-211
-212    if args.tag_version:
-213        hassle_utilities.tag_version(args.package)
-214
-215    if args.publish:
-216        os.system(f"twine upload {args.package / 'dist' / '*'}")
-217
-218    if args.install:
-219        os.system(f"pip install {args.package} --no-deps --upgrade --no-
+205
+206    if args.commit_all:
+207        os.chdir(args.package)
+208        if args.commit_all == "build":
+209            version = pyproject_path.loads()["project"]["version"]
+210            args.commit_all = f"chore: build v{version}"
+211        os.system("git add .")
+212        os.system(f'git commit -m "{args.commit_all}"')
+213
+214    if args.tag_version:
+215        hassle_utilities.tag_version(args.package)
+216
+217    if args.publish:
+218        os.system(f"twine upload {args.package / 'dist' / '*'}")
+219
+220    if args.install:
+221        os.system(f"pip install {args.package} --no-deps --upgrade --no-
 cache-dir")
-220
-221    if args.sync:
-222        os.chdir(args.package)
-223        os.system(f"git pull --tags origin main")
-224        os.system(f"git push origin main:main --tags")
+222
+223    if args.sync:
+224        os.chdir(args.package)
+225        os.system(f"git pull --tags origin main")
+226        os.system(f"git push origin main:main --tags")
```

### Comparing `hassle-2.7.0/docs/hassle/hassle_config.html` & `hassle-2.7.1/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/docs/hassle/hassle_utilities.html` & `hassle-2.7.1/docs/hassle/hassle_utilities.html`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/docs/hassle/new_project.html` & `hassle-2.7.1/docs/hassle/new_project.html`

 * *Files 0% similar despite different names*

```diff
@@ -189,177 +189,173 @@
 </span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
 </span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="s2">&quot;__init__.py&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.py&quot;</span><span class="p">])</span>
 </span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
 </span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
 </span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
 </span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">    until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
 </span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    already exists on pypi.org .</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">    Returns True if package name exists.</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="p">)</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="p">]</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="sd">&quot;&quot;&quot;Create pyproject.toml in ./{project_name} from args,</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">    pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="p">)</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in ./{package_name}/src/{package_name}/&quot;&quot;&quot;</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="sd">&quot;&quot;&quot;Create README.md in ./{package_name}</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">    from readme_template and args.&quot;&quot;&quot;</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="p">)</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to ./{package_name} .&quot;&quot;&quot;</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name already exists on `pypi.org`.</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    Returns `True` if package name exists.</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>    <span class="p">]</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="sd">&quot;&quot;&quot;Create `pyproject.toml` in `./{project_name}` from args, pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="p">)</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="p">)</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in `./{package_name}/src/{package_name}/`&quot;&quot;&quot;</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="sd">&quot;&quot;&quot;Create `README.md` in `./{package_name}` from readme_template and args.&quot;&quot;&quot;</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="p">)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to `./{package_name}`.&quot;&quot;&quot;</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="sd">&quot;&quot;&quot;Add `.gitignore` to `./{package_name}`&quot;&quot;&quot;</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="sd">&quot;&quot;&quot;Add .gitignore to ./{package_name}&quot;&quot;&quot;</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>    <span class="sd">&quot;&quot;&quot;Add settings.json to ./.vscode&quot;&quot;&quot;</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="p">)</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="p">)</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="sd">&quot;&quot;&quot;Add `settings.json` to `./.vscode`&quot;&quot;&quot;</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="p">)</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -476,34 +472,32 @@
         <span class="name">get_answer</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">question</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="get_answer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#get_answer"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="get_answer-110"><a href="#get_answer-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">get_answer</span><span class="p">(</span><span class="n">question</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="get_answer-111"><a href="#get_answer-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question</span>
-</span><span id="get_answer-112"><a href="#get_answer-112"><span class="linenos">112</span></a><span class="sd">    until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
-</span><span id="get_answer-113"><a href="#get_answer-113"><span class="linenos">113</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="get_answer-114"><a href="#get_answer-114"><span class="linenos">114</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
-</span><span id="get_answer-115"><a href="#get_answer-115"><span class="linenos">115</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
-</span><span id="get_answer-116"><a href="#get_answer-116"><span class="linenos">116</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
-</span><span id="get_answer-117"><a href="#get_answer-117"><span class="linenos">117</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
-</span><span id="get_answer-118"><a href="#get_answer-118"><span class="linenos">118</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-119"><a href="#get_answer-119"><span class="linenos">119</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="get_answer-120"><a href="#get_answer-120"><span class="linenos">120</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-121"><a href="#get_answer-121"><span class="linenos">121</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="get_answer-122"><a href="#get_answer-122"><span class="linenos">122</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
-</span><span id="get_answer-123"><a href="#get_answer-123"><span class="linenos">123</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="get_answer-124"><a href="#get_answer-124"><span class="linenos">124</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="get_answer-125"><a href="#get_answer-125"><span class="linenos">125</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
+</span><span id="get_answer-111"><a href="#get_answer-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Repeatedly ask the user a yes/no question until a &#39;y&#39; or a &#39;n&#39; is received.&quot;&quot;&quot;</span>
+</span><span id="get_answer-112"><a href="#get_answer-112"><span class="linenos">112</span></a>    <span class="n">ans</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="get_answer-113"><a href="#get_answer-113"><span class="linenos">113</span></a>    <span class="n">question</span> <span class="o">=</span> <span class="n">question</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
+</span><span id="get_answer-114"><a href="#get_answer-114"><span class="linenos">114</span></a>    <span class="k">if</span> <span class="s2">&quot;?&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">question</span><span class="p">:</span>
+</span><span id="get_answer-115"><a href="#get_answer-115"><span class="linenos">115</span></a>        <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot;?&quot;</span>
+</span><span id="get_answer-116"><a href="#get_answer-116"><span class="linenos">116</span></a>    <span class="n">question</span> <span class="o">+=</span> <span class="s2">&quot; (y/n): &quot;</span>
+</span><span id="get_answer-117"><a href="#get_answer-117"><span class="linenos">117</span></a>    <span class="k">while</span> <span class="n">ans</span> <span class="ow">not</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">,</span> <span class="s2">&quot;n&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-118"><a href="#get_answer-118"><span class="linenos">118</span></a>        <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="n">question</span><span class="p">)</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="get_answer-119"><a href="#get_answer-119"><span class="linenos">119</span></a>        <span class="k">if</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;y&quot;</span><span class="p">,</span> <span class="s2">&quot;yes&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-120"><a href="#get_answer-120"><span class="linenos">120</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="get_answer-121"><a href="#get_answer-121"><span class="linenos">121</span></a>        <span class="k">elif</span> <span class="n">ans</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;n&quot;</span><span class="p">,</span> <span class="s2">&quot;no&quot;</span><span class="p">]:</span>
+</span><span id="get_answer-122"><a href="#get_answer-122"><span class="linenos">122</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="get_answer-123"><a href="#get_answer-123"><span class="linenos">123</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="get_answer-124"><a href="#get_answer-124"><span class="linenos">124</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Invalid answer.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Repeatedly ask the user a yes/no question
-until a 'y' or a 'n' is received.</p>
+            <div class="docstring"><p>Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received.</p>
 </div>
 
 
                 </section>
                 <section id="check_pypi_for_name">
                             <input id="check_pypi_for_name-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -511,37 +505,35 @@
         <span class="def">def</span>
         <span class="name">check_pypi_for_name</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="check_pypi_for_name-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#check_pypi_for_name"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name-128"><a href="#check_pypi_for_name-128"><span class="linenos">128</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="check_pypi_for_name-129"><a href="#check_pypi_for_name-129"><span class="linenos">129</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name</span>
-</span><span id="check_pypi_for_name-130"><a href="#check_pypi_for_name-130"><span class="linenos">130</span></a><span class="sd">    already exists on pypi.org .</span>
-</span><span id="check_pypi_for_name-131"><a href="#check_pypi_for_name-131"><span class="linenos">131</span></a><span class="sd">    Returns True if package name exists.</span>
-</span><span id="check_pypi_for_name-132"><a href="#check_pypi_for_name-132"><span class="linenos">132</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
-</span><span id="check_pypi_for_name-133"><a href="#check_pypi_for_name-133"><span class="linenos">133</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="check_pypi_for_name-134"><a href="#check_pypi_for_name-134"><span class="linenos">134</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-135"><a href="#check_pypi_for_name-135"><span class="linenos">135</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
-</span><span id="check_pypi_for_name-136"><a href="#check_pypi_for_name-136"><span class="linenos">136</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
-</span><span id="check_pypi_for_name-137"><a href="#check_pypi_for_name-137"><span class="linenos">137</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="check_pypi_for_name-138"><a href="#check_pypi_for_name-138"><span class="linenos">138</span></a>        <span class="p">)</span>
-</span><span id="check_pypi_for_name-139"><a href="#check_pypi_for_name-139"><span class="linenos">139</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-140"><a href="#check_pypi_for_name-140"><span class="linenos">140</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="check_pypi_for_name-141"><a href="#check_pypi_for_name-141"><span class="linenos">141</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
-</span><span id="check_pypi_for_name-142"><a href="#check_pypi_for_name-142"><span class="linenos">142</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name-143"><a href="#check_pypi_for_name-143"><span class="linenos">143</span></a>    <span class="p">]</span>
-</span><span id="check_pypi_for_name-144"><a href="#check_pypi_for_name-144"><span class="linenos">144</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name-127"><a href="#check_pypi_for_name-127"><span class="linenos">127</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name</span><span class="p">(</span><span class="n">package_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="check_pypi_for_name-128"><a href="#check_pypi_for_name-128"><span class="linenos">128</span></a>    <span class="sd">&quot;&quot;&quot;Check if a package with package_name already exists on `pypi.org`.</span>
+</span><span id="check_pypi_for_name-129"><a href="#check_pypi_for_name-129"><span class="linenos">129</span></a><span class="sd">    Returns `True` if package name exists.</span>
+</span><span id="check_pypi_for_name-130"><a href="#check_pypi_for_name-130"><span class="linenos">130</span></a><span class="sd">    Only checks the first page of results.&quot;&quot;&quot;</span>
+</span><span id="check_pypi_for_name-131"><a href="#check_pypi_for_name-131"><span class="linenos">131</span></a>    <span class="n">url</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;https://pypi.org/search/?q=</span><span class="si">{</span><span class="n">package_name</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="check_pypi_for_name-132"><a href="#check_pypi_for_name-132"><span class="linenos">132</span></a>    <span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-133"><a href="#check_pypi_for_name-133"><span class="linenos">133</span></a>    <span class="k">if</span> <span class="n">response</span><span class="o">.</span><span class="n">status_code</span> <span class="o">!=</span> <span class="mi">200</span><span class="p">:</span>
+</span><span id="check_pypi_for_name-134"><a href="#check_pypi_for_name-134"><span class="linenos">134</span></a>        <span class="k">raise</span> <span class="ne">RuntimeError</span><span class="p">(</span>
+</span><span id="check_pypi_for_name-135"><a href="#check_pypi_for_name-135"><span class="linenos">135</span></a>            <span class="sa">f</span><span class="s2">&quot;Error: pypi.org returned status code: </span><span class="si">{</span><span class="n">response</span><span class="o">.</span><span class="n">status_code</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="check_pypi_for_name-136"><a href="#check_pypi_for_name-136"><span class="linenos">136</span></a>        <span class="p">)</span>
+</span><span id="check_pypi_for_name-137"><a href="#check_pypi_for_name-137"><span class="linenos">137</span></a>    <span class="n">soup</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">&quot;html.parser&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-138"><a href="#check_pypi_for_name-138"><span class="linenos">138</span></a>    <span class="n">pypi_packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="check_pypi_for_name-139"><a href="#check_pypi_for_name-139"><span class="linenos">139</span></a>        <span class="n">span</span><span class="o">.</span><span class="n">text</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>
+</span><span id="check_pypi_for_name-140"><a href="#check_pypi_for_name-140"><span class="linenos">140</span></a>        <span class="k">for</span> <span class="n">span</span> <span class="ow">in</span> <span class="n">soup</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">&quot;span&quot;</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">&quot;package-snippet__name&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name-141"><a href="#check_pypi_for_name-141"><span class="linenos">141</span></a>    <span class="p">]</span>
+</span><span id="check_pypi_for_name-142"><a href="#check_pypi_for_name-142"><span class="linenos">142</span></a>    <span class="k">return</span> <span class="n">package_name</span> <span class="ow">in</span> <span class="n">pypi_packages</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Check if a package with package_name
-already exists on pypi.org .
-Returns True if package name exists.
+            <div class="docstring"><p>Check if a package with package_name already exists on <code>pypi.org</code>.
+Returns <code>True</code> if package name exists.
 Only checks the first page of results.</p>
 </div>
 
 
                 </section>
                 <section id="check_pypi_for_name_cli">
                             <input id="check_pypi_for_name_cli-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -550,22 +542,22 @@
         <span class="def">def</span>
         <span class="name">check_pypi_for_name_cli</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="check_pypi_for_name_cli-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#check_pypi_for_name_cli"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name_cli-147"><a href="#check_pypi_for_name_cli-147"><span class="linenos">147</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
-</span><span id="check_pypi_for_name_cli-148"><a href="#check_pypi_for_name_cli-148"><span class="linenos">148</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="check_pypi_for_name_cli-149"><a href="#check_pypi_for_name_cli-149"><span class="linenos">149</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
-</span><span id="check_pypi_for_name_cli-150"><a href="#check_pypi_for_name_cli-150"><span class="linenos">150</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="check_pypi_for_name_cli-151"><a href="#check_pypi_for_name_cli-151"><span class="linenos">151</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="check_pypi_for_name_cli-152"><a href="#check_pypi_for_name_cli-152"><span class="linenos">152</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
-</span><span id="check_pypi_for_name_cli-153"><a href="#check_pypi_for_name_cli-153"><span class="linenos">153</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="check_pypi_for_name_cli-154"><a href="#check_pypi_for_name_cli-154"><span class="linenos">154</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="check_pypi_for_name_cli-145"><a href="#check_pypi_for_name_cli-145"><span class="linenos">145</span></a><span class="k">def</span> <span class="nf">check_pypi_for_name_cli</span><span class="p">():</span>
+</span><span id="check_pypi_for_name_cli-146"><a href="#check_pypi_for_name_cli-146"><span class="linenos">146</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="check_pypi_for_name_cli-147"><a href="#check_pypi_for_name_cli-147"><span class="linenos">147</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">)</span>
+</span><span id="check_pypi_for_name_cli-148"><a href="#check_pypi_for_name_cli-148"><span class="linenos">148</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="check_pypi_for_name_cli-149"><a href="#check_pypi_for_name_cli-149"><span class="linenos">149</span></a>    <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="check_pypi_for_name_cli-150"><a href="#check_pypi_for_name_cli-150"><span class="linenos">150</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is already taken.&quot;</span><span class="p">)</span>
+</span><span id="check_pypi_for_name_cli-151"><a href="#check_pypi_for_name_cli-151"><span class="linenos">151</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="check_pypi_for_name_cli-152"><a href="#check_pypi_for_name_cli-152"><span class="linenos">152</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is available.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="create_pyproject_file">
@@ -575,49 +567,47 @@
         <span class="def">def</span>
         <span class="name">create_pyproject_file</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_pyproject_file-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_pyproject_file"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_pyproject_file-157"><a href="#create_pyproject_file-157"><span class="linenos">157</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="create_pyproject_file-158"><a href="#create_pyproject_file-158"><span class="linenos">158</span></a>    <span class="sd">&quot;&quot;&quot;Create pyproject.toml in ./{project_name} from args,</span>
-</span><span id="create_pyproject_file-159"><a href="#create_pyproject_file-159"><span class="linenos">159</span></a><span class="sd">    pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
-</span><span id="create_pyproject_file-160"><a href="#create_pyproject_file-160"><span class="linenos">160</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
-</span><span id="create_pyproject_file-161"><a href="#create_pyproject_file-161"><span class="linenos">161</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
-</span><span id="create_pyproject_file-162"><a href="#create_pyproject_file-162"><span class="linenos">162</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
-</span><span id="create_pyproject_file-163"><a href="#create_pyproject_file-163"><span class="linenos">163</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
-</span><span id="create_pyproject_file-164"><a href="#create_pyproject_file-164"><span class="linenos">164</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
-</span><span id="create_pyproject_file-165"><a href="#create_pyproject_file-165"><span class="linenos">165</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="create_pyproject_file-166"><a href="#create_pyproject_file-166"><span class="linenos">166</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
-</span><span id="create_pyproject_file-167"><a href="#create_pyproject_file-167"><span class="linenos">167</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
-</span><span id="create_pyproject_file-168"><a href="#create_pyproject_file-168"><span class="linenos">168</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
-</span><span id="create_pyproject_file-169"><a href="#create_pyproject_file-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="create_pyproject_file-170"><a href="#create_pyproject_file-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
-</span><span id="create_pyproject_file-171"><a href="#create_pyproject_file-171"><span class="linenos">171</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="create_pyproject_file-172"><a href="#create_pyproject_file-172"><span class="linenos">172</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
-</span><span id="create_pyproject_file-173"><a href="#create_pyproject_file-173"><span class="linenos">173</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
-</span><span id="create_pyproject_file-174"><a href="#create_pyproject_file-174"><span class="linenos">174</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
-</span><span id="create_pyproject_file-175"><a href="#create_pyproject_file-175"><span class="linenos">175</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="create_pyproject_file-176"><a href="#create_pyproject_file-176"><span class="linenos">176</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
-</span><span id="create_pyproject_file-177"><a href="#create_pyproject_file-177"><span class="linenos">177</span></a>        <span class="p">)</span>
-</span><span id="create_pyproject_file-178"><a href="#create_pyproject_file-178"><span class="linenos">178</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="create_pyproject_file-179"><a href="#create_pyproject_file-179"><span class="linenos">179</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-</span><span id="create_pyproject_file-180"><a href="#create_pyproject_file-180"><span class="linenos">180</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
-</span><span id="create_pyproject_file-181"><a href="#create_pyproject_file-181"><span class="linenos">181</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="create_pyproject_file-182"><a href="#create_pyproject_file-182"><span class="linenos">182</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="create_pyproject_file-183"><a href="#create_pyproject_file-183"><span class="linenos">183</span></a>        <span class="p">)</span>
-</span><span id="create_pyproject_file-184"><a href="#create_pyproject_file-184"><span class="linenos">184</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
-</span><span id="create_pyproject_file-185"><a href="#create_pyproject_file-185"><span class="linenos">185</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
-</span><span id="create_pyproject_file-186"><a href="#create_pyproject_file-186"><span class="linenos">186</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_pyproject_file-155"><a href="#create_pyproject_file-155"><span class="linenos">155</span></a><span class="k">def</span> <span class="nf">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="create_pyproject_file-156"><a href="#create_pyproject_file-156"><span class="linenos">156</span></a>    <span class="sd">&quot;&quot;&quot;Create `pyproject.toml` in `./{project_name}` from args, pyproject_template, and hassle_config.&quot;&quot;&quot;</span>
+</span><span id="create_pyproject_file-157"><a href="#create_pyproject_file-157"><span class="linenos">157</span></a>    <span class="n">pyproject</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;pyproject_template.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">loads</span><span class="p">()</span>
+</span><span id="create_pyproject_file-158"><a href="#create_pyproject_file-158"><span class="linenos">158</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">config_exists</span><span class="p">():</span>
+</span><span id="create_pyproject_file-159"><a href="#create_pyproject_file-159"><span class="linenos">159</span></a>        <span class="n">hassle_config</span><span class="o">.</span><span class="n">warn</span><span class="p">()</span>
+</span><span id="create_pyproject_file-160"><a href="#create_pyproject_file-160"><span class="linenos">160</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue creating new package with blank config?&quot;</span><span class="p">):</span>
+</span><span id="create_pyproject_file-161"><a href="#create_pyproject_file-161"><span class="linenos">161</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="s2">&quot;Aborting new package creation&quot;</span><span class="p">)</span>
+</span><span id="create_pyproject_file-162"><a href="#create_pyproject_file-162"><span class="linenos">162</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="create_pyproject_file-163"><a href="#create_pyproject_file-163"><span class="linenos">163</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating blank hassle_config.toml...&quot;</span><span class="p">)</span>
+</span><span id="create_pyproject_file-164"><a href="#create_pyproject_file-164"><span class="linenos">164</span></a>            <span class="n">hassle_config</span><span class="o">.</span><span class="n">create_config</span><span class="p">()</span>
+</span><span id="create_pyproject_file-165"><a href="#create_pyproject_file-165"><span class="linenos">165</span></a>    <span class="n">config</span> <span class="o">=</span> <span class="n">hassle_config</span><span class="o">.</span><span class="n">load_config</span><span class="p">()</span>
+</span><span id="create_pyproject_file-166"><a href="#create_pyproject_file-166"><span class="linenos">166</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;name&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="create_pyproject_file-167"><a href="#create_pyproject_file-167"><span class="linenos">167</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;authors&quot;</span><span class="p">]</span>
+</span><span id="create_pyproject_file-168"><a href="#create_pyproject_file-168"><span class="linenos">168</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;description&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="create_pyproject_file-169"><a href="#create_pyproject_file-169"><span class="linenos">169</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;dependencies&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">dependencies</span>
+</span><span id="create_pyproject_file-170"><a href="#create_pyproject_file-170"><span class="linenos">170</span></a>    <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">keywords</span>
+</span><span id="create_pyproject_file-171"><a href="#create_pyproject_file-171"><span class="linenos">171</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span><span class="p">:</span>
+</span><span id="create_pyproject_file-172"><a href="#create_pyproject_file-172"><span class="linenos">172</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">][</span><span class="mi">2</span><span class="p">]</span> <span class="o">=</span> <span class="s2">&quot;Operating System :: &quot;</span> <span class="o">+</span> <span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="create_pyproject_file-173"><a href="#create_pyproject_file-173"><span class="linenos">173</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">operating_system</span>
+</span><span id="create_pyproject_file-174"><a href="#create_pyproject_file-174"><span class="linenos">174</span></a>        <span class="p">)</span>
+</span><span id="create_pyproject_file-175"><a href="#create_pyproject_file-175"><span class="linenos">175</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="create_pyproject_file-176"><a href="#create_pyproject_file-176"><span class="linenos">176</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;classifiers&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+</span><span id="create_pyproject_file-177"><a href="#create_pyproject_file-177"><span class="linenos">177</span></a>    <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">]:</span>
+</span><span id="create_pyproject_file-178"><a href="#create_pyproject_file-178"><span class="linenos">178</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span> <span class="o">=</span> <span class="n">config</span><span class="p">[</span><span class="s2">&quot;project_urls&quot;</span><span class="p">][</span><span class="n">field</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="create_pyproject_file-179"><a href="#create_pyproject_file-179"><span class="linenos">179</span></a>            <span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="create_pyproject_file-180"><a href="#create_pyproject_file-180"><span class="linenos">180</span></a>        <span class="p">)</span>
+</span><span id="create_pyproject_file-181"><a href="#create_pyproject_file-181"><span class="linenos">181</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">add_script</span><span class="p">:</span>
+</span><span id="create_pyproject_file-182"><a href="#create_pyproject_file-182"><span class="linenos">182</span></a>        <span class="n">pyproject</span><span class="p">[</span><span class="s2">&quot;project&quot;</span><span class="p">][</span><span class="s2">&quot;scripts&quot;</span><span class="p">][</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">.</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">:main&quot;</span>
+</span><span id="create_pyproject_file-183"><a href="#create_pyproject_file-183"><span class="linenos">183</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;pyproject.toml&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">pyproject</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Create pyproject.toml in ./{project_name} from args,
-pyproject_template, and hassle_config.</p>
+            <div class="docstring"><p>Create <code>pyproject.toml</code> in <code>./{project_name}</code> from args, pyproject_template, and hassle_config.</p>
 </div>
 
 
                 </section>
                 <section id="create_source_files">
                             <input id="create_source_files-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -625,23 +615,23 @@
         <span class="def">def</span>
         <span class="name">create_source_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">srcdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_source_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_source_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_source_files-189"><a href="#create_source_files-189"><span class="linenos">189</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="create_source_files-190"><a href="#create_source_files-190"><span class="linenos">190</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in ./{package_name}/src/{package_name}/&quot;&quot;&quot;</span>
-</span><span id="create_source_files-191"><a href="#create_source_files-191"><span class="linenos">191</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="create_source_files-192"><a href="#create_source_files-192"><span class="linenos">192</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
-</span><span id="create_source_files-193"><a href="#create_source_files-193"><span class="linenos">193</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_source_files-186"><a href="#create_source_files-186"><span class="linenos">186</span></a><span class="k">def</span> <span class="nf">create_source_files</span><span class="p">(</span><span class="n">srcdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">filelist</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="create_source_files-187"><a href="#create_source_files-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Generate empty source files in `./{package_name}/src/{package_name}/`&quot;&quot;&quot;</span>
+</span><span id="create_source_files-188"><a href="#create_source_files-188"><span class="linenos">188</span></a>    <span class="n">srcdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="create_source_files-189"><a href="#create_source_files-189"><span class="linenos">189</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">filelist</span><span class="p">:</span>
+</span><span id="create_source_files-190"><a href="#create_source_files-190"><span class="linenos">190</span></a>        <span class="p">(</span><span class="n">srcdir</span> <span class="o">/</span> <span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Generate empty source files in ./{package_name}/src/{package_name}/</p>
+            <div class="docstring"><p>Generate empty source files in <code>./{package_name}/src/{package_name}/</code></p>
 </div>
 
 
                 </section>
                 <section id="create_readme">
                             <input id="create_readme-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -649,27 +639,25 @@
         <span class="def">def</span>
         <span class="name">create_readme</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_readme-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_readme"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_readme-196"><a href="#create_readme-196"><span class="linenos">196</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="create_readme-197"><a href="#create_readme-197"><span class="linenos">197</span></a>    <span class="sd">&quot;&quot;&quot;Create README.md in ./{package_name}</span>
-</span><span id="create_readme-198"><a href="#create_readme-198"><span class="linenos">198</span></a><span class="sd">    from readme_template and args.&quot;&quot;&quot;</span>
-</span><span id="create_readme-199"><a href="#create_readme-199"><span class="linenos">199</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="create_readme-200"><a href="#create_readme-200"><span class="linenos">200</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
-</span><span id="create_readme-201"><a href="#create_readme-201"><span class="linenos">201</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
-</span><span id="create_readme-202"><a href="#create_readme-202"><span class="linenos">202</span></a>    <span class="p">)</span>
-</span><span id="create_readme-203"><a href="#create_readme-203"><span class="linenos">203</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_readme-193"><a href="#create_readme-193"><span class="linenos">193</span></a><span class="k">def</span> <span class="nf">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="create_readme-194"><a href="#create_readme-194"><span class="linenos">194</span></a>    <span class="sd">&quot;&quot;&quot;Create `README.md` in `./{package_name}` from readme_template and args.&quot;&quot;&quot;</span>
+</span><span id="create_readme-195"><a href="#create_readme-195"><span class="linenos">195</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;README_template.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="create_readme-196"><a href="#create_readme-196"><span class="linenos">196</span></a>    <span class="n">readme</span> <span class="o">=</span> <span class="n">readme</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$name&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span>
+</span><span id="create_readme-197"><a href="#create_readme-197"><span class="linenos">197</span></a>        <span class="s2">&quot;$description&quot;</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">description</span>
+</span><span id="create_readme-198"><a href="#create_readme-198"><span class="linenos">198</span></a>    <span class="p">)</span>
+</span><span id="create_readme-199"><a href="#create_readme-199"><span class="linenos">199</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;README.md&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">readme</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Create README.md in ./{package_name}
-from readme_template and args.</p>
+            <div class="docstring"><p>Create <code>README.md</code> in <code>./{package_name}</code> from readme_template and args.</p>
 </div>
 
 
                 </section>
                 <section id="create_license">
                             <input id="create_license-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -677,23 +665,23 @@
         <span class="def">def</span>
         <span class="name">create_license</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_license-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_license"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_license-206"><a href="#create_license-206"><span class="linenos">206</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="create_license-207"><a href="#create_license-207"><span class="linenos">207</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to ./{package_name} .&quot;&quot;&quot;</span>
-</span><span id="create_license-208"><a href="#create_license-208"><span class="linenos">208</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="create_license-209"><a href="#create_license-209"><span class="linenos">209</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
-</span><span id="create_license-210"><a href="#create_license-210"><span class="linenos">210</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_license-202"><a href="#create_license-202"><span class="linenos">202</span></a><span class="k">def</span> <span class="nf">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_license-203"><a href="#create_license-203"><span class="linenos">203</span></a>    <span class="sd">&quot;&quot;&quot;Add MIT license file to `./{package_name}`.&quot;&quot;&quot;</span>
+</span><span id="create_license-204"><a href="#create_license-204"><span class="linenos">204</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;license_template.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="create_license-205"><a href="#create_license-205"><span class="linenos">205</span></a>    <span class="n">license_template</span> <span class="o">=</span> <span class="n">license_template</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;$year&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">year</span><span class="p">))</span>
+</span><span id="create_license-206"><a href="#create_license-206"><span class="linenos">206</span></a>    <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;LICENSE.txt&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">license_template</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Add MIT license file to ./{package_name} .</p>
+            <div class="docstring"><p>Add MIT license file to <code>./{package_name}</code>.</p>
 </div>
 
 
                 </section>
                 <section id="create_gitignore">
                             <input id="create_gitignore-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -701,21 +689,21 @@
         <span class="def">def</span>
         <span class="name">create_gitignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_gitignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_gitignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_gitignore-213"><a href="#create_gitignore-213"><span class="linenos">213</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="create_gitignore-214"><a href="#create_gitignore-214"><span class="linenos">214</span></a>    <span class="sd">&quot;&quot;&quot;Add .gitignore to ./{package_name}&quot;&quot;&quot;</span>
-</span><span id="create_gitignore-215"><a href="#create_gitignore-215"><span class="linenos">215</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_gitignore-209"><a href="#create_gitignore-209"><span class="linenos">209</span></a><span class="k">def</span> <span class="nf">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_gitignore-210"><a href="#create_gitignore-210"><span class="linenos">210</span></a>    <span class="sd">&quot;&quot;&quot;Add `.gitignore` to `./{package_name}`&quot;&quot;&quot;</span>
+</span><span id="create_gitignore-211"><a href="#create_gitignore-211"><span class="linenos">211</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.gitignore_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.gitignore&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Add .gitignore to ./{package_name}</p>
+            <div class="docstring"><p>Add <code>.gitignore</code> to <code>./{package_name}</code></p>
 </div>
 
 
                 </section>
                 <section id="create_vscode_settings">
                             <input id="create_vscode_settings-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -723,23 +711,23 @@
         <span class="def">def</span>
         <span class="name">create_vscode_settings</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">targetdir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_vscode_settings-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_vscode_settings"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_vscode_settings-218"><a href="#create_vscode_settings-218"><span class="linenos">218</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
-</span><span id="create_vscode_settings-219"><a href="#create_vscode_settings-219"><span class="linenos">219</span></a>    <span class="sd">&quot;&quot;&quot;Add settings.json to ./.vscode&quot;&quot;&quot;</span>
-</span><span id="create_vscode_settings-220"><a href="#create_vscode_settings-220"><span class="linenos">220</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
-</span><span id="create_vscode_settings-221"><a href="#create_vscode_settings-221"><span class="linenos">221</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="create_vscode_settings-222"><a href="#create_vscode_settings-222"><span class="linenos">222</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_vscode_settings-214"><a href="#create_vscode_settings-214"><span class="linenos">214</span></a><span class="k">def</span> <span class="nf">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">):</span>
+</span><span id="create_vscode_settings-215"><a href="#create_vscode_settings-215"><span class="linenos">215</span></a>    <span class="sd">&quot;&quot;&quot;Add `settings.json` to `./.vscode`&quot;&quot;&quot;</span>
+</span><span id="create_vscode_settings-216"><a href="#create_vscode_settings-216"><span class="linenos">216</span></a>    <span class="n">vsdir</span> <span class="o">=</span> <span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;.vscode&quot;</span>
+</span><span id="create_vscode_settings-217"><a href="#create_vscode_settings-217"><span class="linenos">217</span></a>    <span class="n">vsdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="create_vscode_settings-218"><a href="#create_vscode_settings-218"><span class="linenos">218</span></a>    <span class="p">(</span><span class="n">root</span> <span class="o">/</span> <span class="s2">&quot;.vscode_template&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">vsdir</span> <span class="o">/</span> <span class="s2">&quot;settings.json&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Add settings.json to ./.vscode</p>
+            <div class="docstring"><p>Add <code>settings.json</code> to <code>./.vscode</code></p>
 </div>
 
 
                 </section>
                 <section id="main">
                             <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -747,59 +735,59 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
-</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
-</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="main-233"><a href="#main-233"><span class="linenos">233</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-234"><a href="#main-234"><span class="linenos">234</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="main-235"><a href="#main-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="main-236"><a href="#main-236"><span class="linenos">236</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="main-237"><a href="#main-237"><span class="linenos">237</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
-</span><span id="main-238"><a href="#main-238"><span class="linenos">238</span></a>            <span class="p">)</span>
-</span><span id="main-239"><a href="#main-239"><span class="linenos">239</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
-</span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
-</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
-</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
-</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
-</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
-</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
-</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>        <span class="p">)</span>
-</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
-</span><span id="main-257"><a href="#main-257"><span class="linenos">257</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-258"><a href="#main-258"><span class="linenos">258</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-259"><a href="#main-259"><span class="linenos">259</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-260"><a href="#main-260"><span class="linenos">260</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
-</span><span id="main-261"><a href="#main-261"><span class="linenos">261</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-262"><a href="#main-262"><span class="linenos">262</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
-</span><span id="main-263"><a href="#main-263"><span class="linenos">263</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
-</span><span id="main-264"><a href="#main-264"><span class="linenos">264</span></a>
-</span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="main-267"><a href="#main-267"><span class="linenos">267</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="main-268"><a href="#main-268"><span class="linenos">268</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
-</span><span id="main-269"><a href="#main-269"><span class="linenos">269</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-221"><a href="#main-221"><span class="linenos">221</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-222"><a href="#main-222"><span class="linenos">222</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-223"><a href="#main-223"><span class="linenos">223</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-224"><a href="#main-224"><span class="linenos">224</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-225"><a href="#main-225"><span class="linenos">225</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="main-226"><a href="#main-226"><span class="linenos">226</span></a>            <span class="k">if</span> <span class="n">check_pypi_for_name</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">):</span>
+</span><span id="main-227"><a href="#main-227"><span class="linenos">227</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists on pypi.org&quot;</span><span class="p">)</span>
+</span><span id="main-228"><a href="#main-228"><span class="linenos">228</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="main-229"><a href="#main-229"><span class="linenos">229</span></a>                    <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-230"><a href="#main-230"><span class="linenos">230</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="main-231"><a href="#main-231"><span class="linenos">231</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="main-232"><a href="#main-232"><span class="linenos">232</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="main-233"><a href="#main-233"><span class="linenos">233</span></a>                <span class="sa">f</span><span class="s2">&quot;Couldn&#39;t verify that </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> doesn&#39;t already exist on pypi.org .&quot;</span>
+</span><span id="main-234"><a href="#main-234"><span class="linenos">234</span></a>            <span class="p">)</span>
+</span><span id="main-235"><a href="#main-235"><span class="linenos">235</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Continue anyway?&quot;</span><span class="p">):</span>
+</span><span id="main-236"><a href="#main-236"><span class="linenos">236</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-237"><a href="#main-237"><span class="linenos">237</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="main-238"><a href="#main-238"><span class="linenos">238</span></a>        <span class="n">targetdir</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span>
+</span><span id="main-239"><a href="#main-239"><span class="linenos">239</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="main-240"><a href="#main-240"><span class="linenos">240</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+</span><span id="main-241"><a href="#main-241"><span class="linenos">241</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="main-242"><a href="#main-242"><span class="linenos">242</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">targetdir</span><span class="si">}</span><span class="s2"> already exists.&quot;</span><span class="p">)</span>
+</span><span id="main-243"><a href="#main-243"><span class="linenos">243</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Overwrite?&quot;</span><span class="p">):</span>
+</span><span id="main-244"><a href="#main-244"><span class="linenos">244</span></a>                <span class="n">sys</span><span class="o">.</span><span class="n">exit</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="main-245"><a href="#main-245"><span class="linenos">245</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-246"><a href="#main-246"><span class="linenos">246</span></a>            <span class="n">create_pyproject_file</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="main-247"><a href="#main-247"><span class="linenos">247</span></a>        <span class="n">create_source_files</span><span class="p">(</span>
+</span><span id="main-248"><a href="#main-248"><span class="linenos">248</span></a>            <span class="n">targetdir</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="p">(</span><span class="n">targetdir</span> <span class="o">/</span> <span class="s2">&quot;src&quot;</span> <span class="o">/</span> <span class="n">args</span><span class="o">.</span><span class="n">name</span><span class="p">),</span>
+</span><span id="main-249"><a href="#main-249"><span class="linenos">249</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">source_files</span><span class="p">,</span>
+</span><span id="main-250"><a href="#main-250"><span class="linenos">250</span></a>        <span class="p">)</span>
+</span><span id="main-251"><a href="#main-251"><span class="linenos">251</span></a>        <span class="n">create_readme</span><span class="p">(</span><span class="n">targetdir</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="main-252"><a href="#main-252"><span class="linenos">252</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">not_package</span><span class="p">:</span>
+</span><span id="main-253"><a href="#main-253"><span class="linenos">253</span></a>            <span class="n">generate_test_files</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-254"><a href="#main-254"><span class="linenos">254</span></a>            <span class="n">create_vscode_settings</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-255"><a href="#main-255"><span class="linenos">255</span></a>        <span class="n">create_gitignore</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-256"><a href="#main-256"><span class="linenos">256</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_license</span><span class="p">:</span>
+</span><span id="main-257"><a href="#main-257"><span class="linenos">257</span></a>            <span class="n">create_license</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-258"><a href="#main-258"><span class="linenos">258</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">targetdir</span><span class="p">)</span>
+</span><span id="main-259"><a href="#main-259"><span class="linenos">259</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="s2">&quot;git init -b main&quot;</span><span class="p">)</span>
+</span><span id="main-260"><a href="#main-260"><span class="linenos">260</span></a>
+</span><span id="main-261"><a href="#main-261"><span class="linenos">261</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="main-262"><a href="#main-262"><span class="linenos">262</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="s2">&quot;Aborting new package creation&quot;</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="main-263"><a href="#main-263"><span class="linenos">263</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="main-264"><a href="#main-264"><span class="linenos">264</span></a>        <span class="k">if</span> <span class="n">get_answer</span><span class="p">(</span><span class="s2">&quot;Delete created files?&quot;</span><span class="p">):</span>
+</span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a>            <span class="n">targetdir</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -130,186 +130,185 @@
 103    args = parser.parse_args()
 104    args.source_files.extend(["__init__.py", f"{args.name}.py"])
 105
 106    return args
 107
 108
 109def get_answer(question: str) -> bool:
-110    """Repeatedly ask the user a yes/no question
-111    until a 'y' or a 'n' is received."""
-112    ans = ""
-113    question = question.strip()
-114    if "?" not in question:
-115        question += "?"
-116    question += " (y/n): "
-117    while ans not in ["y", "yes", "no", "n"]:
-118        ans = input(question).strip().lower()
-119        if ans in ["y", "yes"]:
-120            return True
-121        elif ans in ["n", "no"]:
-122            return False
-123        else:
-124            print("Invalid answer.")
+110    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is
+received."""
+111    ans = ""
+112    question = question.strip()
+113    if "?" not in question:
+114        question += "?"
+115    question += " (y/n): "
+116    while ans not in ["y", "yes", "no", "n"]:
+117        ans = input(question).strip().lower()
+118        if ans in ["y", "yes"]:
+119            return True
+120        elif ans in ["n", "no"]:
+121            return False
+122        else:
+123            print("Invalid answer.")
+124
 125
-126
-127def check_pypi_for_name(package_name: str) -> bool:
-128    """Check if a package with package_name
-129    already exists on pypi.org .
-130    Returns True if package name exists.
-131    Only checks the first page of results."""
-132    url = f"https://pypi.org/search/?q={package_name.lower()}"
-133    response = requests.get(url)
-134    if response.status_code != 200:
-135        raise RuntimeError(
-136            f"Error: pypi.org returned status code: {response.status_code}"
-137        )
-138    soup = BeautifulSoup(response.text, "html.parser")
-139    pypi_packages = [
-140        span.text.lower()
-141        for span in soup.find_all("span", class_="package-snippet__name")
-142    ]
-143    return package_name in pypi_packages
-144
-145
-146def check_pypi_for_name_cli():
-147    parser = argparse.ArgumentParser()
-148    parser.add_argument("name", type=str)
-149    args = parser.parse_args()
-150    if check_pypi_for_name(args.name):
-151        print(f"{args.name} is already taken.")
-152    else:
-153        print(f"{args.name} is available.")
-154
-155
-156def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
-157    """Create pyproject.toml in ./{project_name} from args,
-158    pyproject_template, and hassle_config."""
-159    pyproject = (root / "pyproject_template.toml").loads()
-160    if not hassle_config.config_exists():
-161        hassle_config.warn()
-162        if not get_answer("Continue creating new package with blank
+126def check_pypi_for_name(package_name: str) -> bool:
+127    """Check if a package with package_name already exists on `pypi.org`.
+128    Returns `True` if package name exists.
+129    Only checks the first page of results."""
+130    url = f"https://pypi.org/search/?q={package_name.lower()}"
+131    response = requests.get(url)
+132    if response.status_code != 200:
+133        raise RuntimeError(
+134            f"Error: pypi.org returned status code: {response.status_code}"
+135        )
+136    soup = BeautifulSoup(response.text, "html.parser")
+137    pypi_packages = [
+138        span.text.lower()
+139        for span in soup.find_all("span", class_="package-snippet__name")
+140    ]
+141    return package_name in pypi_packages
+142
+143
+144def check_pypi_for_name_cli():
+145    parser = argparse.ArgumentParser()
+146    parser.add_argument("name", type=str)
+147    args = parser.parse_args()
+148    if check_pypi_for_name(args.name):
+149        print(f"{args.name} is already taken.")
+150    else:
+151        print(f"{args.name} is available.")
+152
+153
+154def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
+155    """Create `pyproject.toml` in `./{project_name}` from args,
+pyproject_template, and hassle_config."""
+156    pyproject = (root / "pyproject_template.toml").loads()
+157    if not hassle_config.config_exists():
+158        hassle_config.warn()
+159        if not get_answer("Continue creating new package with blank
 config?"):
-163            raise Exception("Aborting new package creation")
-164        else:
-165            print("Creating blank hassle_config.toml...")
-166            hassle_config.create_config()
-167    config = hassle_config.load_config()
-168    pyproject["project"]["name"] = args.name
-169    pyproject["project"]["authors"] = config["authors"]
-170    pyproject["project"]["description"] = args.description
-171    pyproject["project"]["dependencies"] = args.dependencies
-172    pyproject["project"]["keywords"] = args.keywords
-173    if args.operating_system:
-174        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
+160            raise Exception("Aborting new package creation")
+161        else:
+162            print("Creating blank hassle_config.toml...")
+163            hassle_config.create_config()
+164    config = hassle_config.load_config()
+165    pyproject["project"]["name"] = args.name
+166    pyproject["project"]["authors"] = config["authors"]
+167    pyproject["project"]["description"] = args.description
+168    pyproject["project"]["dependencies"] = args.dependencies
+169    pyproject["project"]["keywords"] = args.keywords
+170    if args.operating_system:
+171        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
 ".join(
-175            args.operating_system
-176        )
-177    if args.no_license:
-178        pyproject["project"]["classifiers"].pop(1)
-179    for field in config["project_urls"]:
-180        pyproject["project"]["urls"][field] = config["project_urls"]
+172            args.operating_system
+173        )
+174    if args.no_license:
+175        pyproject["project"]["classifiers"].pop(1)
+176    for field in config["project_urls"]:
+177        pyproject["project"]["urls"][field] = config["project_urls"]
 [field].replace(
-181            "$name", args.name
-182        )
-183    if args.add_script:
-184        pyproject["project"]["scripts"][args.name] = f"{args.name}.
+178            "$name", args.name
+179        )
+180    if args.add_script:
+181        pyproject["project"]["scripts"][args.name] = f"{args.name}.
 {args.name}:main"
-185    (targetdir / "pyproject.toml").dumps(pyproject)
-186
-187
-188def create_source_files(srcdir: Pathier, filelist: list[str]):
-189    """Generate empty source files in ./{package_name}/src/{package_name}/
-"""
-190    srcdir.mkdir(parents=True, exist_ok=True)
-191    for file in filelist:
-192        (srcdir / file).touch()
-193
-194
-195def create_readme(targetdir: Pathier, args: argparse.Namespace):
-196    """Create README.md in ./{package_name}
-197    from readme_template and args."""
-198    readme = (root / "README_template.md").read_text()
-199    readme = readme.replace("$name", args.name).replace(
-200        "$description", args.description
-201    )
-202    (targetdir / "README.md").write_text(readme)
-203
-204
-205def create_license(targetdir: Pathier):
-206    """Add MIT license file to ./{package_name} ."""
-207    license_template = (root / "license_template.txt").read_text()
-208    license_template = license_template.replace("$year", str(datetime.now
+182    (targetdir / "pyproject.toml").dumps(pyproject)
+183
+184
+185def create_source_files(srcdir: Pathier, filelist: list[str]):
+186    """Generate empty source files in `./{package_name}/src/{package_name}/
+`"""
+187    srcdir.mkdir(parents=True, exist_ok=True)
+188    for file in filelist:
+189        (srcdir / file).touch()
+190
+191
+192def create_readme(targetdir: Pathier, args: argparse.Namespace):
+193    """Create `README.md` in `./{package_name}` from readme_template and
+args."""
+194    readme = (root / "README_template.md").read_text()
+195    readme = readme.replace("$name", args.name).replace(
+196        "$description", args.description
+197    )
+198    (targetdir / "README.md").write_text(readme)
+199
+200
+201def create_license(targetdir: Pathier):
+202    """Add MIT license file to `./{package_name}`."""
+203    license_template = (root / "license_template.txt").read_text()
+204    license_template = license_template.replace("$year", str(datetime.now
 ().year))
-209    (targetdir / "LICENSE.txt").write_text(license_template)
-210
+205    (targetdir / "LICENSE.txt").write_text(license_template)
+206
+207
+208def create_gitignore(targetdir: Pathier):
+209    """Add `.gitignore` to `./{package_name}`"""
+210    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
 211
-212def create_gitignore(targetdir: Pathier):
-213    """Add .gitignore to ./{package_name}"""
-214    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
-215
-216
-217def create_vscode_settings(targetdir: Pathier):
-218    """Add settings.json to ./.vscode"""
-219    vsdir = targetdir / ".vscode"
-220    vsdir.mkdir(parents=True, exist_ok=True)
-221    (root / ".vscode_template").copy(vsdir / "settings.json", True)
-222
-223
-224def main(args: argparse.Namespace = None):
-225    if not args:
-226        args = get_args()
-227    if not args.not_package:
-228        try:
-229            if check_pypi_for_name(args.name):
-230                print(f"{args.name} already exists on pypi.org")
-231                if not get_answer("Continue anyway?"):
-232                    sys.exit(0)
-233        except Exception as e:
-234            print(e)
-235            print(
-236                f"Couldn't verify that {args.name} doesn't already exist on
+212
+213def create_vscode_settings(targetdir: Pathier):
+214    """Add `settings.json` to `./.vscode`"""
+215    vsdir = targetdir / ".vscode"
+216    vsdir.mkdir(parents=True, exist_ok=True)
+217    (root / ".vscode_template").copy(vsdir / "settings.json", True)
+218
+219
+220def main(args: argparse.Namespace = None):
+221    if not args:
+222        args = get_args()
+223    if not args.not_package:
+224        try:
+225            if check_pypi_for_name(args.name):
+226                print(f"{args.name} already exists on pypi.org")
+227                if not get_answer("Continue anyway?"):
+228                    sys.exit(0)
+229        except Exception as e:
+230            print(e)
+231            print(
+232                f"Couldn't verify that {args.name} doesn't already exist on
 pypi.org ."
-237            )
-238            if not get_answer("Continue anyway?"):
-239                sys.exit(0)
-240    try:
-241        targetdir: Pathier = Pathier.cwd() / args.name
-242        try:
-243            targetdir.mkdir(parents=True, exist_ok=False)
-244        except:
-245            print(f"{targetdir} already exists.")
-246            if not get_answer("Overwrite?"):
-247                sys.exit(0)
-248        if not args.not_package:
-249            create_pyproject_file(targetdir, args)
-250        create_source_files(
-251            targetdir if args.not_package else (targetdir / "src" /
+233            )
+234            if not get_answer("Continue anyway?"):
+235                sys.exit(0)
+236    try:
+237        targetdir: Pathier = Pathier.cwd() / args.name
+238        try:
+239            targetdir.mkdir(parents=True, exist_ok=False)
+240        except:
+241            print(f"{targetdir} already exists.")
+242            if not get_answer("Overwrite?"):
+243                sys.exit(0)
+244        if not args.not_package:
+245            create_pyproject_file(targetdir, args)
+246        create_source_files(
+247            targetdir if args.not_package else (targetdir / "src" /
 args.name),
-252            args.source_files[1:] if args.not_package else
+248            args.source_files[1:] if args.not_package else
 args.source_files,
-253        )
-254        create_readme(targetdir, args)
-255        if not args.not_package:
-256            generate_test_files(targetdir)
-257            create_vscode_settings(targetdir)
-258        create_gitignore(targetdir)
-259        if not args.no_license:
-260            create_license(targetdir)
-261        os.chdir(targetdir)
-262        os.system("git init -b main")
-263
-264    except Exception as e:
-265        if not "Aborting new package creation" in str(e):
-266            print(e)
-267        if get_answer("Delete created files?"):
-268            targetdir.delete()
-269
-270
-271if __name__ == "__main__":
-272    main(get_args())
+249        )
+250        create_readme(targetdir, args)
+251        if not args.not_package:
+252            generate_test_files(targetdir)
+253            create_vscode_settings(targetdir)
+254        create_gitignore(targetdir)
+255        if not args.no_license:
+256            create_license(targetdir)
+257        os.chdir(targetdir)
+258        os.system("git init -b main")
+259
+260    except Exception as e:
+261        if not "Aborting new package creation" in str(e):
+262            print(e)
+263        if get_answer("Delete created files?"):
+264            targetdir.delete()
+265
+266
+267if __name__ == "__main__":
+268    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
 _17def get_args() -> argparse.Namespace:
 _18    parser = argparse.ArgumentParser()
 _19
 _20    parser.add_argument(
 _21        "name",
@@ -405,189 +404,188 @@
 104    args = parser.parse_args()
 105    args.source_files.extend(["__init__.py", f"{args.name}.py"])
 106
 107    return args
   ⁰
 def get_answer(question: str) -> bool: View Source
 110def get_answer(question: str) -> bool:
-111    """Repeatedly ask the user a yes/no question
-112    until a 'y' or a 'n' is received."""
-113    ans = ""
-114    question = question.strip()
-115    if "?" not in question:
-116        question += "?"
-117    question += " (y/n): "
-118    while ans not in ["y", "yes", "no", "n"]:
-119        ans = input(question).strip().lower()
-120        if ans in ["y", "yes"]:
-121            return True
-122        elif ans in ["n", "no"]:
-123            return False
-124        else:
-125            print("Invalid answer.")
+111    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is
+received."""
+112    ans = ""
+113    question = question.strip()
+114    if "?" not in question:
+115        question += "?"
+116    question += " (y/n): "
+117    while ans not in ["y", "yes", "no", "n"]:
+118        ans = input(question).strip().lower()
+119        if ans in ["y", "yes"]:
+120            return True
+121        elif ans in ["n", "no"]:
+122            return False
+123        else:
+124            print("Invalid answer.")
 Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received.
   ⁰
 def check_pypi_for_name(package_name: str) -> bool: View Source
-128def check_pypi_for_name(package_name: str) -> bool:
-129    """Check if a package with package_name
-130    already exists on pypi.org .
-131    Returns True if package name exists.
-132    Only checks the first page of results."""
-133    url = f"https://pypi.org/search/?q={package_name.lower()}"
-134    response = requests.get(url)
-135    if response.status_code != 200:
-136        raise RuntimeError(
-137            f"Error: pypi.org returned status code: {response.status_code}"
-138        )
-139    soup = BeautifulSoup(response.text, "html.parser")
-140    pypi_packages = [
-141        span.text.lower()
-142        for span in soup.find_all("span", class_="package-snippet__name")
-143    ]
-144    return package_name in pypi_packages
-Check if a package with package_name already exists on pypi.org . Returns True
+127def check_pypi_for_name(package_name: str) -> bool:
+128    """Check if a package with package_name already exists on `pypi.org`.
+129    Returns `True` if package name exists.
+130    Only checks the first page of results."""
+131    url = f"https://pypi.org/search/?q={package_name.lower()}"
+132    response = requests.get(url)
+133    if response.status_code != 200:
+134        raise RuntimeError(
+135            f"Error: pypi.org returned status code: {response.status_code}"
+136        )
+137    soup = BeautifulSoup(response.text, "html.parser")
+138    pypi_packages = [
+139        span.text.lower()
+140        for span in soup.find_all("span", class_="package-snippet__name")
+141    ]
+142    return package_name in pypi_packages
+Check if a package with package_name already exists on pypi.org. Returns True
 if package name exists. Only checks the first page of results.
   ⁰
 def check_pypi_for_name_cli(): View Source
-147def check_pypi_for_name_cli():
-148    parser = argparse.ArgumentParser()
-149    parser.add_argument("name", type=str)
-150    args = parser.parse_args()
-151    if check_pypi_for_name(args.name):
-152        print(f"{args.name} is already taken.")
-153    else:
-154        print(f"{args.name} is available.")
+145def check_pypi_for_name_cli():
+146    parser = argparse.ArgumentParser()
+147    parser.add_argument("name", type=str)
+148    args = parser.parse_args()
+149    if check_pypi_for_name(args.name):
+150        print(f"{args.name} is already taken.")
+151    else:
+152        print(f"{args.name} is available.")
   ⁰
 def create_pyproject_file(targetdir: pathier.pathier.Pathier, args:
 argparse.Namespace): View Source
-157def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
-158    """Create pyproject.toml in ./{project_name} from args,
-159    pyproject_template, and hassle_config."""
-160    pyproject = (root / "pyproject_template.toml").loads()
-161    if not hassle_config.config_exists():
-162        hassle_config.warn()
-163        if not get_answer("Continue creating new package with blank
+155def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
+156    """Create `pyproject.toml` in `./{project_name}` from args,
+pyproject_template, and hassle_config."""
+157    pyproject = (root / "pyproject_template.toml").loads()
+158    if not hassle_config.config_exists():
+159        hassle_config.warn()
+160        if not get_answer("Continue creating new package with blank
 config?"):
-164            raise Exception("Aborting new package creation")
-165        else:
-166            print("Creating blank hassle_config.toml...")
-167            hassle_config.create_config()
-168    config = hassle_config.load_config()
-169    pyproject["project"]["name"] = args.name
-170    pyproject["project"]["authors"] = config["authors"]
-171    pyproject["project"]["description"] = args.description
-172    pyproject["project"]["dependencies"] = args.dependencies
-173    pyproject["project"]["keywords"] = args.keywords
-174    if args.operating_system:
-175        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
+161            raise Exception("Aborting new package creation")
+162        else:
+163            print("Creating blank hassle_config.toml...")
+164            hassle_config.create_config()
+165    config = hassle_config.load_config()
+166    pyproject["project"]["name"] = args.name
+167    pyproject["project"]["authors"] = config["authors"]
+168    pyproject["project"]["description"] = args.description
+169    pyproject["project"]["dependencies"] = args.dependencies
+170    pyproject["project"]["keywords"] = args.keywords
+171    if args.operating_system:
+172        pyproject["project"]["classifiers"][2] = "Operating System :: " + "
 ".join(
-176            args.operating_system
-177        )
-178    if args.no_license:
-179        pyproject["project"]["classifiers"].pop(1)
-180    for field in config["project_urls"]:
-181        pyproject["project"]["urls"][field] = config["project_urls"]
+173            args.operating_system
+174        )
+175    if args.no_license:
+176        pyproject["project"]["classifiers"].pop(1)
+177    for field in config["project_urls"]:
+178        pyproject["project"]["urls"][field] = config["project_urls"]
 [field].replace(
-182            "$name", args.name
-183        )
-184    if args.add_script:
-185        pyproject["project"]["scripts"][args.name] = f"{args.name}.
+179            "$name", args.name
+180        )
+181    if args.add_script:
+182        pyproject["project"]["scripts"][args.name] = f"{args.name}.
 {args.name}:main"
-186    (targetdir / "pyproject.toml").dumps(pyproject)
+183    (targetdir / "pyproject.toml").dumps(pyproject)
 Create pyproject.toml in ./{project_name} from args, pyproject_template, and
 hassle_config.
   ⁰
 def create_source_files(srcdir: pathier.pathier.Pathier, filelist: list[str]):
 View Source
-189def create_source_files(srcdir: Pathier, filelist: list[str]):
-190    """Generate empty source files in ./{package_name}/src/{package_name}/
-"""
-191    srcdir.mkdir(parents=True, exist_ok=True)
-192    for file in filelist:
-193        (srcdir / file).touch()
+186def create_source_files(srcdir: Pathier, filelist: list[str]):
+187    """Generate empty source files in `./{package_name}/src/{package_name}/
+`"""
+188    srcdir.mkdir(parents=True, exist_ok=True)
+189    for file in filelist:
+190        (srcdir / file).touch()
 Generate empty source files in ./{package_name}/src/{package_name}/
   ⁰
 def create_readme(targetdir: pathier.pathier.Pathier, args:
 argparse.Namespace): View Source
-196def create_readme(targetdir: Pathier, args: argparse.Namespace):
-197    """Create README.md in ./{package_name}
-198    from readme_template and args."""
-199    readme = (root / "README_template.md").read_text()
-200    readme = readme.replace("$name", args.name).replace(
-201        "$description", args.description
-202    )
-203    (targetdir / "README.md").write_text(readme)
+193def create_readme(targetdir: Pathier, args: argparse.Namespace):
+194    """Create `README.md` in `./{package_name}` from readme_template and
+args."""
+195    readme = (root / "README_template.md").read_text()
+196    readme = readme.replace("$name", args.name).replace(
+197        "$description", args.description
+198    )
+199    (targetdir / "README.md").write_text(readme)
 Create README.md in ./{package_name} from readme_template and args.
   ⁰
 def create_license(targetdir: pathier.pathier.Pathier): View Source
-206def create_license(targetdir: Pathier):
-207    """Add MIT license file to ./{package_name} ."""
-208    license_template = (root / "license_template.txt").read_text()
-209    license_template = license_template.replace("$year", str(datetime.now
+202def create_license(targetdir: Pathier):
+203    """Add MIT license file to `./{package_name}`."""
+204    license_template = (root / "license_template.txt").read_text()
+205    license_template = license_template.replace("$year", str(datetime.now
 ().year))
-210    (targetdir / "LICENSE.txt").write_text(license_template)
-Add MIT license file to ./{package_name} .
+206    (targetdir / "LICENSE.txt").write_text(license_template)
+Add MIT license file to ./{package_name}.
   ⁰
 def create_gitignore(targetdir: pathier.pathier.Pathier): View Source
-213def create_gitignore(targetdir: Pathier):
-214    """Add .gitignore to ./{package_name}"""
-215    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
+209def create_gitignore(targetdir: Pathier):
+210    """Add `.gitignore` to `./{package_name}`"""
+211    (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
 Add .gitignore to ./{package_name}
   ⁰
 def create_vscode_settings(targetdir: pathier.pathier.Pathier): View Source
-218def create_vscode_settings(targetdir: Pathier):
-219    """Add settings.json to ./.vscode"""
-220    vsdir = targetdir / ".vscode"
-221    vsdir.mkdir(parents=True, exist_ok=True)
-222    (root / ".vscode_template").copy(vsdir / "settings.json", True)
+214def create_vscode_settings(targetdir: Pathier):
+215    """Add `settings.json` to `./.vscode`"""
+216    vsdir = targetdir / ".vscode"
+217    vsdir.mkdir(parents=True, exist_ok=True)
+218    (root / ".vscode_template").copy(vsdir / "settings.json", True)
 Add settings.json to ./.vscode
   ⁰
 def main(args: argparse.Namespace = None): View Source
-225def main(args: argparse.Namespace = None):
-226    if not args:
-227        args = get_args()
-228    if not args.not_package:
-229        try:
-230            if check_pypi_for_name(args.name):
-231                print(f"{args.name} already exists on pypi.org")
-232                if not get_answer("Continue anyway?"):
-233                    sys.exit(0)
-234        except Exception as e:
-235            print(e)
-236            print(
-237                f"Couldn't verify that {args.name} doesn't already exist on
+221def main(args: argparse.Namespace = None):
+222    if not args:
+223        args = get_args()
+224    if not args.not_package:
+225        try:
+226            if check_pypi_for_name(args.name):
+227                print(f"{args.name} already exists on pypi.org")
+228                if not get_answer("Continue anyway?"):
+229                    sys.exit(0)
+230        except Exception as e:
+231            print(e)
+232            print(
+233                f"Couldn't verify that {args.name} doesn't already exist on
 pypi.org ."
-238            )
-239            if not get_answer("Continue anyway?"):
-240                sys.exit(0)
-241    try:
-242        targetdir: Pathier = Pathier.cwd() / args.name
-243        try:
-244            targetdir.mkdir(parents=True, exist_ok=False)
-245        except:
-246            print(f"{targetdir} already exists.")
-247            if not get_answer("Overwrite?"):
-248                sys.exit(0)
-249        if not args.not_package:
-250            create_pyproject_file(targetdir, args)
-251        create_source_files(
-252            targetdir if args.not_package else (targetdir / "src" /
+234            )
+235            if not get_answer("Continue anyway?"):
+236                sys.exit(0)
+237    try:
+238        targetdir: Pathier = Pathier.cwd() / args.name
+239        try:
+240            targetdir.mkdir(parents=True, exist_ok=False)
+241        except:
+242            print(f"{targetdir} already exists.")
+243            if not get_answer("Overwrite?"):
+244                sys.exit(0)
+245        if not args.not_package:
+246            create_pyproject_file(targetdir, args)
+247        create_source_files(
+248            targetdir if args.not_package else (targetdir / "src" /
 args.name),
-253            args.source_files[1:] if args.not_package else
+249            args.source_files[1:] if args.not_package else
 args.source_files,
-254        )
-255        create_readme(targetdir, args)
-256        if not args.not_package:
-257            generate_test_files(targetdir)
-258            create_vscode_settings(targetdir)
-259        create_gitignore(targetdir)
-260        if not args.no_license:
-261            create_license(targetdir)
-262        os.chdir(targetdir)
-263        os.system("git init -b main")
-264
-265    except Exception as e:
-266        if not "Aborting new package creation" in str(e):
-267            print(e)
-268        if get_answer("Delete created files?"):
-269            targetdir.delete()
+250        )
+251        create_readme(targetdir, args)
+252        if not args.not_package:
+253            generate_test_files(targetdir)
+254            create_vscode_settings(targetdir)
+255        create_gitignore(targetdir)
+256        if not args.no_license:
+257            create_license(targetdir)
+258        os.chdir(targetdir)
+259        os.system("git init -b main")
+260
+261    except Exception as e:
+262        if not "Aborting new package creation" in str(e):
+263            print(e)
+264        if get_answer("Delete created files?"):
+265            targetdir.delete()
```

### Comparing `hassle-2.7.0/docs/hassle/run_tests.html` & `hassle-2.7.1/docs/hassle/run_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/src/hassle/generate_tests.py` & `hassle-2.7.1/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/src/hassle/hassle.py` & `hassle-2.7.1/src/hassle/hassle.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,17 @@
     if args.build:
         (args.package / "dist").delete()
         os.system(f"black {args.package}")
         os.system(f"isort {args.package}")
         hassle_utilities.update_dependencies(
             pyproject_path, args.overwrite_dependencies
         )
-        hassle_utilities.update_minimum_python_version(pyproject_path)
+        # Vermin isn't taking into account the minimum version of dependencies.
+        # Removing from now and defaulting to >=3.10
+        # hassle_utilities.update_minimum_python_version(pyproject_path)
         hassle_utilities.generate_docs(args.package)
         os.system(f"py -m build {args.package}")
 
     if args.update_changelog:
         hassle_utilities.update_changelog(pyproject_path)
         # If we're going to add tag for current version
         # commit changelog first
```

### Comparing `hassle-2.7.0/src/hassle/hassle_config.py` & `hassle-2.7.1/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/src/hassle/hassle_utilities.py` & `hassle-2.7.1/src/hassle/hassle_utilities.py`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/src/hassle/license_template.txt` & `hassle-2.7.1/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/src/hassle/new_project.py` & `hassle-2.7.1/src/hassle/new_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,15 @@
     args = parser.parse_args()
     args.source_files.extend(["__init__.py", f"{args.name}.py"])
 
     return args
 
 
 def get_answer(question: str) -> bool:
-    """Repeatedly ask the user a yes/no question
-    until a 'y' or a 'n' is received."""
+    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received."""
     ans = ""
     question = question.strip()
     if "?" not in question:
         question += "?"
     question += " (y/n): "
     while ans not in ["y", "yes", "no", "n"]:
         ans = input(question).strip().lower()
@@ -121,17 +120,16 @@
         elif ans in ["n", "no"]:
             return False
         else:
             print("Invalid answer.")
 
 
 def check_pypi_for_name(package_name: str) -> bool:
-    """Check if a package with package_name
-    already exists on pypi.org .
-    Returns True if package name exists.
+    """Check if a package with package_name already exists on `pypi.org`.
+    Returns `True` if package name exists.
     Only checks the first page of results."""
     url = f"https://pypi.org/search/?q={package_name.lower()}"
     response = requests.get(url)
     if response.status_code != 200:
         raise RuntimeError(
             f"Error: pypi.org returned status code: {response.status_code}"
         )
@@ -150,16 +148,15 @@
     if check_pypi_for_name(args.name):
         print(f"{args.name} is already taken.")
     else:
         print(f"{args.name} is available.")
 
 
 def create_pyproject_file(targetdir: Pathier, args: argparse.Namespace):
-    """Create pyproject.toml in ./{project_name} from args,
-    pyproject_template, and hassle_config."""
+    """Create `pyproject.toml` in `./{project_name}` from args, pyproject_template, and hassle_config."""
     pyproject = (root / "pyproject_template.toml").loads()
     if not hassle_config.config_exists():
         hassle_config.warn()
         if not get_answer("Continue creating new package with blank config?"):
             raise Exception("Aborting new package creation")
         else:
             print("Creating blank hassle_config.toml...")
@@ -182,44 +179,43 @@
         )
     if args.add_script:
         pyproject["project"]["scripts"][args.name] = f"{args.name}.{args.name}:main"
     (targetdir / "pyproject.toml").dumps(pyproject)
 
 
 def create_source_files(srcdir: Pathier, filelist: list[str]):
-    """Generate empty source files in ./{package_name}/src/{package_name}/"""
+    """Generate empty source files in `./{package_name}/src/{package_name}/`"""
     srcdir.mkdir(parents=True, exist_ok=True)
     for file in filelist:
         (srcdir / file).touch()
 
 
 def create_readme(targetdir: Pathier, args: argparse.Namespace):
-    """Create README.md in ./{package_name}
-    from readme_template and args."""
+    """Create `README.md` in `./{package_name}` from readme_template and args."""
     readme = (root / "README_template.md").read_text()
     readme = readme.replace("$name", args.name).replace(
         "$description", args.description
     )
     (targetdir / "README.md").write_text(readme)
 
 
 def create_license(targetdir: Pathier):
-    """Add MIT license file to ./{package_name} ."""
+    """Add MIT license file to `./{package_name}`."""
     license_template = (root / "license_template.txt").read_text()
     license_template = license_template.replace("$year", str(datetime.now().year))
     (targetdir / "LICENSE.txt").write_text(license_template)
 
 
 def create_gitignore(targetdir: Pathier):
-    """Add .gitignore to ./{package_name}"""
+    """Add `.gitignore` to `./{package_name}`"""
     (root / ".gitignore_template").copy(targetdir / ".gitignore", True)
 
 
 def create_vscode_settings(targetdir: Pathier):
-    """Add settings.json to ./.vscode"""
+    """Add `settings.json` to `./.vscode`"""
     vsdir = targetdir / ".vscode"
     vsdir.mkdir(parents=True, exist_ok=True)
     (root / ".vscode_template").copy(vsdir / "settings.json", True)
 
 
 def main(args: argparse.Namespace = None):
     if not args:
```

### Comparing `hassle-2.7.0/src/hassle/pyproject_template.toml` & `hassle-2.7.1/src/hassle/pyproject_template.toml`

 * *Files 17% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 220d 0a61 7574 686f 7273 203d 205b   ""..authors = [
 00000070: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 00000080: 2022 220d 0a76 6572 7369 6f6e 203d 2022   ""..version = "
 00000090: 302e 302e 3022 0d0a 7265 7175 6972 6573  0.0.0"..requires
-000000a0: 2d70 7974 686f 6e20 3d20 223e 3d33 2e30  -python = ">=3.0
-000000b0: 220d 0a64 6570 656e 6465 6e63 6965 7320  "..dependencies 
-000000c0: 3d20 5b5d 0d0a 7265 6164 6d65 203d 2022  = []..readme = "
-000000d0: 5245 4144 4d45 2e6d 6422 0d0a 6b65 7977  README.md"..keyw
-000000e0: 6f72 6473 203d 205b 5d0d 0a63 6c61 7373  ords = []..class
-000000f0: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
-00000100: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
-00000110: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000120: 3a3a 2033 222c 0d0a 2020 2020 224c 6963  :: 3",..    "Lic
-00000130: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000140: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-00000150: 6e73 6522 2c0d 0a20 2020 2022 4f70 6572  nse",..    "Oper
-00000160: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000170: 4f53 2049 6e64 6570 656e 6465 6e74 222c  OS Independent",
-00000180: 0d0a 2020 2020 5d0d 0a0d 0a5b 7072 6f6a  ..    ]....[proj
-00000190: 6563 742e 7572 6c73 5d0d 0a22 486f 6d65  ect.urls].."Home
-000001a0: 7061 6765 2220 3d20 2222 0d0a 2244 6f63  page" = "".."Doc
-000001b0: 756d 656e 7461 7469 6f6e 2220 3d20 2222  umentation" = ""
-000001c0: 0d0a 2253 6f75 7263 6520 636f 6465 2220  .."Source code" 
-000001d0: 3d20 2222 0d0a 0d0a 5b74 6f6f 6c2e 7079  = ""....[tool.py
-000001e0: 7465 7374 2e69 6e69 5f6f 7074 696f 6e73  test.ini_options
-000001f0: 5d0d 0a61 6464 6f70 7473 203d 205b 0d0a  ]..addopts = [..
-00000200: 2020 2020 222d 2d69 6d70 6f72 742d 6d6f      "--import-mo
-00000210: 6465 3d69 6d70 6f72 746c 6962 222c 0d0a  de=importlib",..
-00000220: 2020 2020 5d0d 0a70 7974 686f 6e70 6174      ]..pythonpat
-00000230: 6820 3d20 2273 7263 220d 0a0d 0a5b 746f  h = "src"....[to
-00000240: 6f6c 2e68 6174 6368 2e62 7569 6c64 2e74  ol.hatch.build.t
-00000250: 6172 6765 7473 2e73 6469 7374 5d0d 0a65  argets.sdist]..e
-00000260: 7863 6c75 6465 203d 205b 0d0a 2020 2020  xclude = [..    
-00000270: 222e 636f 7665 7261 6765 222c 0d0a 2020  ".coverage",..  
-00000280: 2020 222e 7079 7465 7374 5f63 6163 6865    ".pytest_cache
-00000290: 222c 0d0a 2020 2020 222e 7673 636f 6465  ",..    ".vscode
-000002a0: 222c 0d0a 2020 2020 2274 6573 7473 222c  ",..    "tests",
-000002b0: 0d0a 2020 2020 222e 6769 7469 676e 6f72  ..    ".gitignor
-000002c0: 6522 0d0a 2020 2020 5d0d 0a5b 7072 6f6a  e"..    ]..[proj
-000002d0: 6563 742e 7363 7269 7074 735d            ect.scripts]
+000000a0: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
+000000b0: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
+000000c0: 203d 205b 5d0d 0a72 6561 646d 6520 3d20   = []..readme = 
+000000d0: 2252 4541 444d 452e 6d64 220d 0a6b 6579  "README.md"..key
+000000e0: 776f 7264 7320 3d20 5b5d 0d0a 636c 6173  words = []..clas
+000000f0: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
+00000100: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
+00000110: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000120: 203a 3a20 3322 2c0d 0a20 2020 2022 4c69   :: 3",..    "Li
+00000130: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000140: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000150: 656e 7365 222c 0d0a 2020 2020 224f 7065  ense",..    "Ope
+00000160: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000170: 204f 5320 496e 6465 7065 6e64 656e 7422   OS Independent"
+00000180: 2c0d 0a20 2020 205d 0d0a 0d0a 5b70 726f  ,..    ]....[pro
+00000190: 6a65 6374 2e75 726c 735d 0d0a 2248 6f6d  ject.urls].."Hom
+000001a0: 6570 6167 6522 203d 2022 220d 0a22 446f  epage" = "".."Do
+000001b0: 6375 6d65 6e74 6174 696f 6e22 203d 2022  cumentation" = "
+000001c0: 220d 0a22 536f 7572 6365 2063 6f64 6522  ".."Source code"
+000001d0: 203d 2022 220d 0a0d 0a5b 746f 6f6c 2e70   = ""....[tool.p
+000001e0: 7974 6573 742e 696e 695f 6f70 7469 6f6e  ytest.ini_option
+000001f0: 735d 0d0a 6164 646f 7074 7320 3d20 5b0d  s]..addopts = [.
+00000200: 0a20 2020 2022 2d2d 696d 706f 7274 2d6d  .    "--import-m
+00000210: 6f64 653d 696d 706f 7274 6c69 6222 2c0d  ode=importlib",.
+00000220: 0a20 2020 205d 0d0a 7079 7468 6f6e 7061  .    ]..pythonpa
+00000230: 7468 203d 2022 7372 6322 0d0a 0d0a 5b74  th = "src"....[t
+00000240: 6f6f 6c2e 6861 7463 682e 6275 696c 642e  ool.hatch.build.
+00000250: 7461 7267 6574 732e 7364 6973 745d 0d0a  targets.sdist]..
+00000260: 6578 636c 7564 6520 3d20 5b0d 0a20 2020  exclude = [..   
+00000270: 2022 2e63 6f76 6572 6167 6522 2c0d 0a20   ".coverage",.. 
+00000280: 2020 2022 2e70 7974 6573 745f 6361 6368     ".pytest_cach
+00000290: 6522 2c0d 0a20 2020 2022 2e76 7363 6f64  e",..    ".vscod
+000002a0: 6522 2c0d 0a20 2020 2022 7465 7374 7322  e",..    "tests"
+000002b0: 2c0d 0a20 2020 2022 2e67 6974 6967 6e6f  ,..    ".gitigno
+000002c0: 7265 220d 0a20 2020 205d 0d0a 5b70 726f  re"..    ]..[pro
+000002d0: 6a65 6374 2e73 6372 6970 7473 5d         ject.scripts]
```

### Comparing `hassle-2.7.0/src/hassle/run_tests.py` & `hassle-2.7.1/src/hassle/run_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/LICENSE.txt` & `hassle-2.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/README.md` & `hassle-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.7.0/pyproject.toml` & `hassle-2.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 372e 3022 0d0a 7265 7175 6972 6573  2.7.0"..requires
+00000100: 322e 372e 3122 0d0a 7265 7175 6972 6573  2.7.1"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..
```

### Comparing `hassle-2.7.0/PKG-INFO` & `hassle-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.7.0
+Version: 2.7.1
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

