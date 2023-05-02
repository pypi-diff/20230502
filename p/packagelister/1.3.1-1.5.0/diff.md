# Comparing `tmp/packagelister-1.3.1.tar.gz` & `tmp/packagelister-1.5.0.tar.gz`

## Comparing `packagelister-1.3.1.tar` & `packagelister-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 packagelister-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/index.html
--rw-r--r--   0        0        0    34264 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister.html
--rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/search.js
--rw-r--r--   0        0        0    69236 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister/packagelister.html
--rw-r--r--   0        0        0    74342 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister/packagelister_cli.html
--rw-r--r--   0        0        0    56419 2020-02-02 00:00:00.000000 packagelister-1.3.1/docs/packagelister/whouses.html
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/__init__.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/packagelister.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/packagelister_cli.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 packagelister-1.3.1/src/packagelister/whouses.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.3.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.3.1/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 packagelister-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 packagelister-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 packagelister-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.5.0/docs/index.html
+-rw-r--r--   0        0        0    34336 2020-02-02 00:00:00.000000 packagelister-1.5.0/docs/packagelister.html
+-rw-r--r--   0        0        0    25388 2020-02-02 00:00:00.000000 packagelister-1.5.0/docs/search.js
+-rw-r--r--   0        0        0    93521 2020-02-02 00:00:00.000000 packagelister-1.5.0/docs/packagelister/packagelister.html
+-rw-r--r--   0        0        0    74342 2020-02-02 00:00:00.000000 packagelister-1.5.0/docs/packagelister/packagelister_cli.html
+-rw-r--r--   0        0        0    56419 2020-02-02 00:00:00.000000 packagelister-1.5.0/docs/packagelister/whouses.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 packagelister-1.5.0/src/packagelister/__init__.py
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 packagelister-1.5.0/src/packagelister/packagelister.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 packagelister-1.5.0/src/packagelister/packagelister_cli.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 packagelister-1.5.0/src/packagelister/whouses.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.5.0/README.md
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 packagelister-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 packagelister-1.5.0/PKG-INFO
```

### Comparing `packagelister-1.3.1/docs/packagelister.html` & `packagelister-1.5.0/docs/packagelister.html`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 packagelister    </h1>
 
                 
                         <input id="mod-packagelister-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-packagelister-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">.packagelister</span> <span class="kn">import</span> <span class="n">scan</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">.packagelister</span> <span class="kn">import</span> <span class="n">get_packages_from_source</span><span class="p">,</span> <span class="n">scan</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -6,9 +6,9 @@
     * packagelister
     * packagelister_cli
     * whouses
 built_with_pdoc[pdoc_logo]
 
 ****** packagelister ******
 ⁰ View Source
-1from .packagelister import scan
+1from .packagelister import get_packages_from_source, scan
```

### Comparing `packagelister-1.3.1/docs/search.js` & `packagelister-1.5.0/docs/search.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -689,14 +689,30 @@
         "doc": "<p></p>\n"
     }, {
         "fullname": "packagelister.packagelister",
         "modulename": "packagelister.packagelister",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
+        "fullname": "packagelister.packagelister.get_packages_from_source",
+        "modulename": "packagelister.packagelister",
+        "qualname": "get_packages_from_source",
+        "kind": "function",
+        "doc": "<p>Scan <code>source</code> and extract the names of imported packages/modules.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>recursive</code>: Extract modules/packages that are imported by <code>source</code>'s imports\nand those imports' imports and those imports' imports...</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">source</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">recursive</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>:</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "packagelister.packagelister.remove_builtins",
+        "modulename": "packagelister.packagelister",
+        "qualname": "remove_builtins",
+        "kind": "function",
+        "doc": "<p>Remove built in packages/modules from a list of package names.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">packages</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>:</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "packagelister.packagelister.scan",
         "modulename": "packagelister.packagelister",
         "qualname": "scan",
         "kind": "function",
         "doc": "<p>Recursively scans a directory for python files to determine\nwhat packages are in use, as well as the version number\nif applicable.</p>\n\n<p>Returns a dictionary where the keys are package\nnames and the values are the version number of the package if there is one\n(None if there isn't) and a list of the files that import the package.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>project_dir</strong>:  Can be an absolute or relative path\nto a directory or a single file (.py).\nIf it is relative, it will be assumed to be relative to\nthe current working directory.\nIf an argument isn't given, the current working directory\nwill be scanned.\nIf the path doesn't exist, an empty dictionary is returned.</li>\n</ul>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">project_dir</span><span class=\"p\">:</span> <span class=\"n\">pathlib</span><span class=\"o\">.</span><span class=\"n\">Path</span> <span class=\"o\">|</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">include_builtins</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">dict</span>:</span></span>",
         "funcdef": "def"
```

### Comparing `packagelister-1.3.1/docs/packagelister/packagelister.html` & `packagelister-1.5.0/docs/packagelister/packagelister_cli.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html lang="en">
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <meta name="generator" content="pdoc 12.3.1"/>
-    <title>packagelister.packagelister API documentation</title>
+    <title>packagelister.packagelister_cli API documentation</title>
 
     <style>/*! * Bootstrap Reboot v5.0.0 (https://getbootstrap.com/) * Copyright 2011-2021 The Bootstrap Authors * Copyright 2011-2021 Twitter, Inc. * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE) * Forked from Normalize.css, licensed MIT (https://github.com/necolas/normalize.css/blob/master/LICENSE.md) */*,::after,::before{box-sizing:border-box}@media (prefers-reduced-motion:no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans","Liberation Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:transparent}hr{margin:1rem 0;color:inherit;background-color:currentColor;border:0;opacity:.25}hr:not([size]){height:1px}h1,h2,h3,h4,h5,h6{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width:1200px){h1{font-size:2.5rem}}h2{font-size:calc(1.325rem + .9vw)}@media (min-width:1200px){h2{font-size:2rem}}h3{font-size:calc(1.3rem + .6vw)}@media (min-width:1200px){h3{font-size:1.75rem}}h4{font-size:calc(1.275rem + .3vw)}@media (min-width:1200px){h4{font-size:1.5rem}}h5{font-size:1.25rem}h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[data-bs-original-title],abbr[title]{-webkit-text-decoration:underline dotted;text-decoration:underline dotted;cursor:help;-webkit-text-decoration-skip-ink:none;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}dl,ol,ul{margin-top:0;margin-bottom:1rem}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small{font-size:.875em}mark{padding:.2em;background-color:#fcf8e3}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:#0d6efd;text-decoration:underline}a:hover{color:#0a58ca}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}code,kbd,pre,samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;font-size:1em;direction:ltr;unicode-bidi:bidi-override}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:#d63384;word-wrap:break-word}a>code{color:inherit}kbd{padding:.2rem .4rem;font-size:.875em;color:#fff;background-color:#212529;border-radius:.2rem}kbd kbd{padding:0;font-size:1em;font-weight:700}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}tbody,td,tfoot,th,thead,tr{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]::-webkit-calendar-picker-indicator{display:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled),button:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width:1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-text,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}</style>
     <style>/*! syntax-highlighting.css */pre{line-height:125%;}span.linenos{color:inherit; background-color:transparent; padding-left:5px; padding-right:20px;}.pdoc-code .hll{background-color:#ffffcc}.pdoc-code{background:#f8f8f8;}.pdoc-code .c{color:#3D7B7B; font-style:italic}.pdoc-code .err{border:1px solid #FF0000}.pdoc-code .k{color:#008000; font-weight:bold}.pdoc-code .o{color:#666666}.pdoc-code .ch{color:#3D7B7B; font-style:italic}.pdoc-code .cm{color:#3D7B7B; font-style:italic}.pdoc-code .cp{color:#9C6500}.pdoc-code .cpf{color:#3D7B7B; font-style:italic}.pdoc-code .c1{color:#3D7B7B; font-style:italic}.pdoc-code .cs{color:#3D7B7B; font-style:italic}.pdoc-code .gd{color:#A00000}.pdoc-code .ge{font-style:italic}.pdoc-code .gr{color:#E40000}.pdoc-code .gh{color:#000080; font-weight:bold}.pdoc-code .gi{color:#008400}.pdoc-code .go{color:#717171}.pdoc-code .gp{color:#000080; font-weight:bold}.pdoc-code .gs{font-weight:bold}.pdoc-code .gu{color:#800080; font-weight:bold}.pdoc-code .gt{color:#0044DD}.pdoc-code .kc{color:#008000; font-weight:bold}.pdoc-code .kd{color:#008000; font-weight:bold}.pdoc-code .kn{color:#008000; font-weight:bold}.pdoc-code .kp{color:#008000}.pdoc-code .kr{color:#008000; font-weight:bold}.pdoc-code .kt{color:#B00040}.pdoc-code .m{color:#666666}.pdoc-code .s{color:#BA2121}.pdoc-code .na{color:#687822}.pdoc-code .nb{color:#008000}.pdoc-code .nc{color:#0000FF; font-weight:bold}.pdoc-code .no{color:#880000}.pdoc-code .nd{color:#AA22FF}.pdoc-code .ni{color:#717171; font-weight:bold}.pdoc-code .ne{color:#CB3F38; font-weight:bold}.pdoc-code .nf{color:#0000FF}.pdoc-code .nl{color:#767600}.pdoc-code .nn{color:#0000FF; font-weight:bold}.pdoc-code .nt{color:#008000; font-weight:bold}.pdoc-code .nv{color:#19177C}.pdoc-code .ow{color:#AA22FF; font-weight:bold}.pdoc-code .w{color:#bbbbbb}.pdoc-code .mb{color:#666666}.pdoc-code .mf{color:#666666}.pdoc-code .mh{color:#666666}.pdoc-code .mi{color:#666666}.pdoc-code .mo{color:#666666}.pdoc-code .sa{color:#BA2121}.pdoc-code .sb{color:#BA2121}.pdoc-code .sc{color:#BA2121}.pdoc-code .dl{color:#BA2121}.pdoc-code .sd{color:#BA2121; font-style:italic}.pdoc-code .s2{color:#BA2121}.pdoc-code .se{color:#AA5D1F; font-weight:bold}.pdoc-code .sh{color:#BA2121}.pdoc-code .si{color:#A45A77; font-weight:bold}.pdoc-code .sx{color:#008000}.pdoc-code .sr{color:#A45A77}.pdoc-code .s1{color:#BA2121}.pdoc-code .ss{color:#19177C}.pdoc-code .bp{color:#008000}.pdoc-code .fm{color:#0000FF}.pdoc-code .vc{color:#19177C}.pdoc-code .vg{color:#19177C}.pdoc-code .vi{color:#19177C}.pdoc-code .vm{color:#19177C}.pdoc-code .il{color:#666666}</style>
     <style>/*! theme.css */:root{--pdoc-background:#fff;}.pdoc{--text:#212529;--muted:#6c757d;--link:#3660a5;--link-hover:#1659c5;--code:#f8f8f8;--active:#fff598;--accent:#eee;--accent2:#c1c1c1;--nav-hover:rgba(255, 255, 255, 0.5);--name:#0066BB;--def:#008800;--annotation:#007020;}</style>
     <style>/*! layout.css */html, body{width:100%;height:100%;}html, main{scroll-behavior:smooth;}body{background-color:var(--pdoc-background);}@media (max-width:769px){#navtoggle{cursor:pointer;position:absolute;width:50px;height:40px;top:1rem;right:1rem;border-color:var(--text);color:var(--text);display:flex;opacity:0.8;}#navtoggle:hover{opacity:1;}#togglestate + div{display:none;}#togglestate:checked + div{display:inherit;}main, header{padding:2rem 3vw;}header + main{margin-top:-3rem;}.git-button{display:none !important;}nav input[type="search"]{max-width:77%;}nav input[type="search"]:first-child{margin-top:-6px;}nav input[type="search"]:valid ~ *{display:none !important;}}@media (min-width:770px){:root{--sidebar-width:clamp(12.5rem, 28vw, 22rem);}nav{position:fixed;overflow:auto;height:100vh;width:var(--sidebar-width);}main, header{padding:3rem 2rem 3rem calc(var(--sidebar-width) + 3rem);width:calc(54rem + var(--sidebar-width));max-width:100%;}header + main{margin-top:-4rem;}#navtoggle{display:none;}}#togglestate{position:absolute;height:0;opacity:0;}nav.pdoc{--pad:clamp(0.5rem, 2vw, 1.75rem);--indent:1.5rem;background-color:var(--accent);border-right:1px solid var(--accent2);box-shadow:0 0 20px rgba(50, 50, 50, .2) inset;padding:0 0 0 var(--pad);overflow-wrap:anywhere;scrollbar-width:thin; scrollbar-color:var(--accent2) transparent }nav.pdoc::-webkit-scrollbar{width:.4rem; }nav.pdoc::-webkit-scrollbar-thumb{background-color:var(--accent2); }nav.pdoc > div{padding:var(--pad) 0;}nav.pdoc .module-list-button{display:inline-flex;align-items:center;color:var(--text);border-color:var(--muted);margin-bottom:1rem;}nav.pdoc .module-list-button:hover{border-color:var(--text);}nav.pdoc input[type=search]{display:block;outline-offset:0;width:calc(100% - var(--pad));}nav.pdoc .logo{max-width:calc(100% - var(--pad));max-height:35vh;display:block;margin:0 auto 1rem;transform:translate(calc(-.5 * var(--pad)), 0);}nav.pdoc ul{list-style:none;padding-left:0;}nav.pdoc > div > ul{margin-left:calc(0px - var(--pad));}nav.pdoc li a{padding:.2rem 0 .2rem calc(var(--pad) + var(--indent));}nav.pdoc > div > ul > li > a{padding-left:var(--pad);}nav.pdoc li{transition:all 100ms;}nav.pdoc li:hover{background-color:var(--nav-hover);}nav.pdoc a, nav.pdoc a:hover{color:var(--text);}nav.pdoc a{display:block;}nav.pdoc > h2:first-of-type{margin-top:1.5rem;}nav.pdoc .class:before{content:"class ";color:var(--muted);}nav.pdoc .function:after{content:"()";color:var(--muted);}nav.pdoc footer:before{content:"";display:block;width:calc(100% - var(--pad));border-top:solid var(--accent2) 1px;margin-top:1.5rem;padding-top:.5rem;}nav.pdoc footer{font-size:small;}</style>
     <style>/*! content.css */.pdoc{color:var(--text);box-sizing:border-box;line-height:1.5;background:none;}.pdoc .pdoc-button{display:inline-block;border:solid black 1px;border-radius:2px;font-size:.75rem;padding:calc(0.5em - 1px) 1em;transition:100ms all;}.pdoc .pdoc-alert{padding:1rem 1rem 1rem calc(1.5rem + 24px);border:1px solid transparent;border-radius:.25rem;background-repeat:no-repeat;background-position:1rem center;margin-bottom:1rem;}.pdoc .pdoc-alert > *:last-child{margin-bottom:0;}.pdoc .pdoc-alert-note {color:#084298;background-color:#cfe2ff;border-color:#b6d4fe;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23084298%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8%2016A8%208%200%201%200%208%200a8%208%200%200%200%200%2016zm.93-9.412-1%204.705c-.07.34.029.533.304.533.194%200%20.487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703%200-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381%202.29-.287zM8%205.5a1%201%200%201%201%200-2%201%201%200%200%201%200%202z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-warning{color:#664d03;background-color:#fff3cd;border-color:#ffecb5;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23664d03%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8.982%201.566a1.13%201.13%200%200%200-1.96%200L.165%2013.233c-.457.778.091%201.767.98%201.767h13.713c.889%200%201.438-.99.98-1.767L8.982%201.566zM8%205c.535%200%20.954.462.9.995l-.35%203.507a.552.552%200%200%201-1.1%200L7.1%205.995A.905.905%200%200%201%208%205zm.002%206a1%201%200%201%201%200%202%201%201%200%200%201%200-2z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-danger{color:#842029;background-color:#f8d7da;border-color:#f5c2c7;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23842029%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M5.52.359A.5.5%200%200%201%206%200h4a.5.5%200%200%201%20.474.658L8.694%206H12.5a.5.5%200%200%201%20.395.807l-7%209a.5.5%200%200%201-.873-.454L6.823%209.5H3.5a.5.5%200%200%201-.48-.641l2.5-8.5z%22/%3E%3C/svg%3E");}.pdoc .visually-hidden{position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important;}.pdoc h1, .pdoc h2, .pdoc h3{font-weight:300;margin:.3em 0;padding:.2em 0;}.pdoc > section:not(.module-info) h1{font-size:1.5rem;font-weight:500;}.pdoc > section:not(.module-info) h2{font-size:1.4rem;font-weight:500;}.pdoc > section:not(.module-info) h3{font-size:1.3rem;font-weight:500;}.pdoc > section:not(.module-info) h4{font-size:1.2rem;}.pdoc > section:not(.module-info) h5{font-size:1.1rem;}.pdoc a{text-decoration:none;color:var(--link);}.pdoc a:hover{color:var(--link-hover);}.pdoc blockquote{margin-left:2rem;}.pdoc pre{border-top:1px solid var(--accent2);border-bottom:1px solid var(--accent2);margin-top:0;margin-bottom:1em;padding:.5rem 0 .5rem .5rem;overflow-x:auto;background-color:var(--code);}.pdoc code{color:var(--text);padding:.2em .4em;margin:0;font-size:85%;background-color:var(--code);border-radius:6px;}.pdoc a > code{color:inherit;}.pdoc pre > code{display:inline-block;font-size:inherit;background:none;border:none;padding:0;}.pdoc > section:not(.module-info){margin-bottom:1.5rem;}.pdoc .modulename{margin-top:0;font-weight:bold;}.pdoc .modulename a{color:var(--link);transition:100ms all;}.pdoc .git-button{float:right;border:solid var(--link) 1px;}.pdoc .git-button:hover{background-color:var(--link);color:var(--pdoc-background);}.view-source-toggle-state,.view-source-toggle-state ~ .pdoc-code{display:none;}.view-source-toggle-state:checked ~ .pdoc-code{display:block;}.view-source-button{display:inline-block;float:right;font-size:.75rem;line-height:1.5rem;color:var(--muted);padding:0 .4rem 0 1.3rem;cursor:pointer;text-indent:-2px;}.view-source-button > span{visibility:hidden;}.module-info .view-source-button{float:none;display:flex;justify-content:flex-end;margin:-1.2rem .4rem -.2rem 0;}.view-source-button::before{position:absolute;content:"View Source";display:list-item;list-style-type:disclosure-closed;}.view-source-toggle-state:checked ~ .attr .view-source-button::before,.view-source-toggle-state:checked ~ .view-source-button::before{list-style-type:disclosure-open;}.pdoc .docstring{margin-bottom:1.5rem;}.pdoc section:not(.module-info) .docstring{margin-left:clamp(0rem, 5vw - 2rem, 1rem);}.pdoc .docstring .pdoc-code{margin-left:1em;margin-right:1em;}.pdoc h1:target,.pdoc h2:target,.pdoc h3:target,.pdoc h4:target,.pdoc h5:target,.pdoc h6:target,.pdoc .pdoc-code > pre > span:target{background-color:var(--active);box-shadow:-1rem 0 0 0 var(--active);}.pdoc .pdoc-code > pre > span:target{display:block;}.pdoc div:target > .attr,.pdoc section:target > .attr,.pdoc dd:target > a{background-color:var(--active);}.pdoc *{scroll-margin:2rem;}.pdoc .pdoc-code .linenos{user-select:none;}.pdoc .attr:hover{filter:contrast(0.95);}.pdoc section, .pdoc .classattr{position:relative;}.pdoc .headerlink{--width:clamp(1rem, 3vw, 2rem);position:absolute;top:0;left:calc(0rem - var(--width));transition:all 100ms ease-in-out;opacity:0;}.pdoc .headerlink::before{content:"#";display:block;text-align:center;width:var(--width);height:2.3rem;line-height:2.3rem;font-size:1.5rem;}.pdoc .attr:hover ~ .headerlink,.pdoc *:target > .headerlink,.pdoc .headerlink:hover{opacity:1;}.pdoc .attr{display:block;margin:.5rem 0 .5rem;padding:.4rem .4rem .4rem 1rem;background-color:var(--accent);overflow-x:auto;}.pdoc .classattr{margin-left:2rem;}.pdoc .name{color:var(--name);font-weight:bold;}.pdoc .def{color:var(--def);font-weight:bold;}.pdoc .signature{background-color:transparent;}.pdoc .param, .pdoc .return-annotation{white-space:pre;}.pdoc .signature.multiline .param{display:block;}.pdoc .signature.condensed .param{display:inline-block;}.pdoc .annotation{color:var(--annotation);}.pdoc .inherited{margin-left:2rem;}.pdoc .inherited dt{font-weight:700;}.pdoc .inherited dt, .pdoc .inherited dd{display:inline;margin-left:0;margin-bottom:.5rem;}.pdoc .inherited dd:not(:last-child):after{content:", ";}.pdoc .inherited .class:before{content:"class ";}.pdoc .inherited .function a:after{content:"()";}.pdoc .search-result .docstring{overflow:auto;max-height:25vh;}.pdoc .search-result.focused > .attr{background-color:var(--active);}.pdoc .attribution{margin-top:2rem;display:block;opacity:0.5;transition:all 200ms;filter:grayscale(100%);}.pdoc .attribution:hover{opacity:1;filter:grayscale(0%);}.pdoc .attribution img{margin-left:5px;height:35px;vertical-align:middle;width:70px;transition:all 200ms;}.pdoc table{display:block;width:max-content;max-width:100%;overflow:auto;margin-bottom:1rem;}.pdoc table th{font-weight:600;}.pdoc table th, .pdoc table td{padding:6px 13px;border:1px solid var(--accent2);}</style>
     <style>/*! custom.css */</style></head>
@@ -27,15 +27,15 @@
                    pattern=".+" required>
 
 
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
-                    <a class="function" href="#scan">scan</a>
+                    <a class="function" href="#main">main</a>
             </li>
     </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
@@ -43,198 +43,222 @@
                 src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20role%3D%22img%22%20aria-label%3D%22pdoc%20logo%22%20width%3D%22300%22%20height%3D%22150%22%20viewBox%3D%22-1%200%2060%2030%22%3E%3Ctitle%3Epdoc%3C/title%3E%3Cpath%20d%3D%22M29.621%2021.293c-.011-.273-.214-.475-.511-.481a.5.5%200%200%200-.489.503l-.044%201.393c-.097.551-.695%201.215-1.566%201.704-.577.428-1.306.486-2.193.182-1.426-.617-2.467-1.654-3.304-2.487l-.173-.172a3.43%203.43%200%200%200-.365-.306.49.49%200%200%200-.286-.196c-1.718-1.06-4.931-1.47-7.353.191l-.219.15c-1.707%201.187-3.413%202.131-4.328%201.03-.02-.027-.49-.685-.141-1.763.233-.721.546-2.408.772-4.076.042-.09.067-.187.046-.288.166-1.347.277-2.625.241-3.351%201.378-1.008%202.271-2.586%202.271-4.362%200-.976-.272-1.935-.788-2.774-.057-.094-.122-.18-.184-.268.033-.167.052-.339.052-.516%200-1.477-1.202-2.679-2.679-2.679-.791%200-1.496.352-1.987.9a6.3%206.3%200%200%200-1.001.029c-.492-.564-1.207-.929-2.012-.929-1.477%200-2.679%201.202-2.679%202.679A2.65%202.65%200%200%200%20.97%206.554c-.383.747-.595%201.572-.595%202.41%200%202.311%201.507%204.29%203.635%205.107-.037.699-.147%202.27-.423%203.294l-.137.461c-.622%202.042-2.515%208.257%201.727%2010.643%201.614.908%203.06%201.248%204.317%201.248%202.665%200%204.492-1.524%205.322-2.401%201.476-1.559%202.886-1.854%206.491.82%201.877%201.393%203.514%201.753%204.861%201.068%202.223-1.713%202.811-3.867%203.399-6.374.077-.846.056-1.469.054-1.537zm-4.835%204.313c-.054.305-.156.586-.242.629-.034-.007-.131-.022-.307-.157-.145-.111-.314-.478-.456-.908.221.121.432.25.675.355.115.039.219.051.33.081zm-2.251-1.238c-.05.33-.158.648-.252.694-.022.001-.125-.018-.307-.157-.217-.166-.488-.906-.639-1.573.358.344.754.693%201.198%201.036zm-3.887-2.337c-.006-.116-.018-.231-.041-.342.635.145%201.189.368%201.599.625.097.231.166.481.174.642-.03.049-.055.101-.067.158-.046.013-.128.026-.298.004-.278-.037-.901-.57-1.367-1.087zm-1.127-.497c.116.306.176.625.12.71-.019.014-.117.045-.345.016-.206-.027-.604-.332-.986-.695.41-.051.816-.056%201.211-.031zm-4.535%201.535c.209.22.379.47.358.598-.006.041-.088.138-.351.234-.144.055-.539-.063-.979-.259a11.66%2011.66%200%200%200%20.972-.573zm.983-.664c.359-.237.738-.418%201.126-.554.25.237.479.548.457.694-.006.042-.087.138-.351.235-.174.064-.694-.105-1.232-.375zm-3.381%201.794c-.022.145-.061.29-.149.401-.133.166-.358.248-.69.251h-.002c-.133%200-.306-.26-.45-.621.417.091.854.07%201.291-.031zm-2.066-8.077a4.78%204.78%200%200%201-.775-.584c.172-.115.505-.254.88-.378l-.105.962zm-.331%202.302a10.32%2010.32%200%200%201-.828-.502c.202-.143.576-.328.984-.49l-.156.992zm-.45%202.157l-.701-.403c.214-.115.536-.249.891-.376a11.57%2011.57%200%200%201-.19.779zm-.181%201.716c.064.398.194.702.298.893-.194-.051-.435-.162-.736-.398.061-.119.224-.3.438-.495zM8.87%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zm-.735-.389a1.15%201.15%200%200%200-.314.783%201.16%201.16%200%200%200%201.162%201.162c.457%200%20.842-.27%201.032-.653.026.117.042.238.042.362a1.68%201.68%200%200%201-1.679%201.679%201.68%201.68%200%200%201-1.679-1.679c0-.843.626-1.535%201.436-1.654zM5.059%205.406A1.68%201.68%200%200%201%203.38%207.085a1.68%201.68%200%200%201-1.679-1.679c0-.037.009-.072.011-.109.21.3.541.508.935.508a1.16%201.16%200%200%200%201.162-1.162%201.14%201.14%200%200%200-.474-.912c.015%200%20.03-.005.045-.005.926.001%201.679.754%201.679%201.68zM3.198%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zM1.375%208.964c0-.52.103-1.035.288-1.52.466.394%201.06.64%201.717.64%201.144%200%202.116-.725%202.499-1.738.383%201.012%201.355%201.738%202.499%201.738.867%200%201.631-.421%202.121-1.062.307.605.478%201.267.478%201.942%200%202.486-2.153%204.51-4.801%204.51s-4.801-2.023-4.801-4.51zm24.342%2019.349c-.985.498-2.267.168-3.813-.979-3.073-2.281-5.453-3.199-7.813-.705-1.315%201.391-4.163%203.365-8.423.97-3.174-1.786-2.239-6.266-1.261-9.479l.146-.492c.276-1.02.395-2.457.444-3.268a6.11%206.11%200%200%200%201.18.115%206.01%206.01%200%200%200%202.536-.562l-.006.175c-.802.215-1.848.612-2.021%201.25-.079.295.021.601.274.837.219.203.415.364.598.501-.667.304-1.243.698-1.311%201.179-.02.144-.022.507.393.787.213.144.395.26.564.365-1.285.521-1.361.96-1.381%201.126-.018.142-.011.496.427.746l.854.489c-.473.389-.971.914-.999%201.429-.018.278.095.532.316.713.675.556%201.231.721%201.653.721.059%200%20.104-.014.158-.02.207.707.641%201.64%201.513%201.64h.013c.8-.008%201.236-.345%201.462-.626.173-.216.268-.457.325-.692.424.195.93.374%201.372.374.151%200%20.294-.021.423-.068.732-.27.944-.704.993-1.021.009-.061.003-.119.002-.179.266.086.538.147.789.147.15%200%20.294-.021.423-.069.542-.2.797-.489.914-.754.237.147.478.258.704.288.106.014.205.021.296.021.356%200%20.595-.101.767-.229.438.435%201.094.992%201.656%201.067.106.014.205.021.296.021a1.56%201.56%200%200%200%20.323-.035c.17.575.453%201.289.866%201.605.358.273.665.362.914.362a.99.99%200%200%200%20.421-.093%201.03%201.03%200%200%200%20.245-.164c.168.428.39.846.68%201.068.358.273.665.362.913.362a.99.99%200%200%200%20.421-.093c.317-.148.512-.448.639-.762.251.157.495.257.726.257.127%200%20.25-.024.37-.071.427-.17.706-.617.841-1.314.022-.015.047-.022.068-.038.067-.051.133-.104.196-.159-.443%201.486-1.107%202.761-2.086%203.257zM8.66%209.925a.5.5%200%201%200-1%200c0%20.653-.818%201.205-1.787%201.205s-1.787-.552-1.787-1.205a.5.5%200%201%200-1%200c0%201.216%201.25%202.205%202.787%202.205s2.787-.989%202.787-2.205zm4.4%2015.965l-.208.097c-2.661%201.258-4.708%201.436-6.086.527-1.542-1.017-1.88-3.19-1.844-4.198a.4.4%200%200%200-.385-.414c-.242-.029-.406.164-.414.385-.046%201.249.367%203.686%202.202%204.896.708.467%201.547.7%202.51.7%201.248%200%202.706-.392%204.362-1.174l.185-.086a.4.4%200%200%200%20.205-.527c-.089-.204-.326-.291-.527-.206zM9.547%202.292c.093.077.205.114.317.114a.5.5%200%200%200%20.318-.886L8.817.397a.5.5%200%200%200-.703.068.5.5%200%200%200%20.069.703l1.364%201.124zm-7.661-.065c.086%200%20.173-.022.253-.068l1.523-.893a.5.5%200%200%200-.506-.863l-1.523.892a.5.5%200%200%200-.179.685c.094.158.261.247.432.247z%22%20transform%3D%22matrix%28-1%200%200%201%2058%200%29%22%20fill%3D%22%233bb300%22/%3E%3Cpath%20d%3D%22M.3%2021.86V10.18q0-.46.02-.68.04-.22.18-.5.28-.54%201.34-.54%201.06%200%201.42.28.38.26.44.78.76-1.04%202.38-1.04%201.64%200%203.1%201.54%201.46%201.54%201.46%203.58%200%202.04-1.46%203.58-1.44%201.54-3.08%201.54-1.64%200-2.38-.92v4.04q0%20.46-.04.68-.02.22-.18.5-.14.3-.5.42-.36.12-.98.12-.62%200-1-.12-.36-.12-.52-.4-.14-.28-.18-.5-.02-.22-.02-.68zm3.96-9.42q-.46.54-.46%201.18%200%20.64.46%201.18.48.52%201.2.52.74%200%201.24-.52.52-.52.52-1.18%200-.66-.48-1.18-.48-.54-1.26-.54-.76%200-1.22.54zm14.741-8.36q.16-.3.54-.42.38-.12%201-.12.64%200%201.02.12.38.12.52.42.16.3.18.54.04.22.04.68v11.94q0%20.46-.04.7-.02.22-.18.5-.3.54-1.7.54-1.38%200-1.54-.98-.84.96-2.34.96-1.8%200-3.28-1.56-1.48-1.58-1.48-3.66%200-2.1%201.48-3.68%201.5-1.58%203.28-1.58%201.48%200%202.3%201v-4.2q0-.46.02-.68.04-.24.18-.52zm-3.24%2010.86q.52.54%201.26.54.74%200%201.22-.54.5-.54.5-1.18%200-.66-.48-1.22-.46-.56-1.26-.56-.8%200-1.28.56-.48.54-.48%201.2%200%20.66.52%201.2zm7.833-1.2q0-2.4%201.68-3.96%201.68-1.56%203.84-1.56%202.16%200%203.82%201.56%201.66%201.54%201.66%203.94%200%201.66-.86%202.96-.86%201.28-2.1%201.9-1.22.6-2.54.6-1.32%200-2.56-.64-1.24-.66-2.1-1.92-.84-1.28-.84-2.88zm4.18%201.44q.64.48%201.3.48.66%200%201.32-.5.66-.5.66-1.48%200-.98-.62-1.46-.62-.48-1.34-.48-.72%200-1.34.5-.62.5-.62%201.48%200%20.96.64%201.46zm11.412-1.44q0%20.84.56%201.32.56.46%201.18.46.64%200%201.18-.36.56-.38.9-.38.6%200%201.46%201.06.46.58.46%201.04%200%20.76-1.1%201.42-1.14.8-2.8.8-1.86%200-3.58-1.34-.82-.64-1.34-1.7-.52-1.08-.52-2.36%200-1.3.52-2.34.52-1.06%201.34-1.7%201.66-1.32%203.54-1.32.76%200%201.48.22.72.2%201.06.4l.32.2q.36.24.56.38.52.4.52.92%200%20.5-.42%201.14-.72%201.1-1.38%201.1-.38%200-1.08-.44-.36-.34-1.04-.34-.66%200-1.24.48-.58.48-.58%201.34z%22%20fill%3D%22green%22/%3E%3C/svg%3E"/>
         </a>
 </div>
     </nav>
     <main class="pdoc">
             <section class="module-info">
                     <h1 class="modulename">
-<a href="./../packagelister.html">packagelister</a><wbr>.packagelister    </h1>
+<a href="./../packagelister.html">packagelister</a><wbr>.packagelister_cli    </h1>
 
                 
-                        <input id="mod-packagelister-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                        <input id="mod-packagelister_cli-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
-                        <label class="view-source-button" for="mod-packagelister-view-source"><span>View Source</span></label>
+                        <label class="view-source-button" for="mod-packagelister_cli-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">import</span> <span class="nn">importlib.metadata</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">import</span> <span class="nn">sys</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="kn">from</span> <span class="nn">pathcrawler</span> <span class="kn">import</span> <span class="n">crawl</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">ProgBar</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="k">def</span> <span class="nf">scan</span><span class="p">(</span><span class="n">project_dir</span><span class="p">:</span> <span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="sd">&quot;&quot;&quot;Recursively scans a directory for python files to determine</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="sd">    what packages are in use, as well as the version number</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a><span class="sd">    if applicable.</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>
-</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="sd">    Returns a dictionary where the keys are package</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="sd">    names and the values are the version number of the package if there is one</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a><span class="sd">    (None if there isn&#39;t) and a list of the files that import the package.</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>
-</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="sd">    :param project_dir: Can be an absolute or relative path</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a><span class="sd">    to a directory or a single file (.py).</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a><span class="sd">    If it is relative, it will be assumed to be relative to</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a><span class="sd">    the current working directory.</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a><span class="sd">    If an argument isn&#39;t given, the current working directory</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a><span class="sd">    will be scanned.</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a><span class="sd">    If the path doesn&#39;t exist, an empty dictionary is returned.&quot;&quot;&quot;</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="p">:</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>    <span class="k">elif</span> <span class="nb">type</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>
-</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="c1"># Return empty dict if project_dir doesn&#39;t exist</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>        <span class="k">return</span> <span class="p">{}</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">crawl</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">suffix</span> <span class="o">==</span> <span class="s2">&quot;.py&quot;</span><span class="p">]</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>    <span class="c1"># If scanning one file, the progress bar will show 0% complete if bar.counter == 0</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="n">standard_lib</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span> <span class="k">else</span> <span class="p">[]</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>        <span class="n">contents</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>            <span class="n">line</span><span class="o">.</span><span class="n">split</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>            <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="s2">&quot;utf-8&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a>            <span class="k">if</span> <span class="n">line</span><span class="o">.</span><span class="n">startswith</span><span class="p">((</span><span class="s2">&quot;from&quot;</span><span class="p">,</span> <span class="s2">&quot;import&quot;</span><span class="p">))</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>        <span class="p">]</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">contents</span><span class="p">:</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos">55</span></a>            <span class="k">if</span> <span class="n">package</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">):</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos">56</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos">57</span></a>            <span class="k">if</span> <span class="s2">&quot;.&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos">58</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[:</span> <span class="n">package</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos">59</span></a>            <span class="k">if</span> <span class="s2">&quot;,&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos">60</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[:</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos">61</span></a>            <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">files</span> <span class="ow">and</span> <span class="n">package</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">standard_lib</span><span class="p">:</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos">62</span></a>                <span class="k">if</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span> <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]:</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos">63</span></a>                    <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">))</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos">64</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos">65</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos">66</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="n">importlib</span><span class="o">.</span><span class="n">metadata</span><span class="o">.</span><span class="n">version</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos">67</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos">68</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos">69</span></a>                    <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos">70</span></a>                        <span class="s2">&quot;files&quot;</span><span class="p">:</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)],</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos">71</span></a>                        <span class="s2">&quot;version&quot;</span><span class="p">:</span> <span class="n">package_version</span><span class="p">,</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos">72</span></a>                    <span class="p">}</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos">73</span></a>    <span class="k">return</span> <span class="n">packages</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">from</span> <span class="nn">pathlib</span> <span class="kn">import</span> <span class="n">Path</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
+</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="kn">from</span> <span class="nn">packagelister</span> <span class="kn">import</span> <span class="n">scan</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>    <span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>        <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>            <span class="s2">&quot;project_path&quot;</span><span class="p">,</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>            <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The project directory path to scan. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>        <span class="p">)</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>            <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>            <span class="s2">&quot;--show_files&quot;</span><span class="p">,</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Show which files imported each of the packages. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>        <span class="p">)</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>
+</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>            <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>            <span class="s2">&quot;--generate_requirements&quot;</span><span class="p">,</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate a requirements.txt file in --project_path. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>        <span class="p">)</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>            <span class="s2">&quot;-v&quot;</span><span class="p">,</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>            <span class="s2">&quot;--versions&quot;</span><span class="p">,</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>            <span class="n">choices</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;==&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;~=&quot;</span><span class="p">],</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When generating a requirements.txt file,</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a><span class="s2">            include the versions of the packages using this</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a><span class="s2">            relation.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>        <span class="p">)</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>        <span class="p">)</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>
+</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a>
+</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos">55</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos">56</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos">57</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos">58</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos">59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos">60</span></a>        <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos">61</span></a>
+</span><span id="L-62"><a href="#L-62"><span class="linenos">62</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos">63</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos">64</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos">65</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos">66</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos">67</span></a>            <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos">68</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos">69</span></a>                <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos">70</span></a>                <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos">71</span></a>                <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos">72</span></a>                <span class="k">else</span> <span class="n">package</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos">73</span></a>                <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos">74</span></a>            <span class="p">)</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos">75</span></a>        <span class="p">)</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos">76</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos">77</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos">78</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos">79</span></a>    <span class="p">}</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos">80</span></a>
+</span><span id="L-81"><a href="#L-81"><span class="linenos">81</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos">82</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos">83</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos">84</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos">85</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos">86</span></a>        <span class="p">]</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos">87</span></a>
+</span><span id="L-88"><a href="#L-88"><span class="linenos">88</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos">89</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos">90</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos">91</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos">92</span></a>    <span class="p">)</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos">93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos">94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos">95</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos">96</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
-                <section id="scan">
-                            <input id="scan-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="main">
+                            <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">scan</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">project_dir</span><span class="p">:</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">dict</span>:</span></span>
+        <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
-                <label class="view-source-button" for="scan-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#scan"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="scan-10"><a href="#scan-10"><span class="linenos">10</span></a><span class="k">def</span> <span class="nf">scan</span><span class="p">(</span><span class="n">project_dir</span><span class="p">:</span> <span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="scan-11"><a href="#scan-11"><span class="linenos">11</span></a>    <span class="sd">&quot;&quot;&quot;Recursively scans a directory for python files to determine</span>
-</span><span id="scan-12"><a href="#scan-12"><span class="linenos">12</span></a><span class="sd">    what packages are in use, as well as the version number</span>
-</span><span id="scan-13"><a href="#scan-13"><span class="linenos">13</span></a><span class="sd">    if applicable.</span>
-</span><span id="scan-14"><a href="#scan-14"><span class="linenos">14</span></a>
-</span><span id="scan-15"><a href="#scan-15"><span class="linenos">15</span></a><span class="sd">    Returns a dictionary where the keys are package</span>
-</span><span id="scan-16"><a href="#scan-16"><span class="linenos">16</span></a><span class="sd">    names and the values are the version number of the package if there is one</span>
-</span><span id="scan-17"><a href="#scan-17"><span class="linenos">17</span></a><span class="sd">    (None if there isn&#39;t) and a list of the files that import the package.</span>
-</span><span id="scan-18"><a href="#scan-18"><span class="linenos">18</span></a>
-</span><span id="scan-19"><a href="#scan-19"><span class="linenos">19</span></a><span class="sd">    :param project_dir: Can be an absolute or relative path</span>
-</span><span id="scan-20"><a href="#scan-20"><span class="linenos">20</span></a><span class="sd">    to a directory or a single file (.py).</span>
-</span><span id="scan-21"><a href="#scan-21"><span class="linenos">21</span></a><span class="sd">    If it is relative, it will be assumed to be relative to</span>
-</span><span id="scan-22"><a href="#scan-22"><span class="linenos">22</span></a><span class="sd">    the current working directory.</span>
-</span><span id="scan-23"><a href="#scan-23"><span class="linenos">23</span></a><span class="sd">    If an argument isn&#39;t given, the current working directory</span>
-</span><span id="scan-24"><a href="#scan-24"><span class="linenos">24</span></a><span class="sd">    will be scanned.</span>
-</span><span id="scan-25"><a href="#scan-25"><span class="linenos">25</span></a><span class="sd">    If the path doesn&#39;t exist, an empty dictionary is returned.&quot;&quot;&quot;</span>
-</span><span id="scan-26"><a href="#scan-26"><span class="linenos">26</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="p">:</span>
-</span><span id="scan-27"><a href="#scan-27"><span class="linenos">27</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="scan-28"><a href="#scan-28"><span class="linenos">28</span></a>    <span class="k">elif</span> <span class="nb">type</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="scan-29"><a href="#scan-29"><span class="linenos">29</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span>
-</span><span id="scan-30"><a href="#scan-30"><span class="linenos">30</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
-</span><span id="scan-31"><a href="#scan-31"><span class="linenos">31</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
-</span><span id="scan-32"><a href="#scan-32"><span class="linenos">32</span></a>
-</span><span id="scan-33"><a href="#scan-33"><span class="linenos">33</span></a>    <span class="c1"># Return empty dict if project_dir doesn&#39;t exist</span>
-</span><span id="scan-34"><a href="#scan-34"><span class="linenos">34</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="scan-35"><a href="#scan-35"><span class="linenos">35</span></a>        <span class="k">return</span> <span class="p">{}</span>
-</span><span id="scan-36"><a href="#scan-36"><span class="linenos">36</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
-</span><span id="scan-37"><a href="#scan-37"><span class="linenos">37</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="scan-38"><a href="#scan-38"><span class="linenos">38</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
-</span><span id="scan-39"><a href="#scan-39"><span class="linenos">39</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="scan-40"><a href="#scan-40"><span class="linenos">40</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">crawl</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">suffix</span> <span class="o">==</span> <span class="s2">&quot;.py&quot;</span><span class="p">]</span>
-</span><span id="scan-41"><a href="#scan-41"><span class="linenos">41</span></a>
-</span><span id="scan-42"><a href="#scan-42"><span class="linenos">42</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
-</span><span id="scan-43"><a href="#scan-43"><span class="linenos">43</span></a>    <span class="c1"># If scanning one file, the progress bar will show 0% complete if bar.counter == 0</span>
-</span><span id="scan-44"><a href="#scan-44"><span class="linenos">44</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="scan-45"><a href="#scan-45"><span class="linenos">45</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="scan-46"><a href="#scan-46"><span class="linenos">46</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="scan-47"><a href="#scan-47"><span class="linenos">47</span></a>    <span class="n">standard_lib</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span> <span class="k">else</span> <span class="p">[]</span>
-</span><span id="scan-48"><a href="#scan-48"><span class="linenos">48</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="scan-49"><a href="#scan-49"><span class="linenos">49</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="scan-50"><a href="#scan-50"><span class="linenos">50</span></a>        <span class="n">contents</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="scan-51"><a href="#scan-51"><span class="linenos">51</span></a>            <span class="n">line</span><span class="o">.</span><span class="n">split</span><span class="p">()[</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="scan-52"><a href="#scan-52"><span class="linenos">52</span></a>            <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="s2">&quot;utf-8&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">()</span>
-</span><span id="scan-53"><a href="#scan-53"><span class="linenos">53</span></a>            <span class="k">if</span> <span class="n">line</span><span class="o">.</span><span class="n">startswith</span><span class="p">((</span><span class="s2">&quot;from&quot;</span><span class="p">,</span> <span class="s2">&quot;import&quot;</span><span class="p">))</span>
-</span><span id="scan-54"><a href="#scan-54"><span class="linenos">54</span></a>        <span class="p">]</span>
-</span><span id="scan-55"><a href="#scan-55"><span class="linenos">55</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">contents</span><span class="p">:</span>
-</span><span id="scan-56"><a href="#scan-56"><span class="linenos">56</span></a>            <span class="k">if</span> <span class="n">package</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">):</span>
-</span><span id="scan-57"><a href="#scan-57"><span class="linenos">57</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[</span><span class="mi">1</span><span class="p">:]</span>
-</span><span id="scan-58"><a href="#scan-58"><span class="linenos">58</span></a>            <span class="k">if</span> <span class="s2">&quot;.&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="scan-59"><a href="#scan-59"><span class="linenos">59</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[:</span> <span class="n">package</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
-</span><span id="scan-60"><a href="#scan-60"><span class="linenos">60</span></a>            <span class="k">if</span> <span class="s2">&quot;,&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
-</span><span id="scan-61"><a href="#scan-61"><span class="linenos">61</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[:</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="scan-62"><a href="#scan-62"><span class="linenos">62</span></a>            <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">files</span> <span class="ow">and</span> <span class="n">package</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">standard_lib</span><span class="p">:</span>
-</span><span id="scan-63"><a href="#scan-63"><span class="linenos">63</span></a>                <span class="k">if</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span> <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]:</span>
-</span><span id="scan-64"><a href="#scan-64"><span class="linenos">64</span></a>                    <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">))</span>
-</span><span id="scan-65"><a href="#scan-65"><span class="linenos">65</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="scan-66"><a href="#scan-66"><span class="linenos">66</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="scan-67"><a href="#scan-67"><span class="linenos">67</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="n">importlib</span><span class="o">.</span><span class="n">metadata</span><span class="o">.</span><span class="n">version</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="scan-68"><a href="#scan-68"><span class="linenos">68</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="scan-69"><a href="#scan-69"><span class="linenos">69</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="scan-70"><a href="#scan-70"><span class="linenos">70</span></a>                    <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="scan-71"><a href="#scan-71"><span class="linenos">71</span></a>                        <span class="s2">&quot;files&quot;</span><span class="p">:</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)],</span>
-</span><span id="scan-72"><a href="#scan-72"><span class="linenos">72</span></a>                        <span class="s2">&quot;version&quot;</span><span class="p">:</span> <span class="n">package_version</span><span class="p">,</span>
-</span><span id="scan-73"><a href="#scan-73"><span class="linenos">73</span></a>                    <span class="p">}</span>
-</span><span id="scan-74"><a href="#scan-74"><span class="linenos">74</span></a>    <span class="k">return</span> <span class="n">packages</span>
+    <a class="headerlink" href="#main"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-8"><a href="#main-8"><span class="linenos"> 8</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-9"><a href="#main-9"><span class="linenos"> 9</span></a>    <span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="main-10"><a href="#main-10"><span class="linenos">10</span></a>        <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="main-11"><a href="#main-11"><span class="linenos">11</span></a>
+</span><span id="main-12"><a href="#main-12"><span class="linenos">12</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-13"><a href="#main-13"><span class="linenos">13</span></a>            <span class="s2">&quot;project_path&quot;</span><span class="p">,</span>
+</span><span id="main-14"><a href="#main-14"><span class="linenos">14</span></a>            <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="main-15"><a href="#main-15"><span class="linenos">15</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="main-16"><a href="#main-16"><span class="linenos">16</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="main-17"><a href="#main-17"><span class="linenos">17</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The project directory path to scan. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-18"><a href="#main-18"><span class="linenos">18</span></a>        <span class="p">)</span>
+</span><span id="main-19"><a href="#main-19"><span class="linenos">19</span></a>
+</span><span id="main-20"><a href="#main-20"><span class="linenos">20</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-21"><a href="#main-21"><span class="linenos">21</span></a>            <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="main-22"><a href="#main-22"><span class="linenos">22</span></a>            <span class="s2">&quot;--show_files&quot;</span><span class="p">,</span>
+</span><span id="main-23"><a href="#main-23"><span class="linenos">23</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="main-24"><a href="#main-24"><span class="linenos">24</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Show which files imported each of the packages. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-25"><a href="#main-25"><span class="linenos">25</span></a>        <span class="p">)</span>
+</span><span id="main-26"><a href="#main-26"><span class="linenos">26</span></a>
+</span><span id="main-27"><a href="#main-27"><span class="linenos">27</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-28"><a href="#main-28"><span class="linenos">28</span></a>            <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
+</span><span id="main-29"><a href="#main-29"><span class="linenos">29</span></a>            <span class="s2">&quot;--generate_requirements&quot;</span><span class="p">,</span>
+</span><span id="main-30"><a href="#main-30"><span class="linenos">30</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="main-31"><a href="#main-31"><span class="linenos">31</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate a requirements.txt file in --project_path. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-32"><a href="#main-32"><span class="linenos">32</span></a>        <span class="p">)</span>
+</span><span id="main-33"><a href="#main-33"><span class="linenos">33</span></a>
+</span><span id="main-34"><a href="#main-34"><span class="linenos">34</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-35"><a href="#main-35"><span class="linenos">35</span></a>            <span class="s2">&quot;-v&quot;</span><span class="p">,</span>
+</span><span id="main-36"><a href="#main-36"><span class="linenos">36</span></a>            <span class="s2">&quot;--versions&quot;</span><span class="p">,</span>
+</span><span id="main-37"><a href="#main-37"><span class="linenos">37</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="main-38"><a href="#main-38"><span class="linenos">38</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="main-39"><a href="#main-39"><span class="linenos">39</span></a>            <span class="n">choices</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;==&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;~=&quot;</span><span class="p">],</span>
+</span><span id="main-40"><a href="#main-40"><span class="linenos">40</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When generating a requirements.txt file,</span>
+</span><span id="main-41"><a href="#main-41"><span class="linenos">41</span></a><span class="s2">            include the versions of the packages using this</span>
+</span><span id="main-42"><a href="#main-42"><span class="linenos">42</span></a><span class="s2">            relation.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-43"><a href="#main-43"><span class="linenos">43</span></a>        <span class="p">)</span>
+</span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a>
+</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
+</span><span id="main-48"><a href="#main-48"><span class="linenos">48</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="main-49"><a href="#main-49"><span class="linenos">49</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-50"><a href="#main-50"><span class="linenos">50</span></a>        <span class="p">)</span>
+</span><span id="main-51"><a href="#main-51"><span class="linenos">51</span></a>
+</span><span id="main-52"><a href="#main-52"><span class="linenos">52</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="main-53"><a href="#main-53"><span class="linenos">53</span></a>
+</span><span id="main-54"><a href="#main-54"><span class="linenos">54</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
+</span><span id="main-55"><a href="#main-55"><span class="linenos">55</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="main-56"><a href="#main-56"><span class="linenos">56</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="main-57"><a href="#main-57"><span class="linenos">57</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
+</span><span id="main-58"><a href="#main-58"><span class="linenos">58</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
+</span><span id="main-59"><a href="#main-59"><span class="linenos">59</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
+</span><span id="main-60"><a href="#main-60"><span class="linenos">60</span></a>
+</span><span id="main-61"><a href="#main-61"><span class="linenos">61</span></a>        <span class="k">return</span> <span class="n">args</span>
+</span><span id="main-62"><a href="#main-62"><span class="linenos">62</span></a>
+</span><span id="main-63"><a href="#main-63"><span class="linenos">63</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-64"><a href="#main-64"><span class="linenos">64</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
+</span><span id="main-65"><a href="#main-65"><span class="linenos">65</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
+</span><span id="main-66"><a href="#main-66"><span class="linenos">66</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
+</span><span id="main-67"><a href="#main-67"><span class="linenos">67</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="main-68"><a href="#main-68"><span class="linenos">68</span></a>            <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="main-69"><a href="#main-69"><span class="linenos">69</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-70"><a href="#main-70"><span class="linenos">70</span></a>                <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
+</span><span id="main-71"><a href="#main-71"><span class="linenos">71</span></a>                <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-72"><a href="#main-72"><span class="linenos">72</span></a>                <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="main-73"><a href="#main-73"><span class="linenos">73</span></a>                <span class="k">else</span> <span class="n">package</span>
+</span><span id="main-74"><a href="#main-74"><span class="linenos">74</span></a>                <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="main-75"><a href="#main-75"><span class="linenos">75</span></a>            <span class="p">)</span>
+</span><span id="main-76"><a href="#main-76"><span class="linenos">76</span></a>        <span class="p">)</span>
+</span><span id="main-77"><a href="#main-77"><span class="linenos">77</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="main-78"><a href="#main-78"><span class="linenos">78</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="main-79"><a href="#main-79"><span class="linenos">79</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="main-80"><a href="#main-80"><span class="linenos">80</span></a>    <span class="p">}</span>
+</span><span id="main-81"><a href="#main-81"><span class="linenos">81</span></a>
+</span><span id="main-82"><a href="#main-82"><span class="linenos">82</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
+</span><span id="main-83"><a href="#main-83"><span class="linenos">83</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="main-84"><a href="#main-84"><span class="linenos">84</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="main-85"><a href="#main-85"><span class="linenos">85</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-86"><a href="#main-86"><span class="linenos">86</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="main-87"><a href="#main-87"><span class="linenos">87</span></a>        <span class="p">]</span>
+</span><span id="main-88"><a href="#main-88"><span class="linenos">88</span></a>
+</span><span id="main-89"><a href="#main-89"><span class="linenos">89</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="main-90"><a href="#main-90"><span class="linenos">90</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="main-91"><a href="#main-91"><span class="linenos">91</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
+</span><span id="main-92"><a href="#main-92"><span class="linenos">92</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="main-93"><a href="#main-93"><span class="linenos">93</span></a>    <span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Recursively scans a directory for python files to determine
-what packages are in use, as well as the version number
-if applicable.</p>
-
-<p>Returns a dictionary where the keys are package
-names and the values are the version number of the package if there is one
-(None if there isn't) and a list of the files that import the package.</p>
-
-<h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><strong>project_dir</strong>:  Can be an absolute or relative path
-to a directory or a single file (.py).
-If it is relative, it will be assumed to be relative to
-the current working directory.
-If an argument isn't given, the current working directory
-will be scanned.
-If the path doesn't exist, an empty dictionary is returned.</li>
-</ul>
-</div>
-
+    
 
                 </section>
     </main>
 <script>
     function escapeHTML(html) {
         return document.createElement('div').appendChild(document.createTextNode(html)).parentNode.innerHTML;
     }
```

#### html2text {}

```diff
@@ -1,176 +1,199 @@
 
 
   ⁰
 ____ packagelister [Unknown INPUT type]
 ***** API Documentation *****
-    * scan
+    * main
 built_with_pdoc[pdoc_logo]
 
-****** packagelister.packagelister ******
+****** packagelister.packagelister_cli ******
 ⁰ View Source
-_1import importlib.metadata
-_2import sys
-_3from pathlib import Path
-_4
-_5from pathcrawler import crawl
-_6from printbuddies import ProgBar
-_7
-_8
-_9def scan(project_dir: Path | str = None, include_builtins: bool = False) -
-> dict:
-10    """Recursively scans a directory for python files to determine
-11    what packages are in use, as well as the version number
-12    if applicable.
-13
-14    Returns a dictionary where the keys are package
-15    names and the values are the version number of the package if there is
-one
-16    (None if there isn't) and a list of the files that import the package.
-17
-18    :param project_dir: Can be an absolute or relative path
-19    to a directory or a single file (.py).
-20    If it is relative, it will be assumed to be relative to
-21    the current working directory.
-22    If an argument isn't given, the current working directory
-23    will be scanned.
-24    If the path doesn't exist, an empty dictionary is returned."""
-25    if not project_dir:
-26        project_dir = Path.cwd()
-27    elif type(project_dir) is str:
-28        project_dir = Path(project_dir)
-29    if not project_dir.is_absolute():
-30        project_dir = project_dir.absolute()
-31
-32    # Return empty dict if project_dir doesn't exist
-33    if not project_dir.exists():
-34        return {}
-35    # You can scan a non python file one at a time if you reeeally want to.
-36    if project_dir.is_file():
-37        files = [project_dir]
-38    else:
-39        files = [file for file in crawl(project_dir) if file.suffix == ".py"]
-40
-41    bar = ProgBar(len(files), width_ratio=0.33)
-42    # If scanning one file, the progress bar will show 0% complete if
-bar.counter == 0
-43    if len(files) == 1:
-44        bar.counter = 1
-45    packages = {}
-46    standard_lib = list(sys.stdlib_module_names) if not include_builtins else
-[]
-47    for file in files:
-48        bar.display(suffix=f"Scanning {file.name}")
-49        contents = [
-50            line.split()[1]
-51            for line in file.read_text(encoding="utf-8").splitlines()
-52            if line.startswith(("from", "import"))
-53        ]
-54        for package in contents:
-55            if package.startswith("."):
-56                package = package[1:]
-57            if "." in package:
-58                package = package[: package.find(".")]
-59            if "," in package:
-60                package = package[:-1]
-61            if file.with_stem(package) not in files and package not in
-standard_lib:
-62                if package in packages and str(file) not in packages[package]
-["files"]:
-63                    packages[package]["files"].append(str(file))
-64                else:
-65                    try:
-66                        package_version = importlib.metadata.version(package)
-67                    except Exception as e:
-68                        package_version = None
-69                    packages[package] = {
-70                        "files": [str(file)],
-71                        "version": package_version,
-72                    }
-73    return packages
-  ⁰
-def scan(
-project_dir: pathlib.Path | str = None,
-include_builtins: bool = False) -> dict: View Source
-10def scan(project_dir: Path | str = None, include_builtins: bool = False) -
-> dict:
-11    """Recursively scans a directory for python files to determine
-12    what packages are in use, as well as the version number
-13    if applicable.
-14
-15    Returns a dictionary where the keys are package
-16    names and the values are the version number of the package if there is
-one
-17    (None if there isn't) and a list of the files that import the package.
+_1import argparse
+_2from pathlib import Path
+_3
+_4from packagelister import scan
+_5
+_6
+_7def main():
+_8    def get_args() -> argparse.Namespace:
+_9        parser = argparse.ArgumentParser()
+10
+11        parser.add_argument(
+12            "project_path",
+13            nargs="?",
+14            type=str,
+15            default=None,
+16            help=""" The project directory path to scan. """,
+17        )
 18
-19    :param project_dir: Can be an absolute or relative path
-20    to a directory or a single file (.py).
-21    If it is relative, it will be assumed to be relative to
-22    the current working directory.
-23    If an argument isn't given, the current working directory
-24    will be scanned.
-25    If the path doesn't exist, an empty dictionary is returned."""
-26    if not project_dir:
-27        project_dir = Path.cwd()
-28    elif type(project_dir) is str:
-29        project_dir = Path(project_dir)
-30    if not project_dir.is_absolute():
-31        project_dir = project_dir.absolute()
+19        parser.add_argument(
+20            "-s",
+21            "--show_files",
+22            action="store_true",
+23            help=""" Show which files imported each of the packages. """,
+24        )
+25
+26        parser.add_argument(
+27            "-g",
+28            "--generate_requirements",
+29            action="store_true",
+30            help=""" Generate a requirements.txt file in --project_path. """,
+31        )
 32
-33    # Return empty dict if project_dir doesn't exist
-34    if not project_dir.exists():
-35        return {}
-36    # You can scan a non python file one at a time if you reeeally want to.
-37    if project_dir.is_file():
-38        files = [project_dir]
-39    else:
-40        files = [file for file in crawl(project_dir) if file.suffix == ".py"]
-41
-42    bar = ProgBar(len(files), width_ratio=0.33)
-43    # If scanning one file, the progress bar will show 0% complete if
-bar.counter == 0
-44    if len(files) == 1:
-45        bar.counter = 1
-46    packages = {}
-47    standard_lib = list(sys.stdlib_module_names) if not include_builtins else
-[]
-48    for file in files:
-49        bar.display(suffix=f"Scanning {file.name}")
-50        contents = [
-51            line.split()[1]
-52            for line in file.read_text(encoding="utf-8").splitlines()
-53            if line.startswith(("from", "import"))
-54        ]
-55        for package in contents:
-56            if package.startswith("."):
-57                package = package[1:]
-58            if "." in package:
-59                package = package[: package.find(".")]
-60            if "," in package:
-61                package = package[:-1]
-62            if file.with_stem(package) not in files and package not in
-standard_lib:
-63                if package in packages and str(file) not in packages[package]
-["files"]:
-64                    packages[package]["files"].append(str(file))
-65                else:
-66                    try:
-67                        package_version = importlib.metadata.version(package)
-68                    except Exception as e:
-69                        package_version = None
-70                    packages[package] = {
-71                        "files": [str(file)],
-72                        "version": package_version,
-73                    }
-74    return packages
-Recursively scans a directory for python files to determine what packages are
-in use, as well as the version number if applicable.
-Returns a dictionary where the keys are package names and the values are the
-version number of the package if there is one (None if there isn't) and a list
-of the files that import the package.
-* Parameters *
-    * project_dir: Can be an absolute or relative path to a directory or a
-      single file (.py). If it is relative, it will be assumed to be relative
-      to the current working directory. If an argument isn't given, the current
-      working directory will be scanned. If the path doesn't exist, an empty
-      dictionary is returned.
+33        parser.add_argument(
+34            "-v",
+35            "--versions",
+36            type=str,
+37            default=None,
+38            choices=["==", "<", "<=", ">", ">=", "~="],
+39            help=""" When generating a requirements.txt file,
+40            include the versions of the packages using this
+41            relation.""",
+42        )
+43
+44        parser.add_argument(
+45            "-i",
+46            "--include_builtins",
+47            action="store_true",
+48            help=""" Include built in standard library modules. """,
+49        )
+50
+51        args = parser.parse_args()
+52
+53        if not args.project_path:
+54            args.project_path = Path.cwd()
+55        else:
+56            args.project_path = Path(args.project_path)
+57        if not args.project_path.is_absolute():
+58            args.project_path = args.project_path.absolute()
+59
+60        return args
+61
+62    args = get_args()
+63    packages = scan(args.project_path, args.include_builtins)
+64    if args.generate_requirements:
+65        req_path = args.project_path / "requirements.txt"
+66        req_path.write_text(
+67            "\n".join(
+68                f"{package}{args.versions}{packages[package]['version']}"
+69                if args.versions
+70                else f"{package}"
+71                if packages[package]["version"]
+72                else package
+73                for package in sorted(packages)
+74            )
+75        )
+76    packages = {
+77        f"{package}=={packages[package]['version']}": packages[package]
+["files"]
+78        for package in sorted(packages)
+79    }
+80
+81    if args.show_files:
+82        longest_key = max(len(package) for package in packages)
+83        packages = [
+84            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str(Path
+(file).relative_to(args.project_path)) for file in packages[package])}"
+85            for package in packages
+86        ]
+87
+88    print(f"Packages used in {args.project_path.stem}:")
+89    print(
+90        *packages,
+91        sep="\n",
+92    )
+93
+94
+95if __name__ == "__main__":
+96    main()
+  ⁰
+def main(): View Source
+_8def main():
+_9    def get_args() -> argparse.Namespace:
+10        parser = argparse.ArgumentParser()
+11
+12        parser.add_argument(
+13            "project_path",
+14            nargs="?",
+15            type=str,
+16            default=None,
+17            help=""" The project directory path to scan. """,
+18        )
+19
+20        parser.add_argument(
+21            "-s",
+22            "--show_files",
+23            action="store_true",
+24            help=""" Show which files imported each of the packages. """,
+25        )
+26
+27        parser.add_argument(
+28            "-g",
+29            "--generate_requirements",
+30            action="store_true",
+31            help=""" Generate a requirements.txt file in --project_path. """,
+32        )
+33
+34        parser.add_argument(
+35            "-v",
+36            "--versions",
+37            type=str,
+38            default=None,
+39            choices=["==", "<", "<=", ">", ">=", "~="],
+40            help=""" When generating a requirements.txt file,
+41            include the versions of the packages using this
+42            relation.""",
+43        )
+44
+45        parser.add_argument(
+46            "-i",
+47            "--include_builtins",
+48            action="store_true",
+49            help=""" Include built in standard library modules. """,
+50        )
+51
+52        args = parser.parse_args()
+53
+54        if not args.project_path:
+55            args.project_path = Path.cwd()
+56        else:
+57            args.project_path = Path(args.project_path)
+58        if not args.project_path.is_absolute():
+59            args.project_path = args.project_path.absolute()
+60
+61        return args
+62
+63    args = get_args()
+64    packages = scan(args.project_path, args.include_builtins)
+65    if args.generate_requirements:
+66        req_path = args.project_path / "requirements.txt"
+67        req_path.write_text(
+68            "\n".join(
+69                f"{package}{args.versions}{packages[package]['version']}"
+70                if args.versions
+71                else f"{package}"
+72                if packages[package]["version"]
+73                else package
+74                for package in sorted(packages)
+75            )
+76        )
+77    packages = {
+78        f"{package}=={packages[package]['version']}": packages[package]
+["files"]
+79        for package in sorted(packages)
+80    }
+81
+82    if args.show_files:
+83        longest_key = max(len(package) for package in packages)
+84        packages = [
+85            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str(Path
+(file).relative_to(args.project_path)) for file in packages[package])}"
+86            for package in packages
+87        ]
+88
+89    print(f"Packages used in {args.project_path.stem}:")
+90    print(
+91        *packages,
+92        sep="\n",
+93    )
```

### Comparing `packagelister-1.3.1/docs/packagelister/whouses.html` & `packagelister-1.5.0/docs/packagelister/whouses.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.1/src/packagelister/packagelister_cli.py` & `packagelister-1.5.0/src/packagelister/packagelister_cli.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.1/src/packagelister/whouses.py` & `packagelister-1.5.0/src/packagelister/whouses.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.1/LICENSE.txt` & `packagelister-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.1/README.md` & `packagelister-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `packagelister-1.3.1/pyproject.toml` & `packagelister-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,66 +8,65 @@
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b7b 6e61  ..authors = [{na
 00000080: 6d65 3d22 4d61 7474 204d 616e 6573 227d  me="Matt Manes"}
 00000090: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 000000a0: 2022 4465 7465 726d 696e 6520 7768 6174   "Determine what
 000000b0: 2033 7264 2d70 6172 7479 2070 6163 6b61   3rd-party packa
 000000c0: 6765 7320 6120 7072 6f6a 6563 7420 696d  ges a project im
 000000d0: 706f 7274 732e 220d 0a76 6572 7369 6f6e  ports."..version
-000000e0: 203d 2022 312e 332e 3122 0d0a 7265 7175   = "1.3.1"..requ
+000000e0: 203d 2022 312e 352e 3022 0d0a 7265 7175   = "1.5.0"..requ
 000000f0: 6972 6573 2d70 7974 686f 6e20 3d20 223e  ires-python = ">
 00000100: 3d33 2e31 3022 0d0a 6465 7065 6e64 656e  =3.10"..dependen
-00000110: 6369 6573 203d 205b 2270 6174 6863 7261  cies = ["pathcra
-00000120: 776c 6572 222c 2022 7072 696e 7462 7564  wler", "printbud
-00000130: 6469 6573 222c 2022 7079 7465 7374 222c  dies", "pytest",
-00000140: 2022 7061 7468 6965 7222 5d0d 0a72 6561   "pathier"]..rea
-00000150: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
-00000160: 220d 0a6b 6579 776f 7264 7320 3d20 5b0d  "..keywords = [.
-00000170: 0a09 2270 6163 6b61 6765 222c 0d0a 0922  .."package",..."
-00000180: 696d 706f 7274 222c 0d0a 0922 6d6f 6475  import",..."modu
-00000190: 6c65 220d 0a20 2020 205d 0d0a 636c 6173  le"..    ]..clas
-000001a0: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
-000001b0: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
-000001c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001d0: 203a 3a20 3322 2c0d 0a20 2020 2022 4c69   :: 3",..    "Li
-000001e0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001f0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000200: 656e 7365 222c 0d0a 2020 2020 224f 7065  ense",..    "Ope
-00000210: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000220: 204f 5320 496e 6465 7065 6e64 656e 7422   OS Independent"
-00000230: 2c0d 0a20 2020 205d 0d0a 0d0a 5b70 726f  ,..    ]....[pro
-00000240: 6a65 6374 2e75 726c 735d 0d0a 2248 6f6d  ject.urls].."Hom
-00000250: 6570 6167 6522 203d 2022 6874 7470 733a  epage" = "https:
-00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
-00000270: 742d 6d61 6e65 732f 7061 636b 6167 656c  t-manes/packagel
-00000280: 6973 7465 7222 0d0a 2244 6f63 756d 656e  ister".."Documen
-00000290: 7461 7469 6f6e 2220 3d20 2268 7474 7073  tation" = "https
-000002a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
-000002b0: 7474 2d6d 616e 6573 2f70 6163 6b61 6765  tt-manes/package
-000002c0: 6c69 7374 6572 2f74 7265 652f 6d61 696e  lister/tree/main
-000002d0: 2f64 6f63 7322 0d0a 2253 6f75 7263 6520  /docs".."Source 
-000002e0: 636f 6465 2220 3d20 2268 7474 7073 3a2f  code" = "https:/
-000002f0: 2f67 6974 6875 622e 636f 6d2f 6d61 7474  /github.com/matt
-00000300: 2d6d 616e 6573 2f70 6163 6b61 6765 6c69  -manes/packageli
-00000310: 7374 6572 2f74 7265 652f 6d61 696e 2f73  ster/tree/main/s
-00000320: 7263 2f70 6163 6b61 6765 6c69 7374 6572  rc/packagelister
-00000330: 220d 0a0d 0a5b 7072 6f6a 6563 742e 7363  "....[project.sc
-00000340: 7269 7074 735d 0d0a 7061 636b 6167 656c  ripts]..packagel
-00000350: 6973 7465 7220 3d20 2270 6163 6b61 6765  ister = "package
-00000360: 6c69 7374 6572 2e70 6163 6b61 6765 6c69  lister.packageli
-00000370: 7374 6572 5f63 6c69 3a6d 6169 6e22 0d0a  ster_cli:main"..
-00000380: 7768 6f75 7365 7320 3d20 2270 6163 6b61  whouses = "packa
-00000390: 6765 6c69 7374 6572 2e77 686f 7573 6573  gelister.whouses
-000003a0: 3a6d 6169 6e22 0d0a 0d0a 5b74 6f6f 6c2e  :main"....[tool.
-000003b0: 7079 7465 7374 2e69 6e69 5f6f 7074 696f  pytest.ini_optio
-000003c0: 6e73 5d0d 0a61 6464 6f70 7473 203d 205b  ns]..addopts = [
-000003d0: 0d0a 2020 2020 222d 2d69 6d70 6f72 742d  ..    "--import-
-000003e0: 6d6f 6465 3d69 6d70 6f72 746c 6962 222c  mode=importlib",
-000003f0: 0d0a 2020 2020 5d0d 0a70 7974 686f 6e70  ..    ]..pythonp
-00000400: 6174 6820 3d20 2273 7263 220d 0a0d 0a5b  ath = "src"....[
-00000410: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
-00000420: 2e74 6172 6765 7473 2e73 6469 7374 5d0d  .targets.sdist].
-00000430: 0a65 7863 6c75 6465 203d 205b 0d0a 2020  .exclude = [..  
-00000440: 2020 222e 636f 7665 7261 6765 222c 0d0a    ".coverage",..
-00000450: 2020 2020 222e 7079 7465 7374 5f63 6163      ".pytest_cac
-00000460: 6865 222c 0d0a 2020 2020 222e 7673 636f  he",..    ".vsco
-00000470: 6465 222c 0d0a 2020 2020 2274 6573 7473  de",..    "tests
-00000480: 220d 0a20 2020 205d                      "..    ]
+00000110: 6369 6573 203d 205b 2270 7269 6e74 6275  cies = ["printbu
+00000120: 6464 6965 7322 2c20 2270 7974 6573 7422  ddies", "pytest"
+00000130: 2c20 2270 6174 6869 6572 225d 0d0a 7265  , "pathier"]..re
+00000140: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
+00000150: 6422 0d0a 6b65 7977 6f72 6473 203d 205b  d"..keywords = [
+00000160: 0d0a 0922 7061 636b 6167 6522 2c0d 0a09  ..."package",...
+00000170: 2269 6d70 6f72 7422 2c0d 0a09 226d 6f64  "import",..."mod
+00000180: 756c 6522 0d0a 2020 2020 5d0d 0a63 6c61  ule"..    ]..cla
+00000190: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
+000001a0: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
+000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001c0: 6e20 3a3a 2033 222c 0d0a 2020 2020 224c  n :: 3",..    "L
+000001d0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001e0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000001f0: 6365 6e73 6522 2c0d 0a20 2020 2022 4f70  cense",..    "Op
+00000200: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000210: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000220: 222c 0d0a 2020 2020 5d0d 0a0d 0a5b 7072  ",..    ]....[pr
+00000230: 6f6a 6563 742e 7572 6c73 5d0d 0a22 486f  oject.urls].."Ho
+00000240: 6d65 7061 6765 2220 3d20 2268 7474 7073  mepage" = "https
+00000250: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+00000260: 7474 2d6d 616e 6573 2f70 6163 6b61 6765  tt-manes/package
+00000270: 6c69 7374 6572 220d 0a22 446f 6375 6d65  lister".."Docume
+00000280: 6e74 6174 696f 6e22 203d 2022 6874 7470  ntation" = "http
+00000290: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+000002a0: 6174 742d 6d61 6e65 732f 7061 636b 6167  att-manes/packag
+000002b0: 656c 6973 7465 722f 7472 6565 2f6d 6169  elister/tree/mai
+000002c0: 6e2f 646f 6373 220d 0a22 536f 7572 6365  n/docs".."Source
+000002d0: 2063 6f64 6522 203d 2022 6874 7470 733a   code" = "https:
+000002e0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
+000002f0: 742d 6d61 6e65 732f 7061 636b 6167 656c  t-manes/packagel
+00000300: 6973 7465 722f 7472 6565 2f6d 6169 6e2f  ister/tree/main/
+00000310: 7372 632f 7061 636b 6167 656c 6973 7465  src/packageliste
+00000320: 7222 0d0a 0d0a 5b70 726f 6a65 6374 2e73  r"....[project.s
+00000330: 6372 6970 7473 5d0d 0a70 6163 6b61 6765  cripts]..package
+00000340: 6c69 7374 6572 203d 2022 7061 636b 6167  lister = "packag
+00000350: 656c 6973 7465 722e 7061 636b 6167 656c  elister.packagel
+00000360: 6973 7465 725f 636c 693a 6d61 696e 220d  ister_cli:main".
+00000370: 0a77 686f 7573 6573 203d 2022 7061 636b  .whouses = "pack
+00000380: 6167 656c 6973 7465 722e 7768 6f75 7365  agelister.whouse
+00000390: 733a 6d61 696e 220d 0a0d 0a5b 746f 6f6c  s:main"....[tool
+000003a0: 2e70 7974 6573 742e 696e 695f 6f70 7469  .pytest.ini_opti
+000003b0: 6f6e 735d 0d0a 6164 646f 7074 7320 3d20  ons]..addopts = 
+000003c0: 5b0d 0a20 2020 2022 2d2d 696d 706f 7274  [..    "--import
+000003d0: 2d6d 6f64 653d 696d 706f 7274 6c69 6222  -mode=importlib"
+000003e0: 2c0d 0a20 2020 205d 0d0a 7079 7468 6f6e  ,..    ]..python
+000003f0: 7061 7468 203d 2022 7372 6322 0d0a 0d0a  path = "src"....
+00000400: 5b74 6f6f 6c2e 6861 7463 682e 6275 696c  [tool.hatch.buil
+00000410: 642e 7461 7267 6574 732e 7364 6973 745d  d.targets.sdist]
+00000420: 0d0a 6578 636c 7564 6520 3d20 5b0d 0a20  ..exclude = [.. 
+00000430: 2020 2022 2e63 6f76 6572 6167 6522 2c0d     ".coverage",.
+00000440: 0a20 2020 2022 2e70 7974 6573 745f 6361  .    ".pytest_ca
+00000450: 6368 6522 2c0d 0a20 2020 2022 2e76 7363  che",..    ".vsc
+00000460: 6f64 6522 2c0d 0a20 2020 2022 7465 7374  ode",..    "test
+00000470: 7322 0d0a 2020 2020 5d                   s"..    ]
```

### Comparing `packagelister-1.3.1/PKG-INFO` & `packagelister-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: packagelister
-Version: 1.3.1
+Version: 1.5.0
 Summary: Determine what 3rd-party packages a project imports.
 Project-URL: Homepage, https://github.com/matt-manes/packagelister
 Project-URL: Documentation, https://github.com/matt-manes/packagelister/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/packagelister/tree/main/src/packagelister
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: import,module,package
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: pathcrawler
 Requires-Dist: pathier
 Requires-Dist: printbuddies
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # packagelister
 Determine what packages and versions a project imports. <br>
```

