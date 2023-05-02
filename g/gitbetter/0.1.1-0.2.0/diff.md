# Comparing `tmp/gitbetter-0.1.1.tar.gz` & `tmp/gitbetter-0.2.0.tar.gz`

## Comparing `gitbetter-0.1.1.tar` & `gitbetter-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 gitbetter-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/index.html
--rw-r--r--   0        0        0    55399 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/search.js
--rw-r--r--   0        0        0   130318 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/gitbetter/git.html
--rw-r--r--   0        0        0   227735 2020-02-02 00:00:00.000000 gitbetter-0.1.1/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.1.1/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 gitbetter-0.1.1/src/gitbetter/git.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 gitbetter-0.1.1/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.1.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 gitbetter-0.1.1/README.md
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 gitbetter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 gitbetter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gitbetter-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.2.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.2.0/docs/index.html
+-rw-r--r--   0        0        0    56993 2020-02-02 00:00:00.000000 gitbetter-0.2.0/docs/search.js
+-rw-r--r--   0        0        0   130318 2020-02-02 00:00:00.000000 gitbetter-0.2.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   250506 2020-02-02 00:00:00.000000 gitbetter-0.2.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.2.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 gitbetter-0.2.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10327 2020-02-02 00:00:00.000000 gitbetter-0.2.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 gitbetter-0.2.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 gitbetter-0.2.0/PKG-INFO
```

### Comparing `gitbetter-0.1.1/docs/gitbetter.html` & `gitbetter-0.2.0/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.1/docs/search.js` & `gitbetter-0.2.0/docs/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -957,28 +957,44 @@
         "fullname": "gitbetter.gitbetter.GitBetter",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter",
         "kind": "class",
         "doc": "<p>GitBetter Shell.</p>\n",
         "bases": "argshell.argshell.ArgShell"
     }, {
-        "fullname": "gitbetter.gitbetter.GitBetter.do_cd",
+        "fullname": "gitbetter.gitbetter.GitBetter.default",
         "modulename": "gitbetter.gitbetter",
-        "qualname": "GitBetter.do_cd",
+        "qualname": "GitBetter.default",
         "kind": "function",
-        "doc": "<p>Change current working directory to <code>path</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">path</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "doc": "<p>Called on an input line when the command prefix is not recognized.</p>\n\n<p>If this method is not overridden, it prints an error message and\nreturns.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">line</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "gitbetter.gitbetter.GitBetter.do_help",
+        "modulename": "gitbetter.gitbetter",
+        "qualname": "GitBetter.do_help",
+        "kind": "function",
+        "doc": "<p>List available commands with \"help\" or detailed help with \"help cmd\".</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">arg</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.gitbetter.GitBetter.do_cwd",
+        "fullname": "gitbetter.gitbetter.GitBetter.do_toggle_unrecognized_command_behavior",
         "modulename": "gitbetter.gitbetter",
-        "qualname": "GitBetter.do_cwd",
+        "qualname": "GitBetter.do_toggle_unrecognized_command_behavior",
         "kind": "function",
-        "doc": "<p>Print the current working directory.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">_</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "doc": "<p>Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.\nWhen on (the default), <code>GitBetter</code> will treat unrecognized commands as if you added the <code>cmd</code> command in front of the input, i.e. <code>os.system(your_input)</code>.\nWhen off, an <code>unknown syntax</code> message will be printed and no commands will be executed.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">arg</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "gitbetter.gitbetter.GitBetter.do_cd",
+        "modulename": "gitbetter.gitbetter",
+        "qualname": "GitBetter.do_cd",
+        "kind": "function",
+        "doc": "<p>Change current working directory to <code>path</code>.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">path</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_cmd",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_cmd",
         "kind": "function",
         "doc": "<p>Execute arbitrary command in the terminal so you don't have to quit gitbetter to run other programs/commands.</p>\n",
```

### Comparing `gitbetter-0.1.1/docs/gitbetter/git.html` & `gitbetter-0.2.0/docs/gitbetter/git.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.1/docs/gitbetter/gitbetter.html` & `gitbetter-0.2.0/docs/gitbetter/gitbetter.html`

 * *Files 5% similar despite different names*

```diff
@@ -48,18 +48,24 @@
             <li>
                     <a class="function" href="#files_postparser">files_postparser</a>
             </li>
             <li>
                     <a class="class" href="#GitBetter">GitBetter</a>
                             <ul class="memberlist">
                         <li>
-                                <a class="function" href="#GitBetter.do_cd">do_cd</a>
+                                <a class="function" href="#GitBetter.default">default</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#GitBetter.do_help">do_help</a>
                         </li>
                         <li>
-                                <a class="function" href="#GitBetter.do_cwd">do_cwd</a>
+                                <a class="function" href="#GitBetter.do_toggle_unrecognized_command_behavior">do_toggle_unrecognized_command_behavior</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#GitBetter.do_cd">do_cd</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_cmd">do_cmd</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_git">do_git</a>
                         </li>
@@ -263,181 +269,209 @@
 </span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
 </span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
 </span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
 </span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
 </span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;gitbetter&gt;&quot;</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="nf">do_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="sd">&quot;&quot;&quot;Print the current working directory.&quot;&quot;&quot;</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">())</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_cmd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Execute arbitrary command in the terminal so you don&#39;t have to quit gitbetter to run other programs/commands.&quot;&quot;&quot;</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                <span class="p">)</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="nd">@property</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `cmd` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="p">)</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="k">def</span> <span class="nf">do_cmd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="sd">&quot;&quot;&quot;Execute arbitrary command in the terminal so you don&#39;t have to quit gitbetter to run other programs/commands.&quot;&quot;&quot;</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
 </span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
 </span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
 </span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
 </span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="new_remote_parser">
                             <input id="new_remote_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -629,220 +663,312 @@
 
     </div>
     <a class="headerlink" href="#GitBetter"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter-100"><a href="#GitBetter-100"><span class="linenos">100</span></a><span class="k">class</span> <span class="nc">GitBetter</span><span class="p">(</span><span class="n">ArgShell</span><span class="p">):</span>
 </span><span id="GitBetter-101"><a href="#GitBetter-101"><span class="linenos">101</span></a>    <span class="sd">&quot;&quot;&quot;GitBetter Shell.&quot;&quot;&quot;</span>
 </span><span id="GitBetter-102"><a href="#GitBetter-102"><span class="linenos">102</span></a>
 </span><span id="GitBetter-103"><a href="#GitBetter-103"><span class="linenos">103</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting gitbetter...</span><span class="se">\n</span><span class="s2">Enter &#39;help&#39; or &#39;?&#39; for command help.&quot;</span>
-</span><span id="GitBetter-104"><a href="#GitBetter-104"><span class="linenos">104</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;gitbetter&gt;&quot;</span>
-</span><span id="GitBetter-105"><a href="#GitBetter-105"><span class="linenos">105</span></a>
-</span><span id="GitBetter-106"><a href="#GitBetter-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-107"><a href="#GitBetter-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-108"><a href="#GitBetter-108"><span class="linenos">108</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="GitBetter-109"><a href="#GitBetter-109"><span class="linenos">109</span></a>
-</span><span id="GitBetter-110"><a href="#GitBetter-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="nf">do_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-111"><a href="#GitBetter-111"><span class="linenos">111</span></a>        <span class="sd">&quot;&quot;&quot;Print the current working directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-112"><a href="#GitBetter-112"><span class="linenos">112</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">())</span>
-</span><span id="GitBetter-113"><a href="#GitBetter-113"><span class="linenos">113</span></a>
-</span><span id="GitBetter-114"><a href="#GitBetter-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_cmd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-115"><a href="#GitBetter-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Execute arbitrary command in the terminal so you don&#39;t have to quit gitbetter to run other programs/commands.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-116"><a href="#GitBetter-116"><span class="linenos">116</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
-</span><span id="GitBetter-117"><a href="#GitBetter-117"><span class="linenos">117</span></a>
-</span><span id="GitBetter-118"><a href="#GitBetter-118"><span class="linenos">118</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-119"><a href="#GitBetter-119"><span class="linenos">119</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="GitBetter-120"><a href="#GitBetter-120"><span class="linenos">120</span></a>
-</span><span id="GitBetter-121"><a href="#GitBetter-121"><span class="linenos">121</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-122"><a href="#GitBetter-122"><span class="linenos">122</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter-104"><a href="#GitBetter-104"><span class="linenos">104</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="GitBetter-105"><a href="#GitBetter-105"><span class="linenos">105</span></a>    <span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="GitBetter-106"><a href="#GitBetter-106"><span class="linenos">106</span></a>
+</span><span id="GitBetter-107"><a href="#GitBetter-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-108"><a href="#GitBetter-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter-109"><a href="#GitBetter-109"><span class="linenos">109</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter-110"><a href="#GitBetter-110"><span class="linenos">110</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="GitBetter-111"><a href="#GitBetter-111"><span class="linenos">111</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter-112"><a href="#GitBetter-112"><span class="linenos">112</span></a>
+</span><span id="GitBetter-113"><a href="#GitBetter-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-114"><a href="#GitBetter-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-115"><a href="#GitBetter-115"><span class="linenos">115</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter-116"><a href="#GitBetter-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="GitBetter-117"><a href="#GitBetter-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter-118"><a href="#GitBetter-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter-119"><a href="#GitBetter-119"><span class="linenos">119</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="GitBetter-120"><a href="#GitBetter-120"><span class="linenos">120</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="GitBetter-121"><a href="#GitBetter-121"><span class="linenos">121</span></a>                <span class="p">)</span>
+</span><span id="GitBetter-122"><a href="#GitBetter-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span><span id="GitBetter-123"><a href="#GitBetter-123"><span class="linenos">123</span></a>
-</span><span id="GitBetter-124"><a href="#GitBetter-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-125"><a href="#GitBetter-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="GitBetter-124"><a href="#GitBetter-124"><span class="linenos">124</span></a>    <span class="nd">@property</span>
+</span><span id="GitBetter-125"><a href="#GitBetter-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="GitBetter-127"><a href="#GitBetter-127"><span class="linenos">127</span></a>
-</span><span id="GitBetter-128"><a href="#GitBetter-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-129"><a href="#GitBetter-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-130"><a href="#GitBetter-130"><span class="linenos">130</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="GitBetter-131"><a href="#GitBetter-131"><span class="linenos">131</span></a>
-</span><span id="GitBetter-132"><a href="#GitBetter-132"><span class="linenos">132</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter-133"><a href="#GitBetter-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-134"><a href="#GitBetter-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter-135"><a href="#GitBetter-135"><span class="linenos">135</span></a>
-</span><span id="GitBetter-136"><a href="#GitBetter-136"><span class="linenos">136</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-137"><a href="#GitBetter-137"><span class="linenos">137</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="GitBetter-138"><a href="#GitBetter-138"><span class="linenos">138</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="GitBetter-139"><a href="#GitBetter-139"><span class="linenos">139</span></a>
-</span><span id="GitBetter-140"><a href="#GitBetter-140"><span class="linenos">140</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-141"><a href="#GitBetter-141"><span class="linenos">141</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-142"><a href="#GitBetter-142"><span class="linenos">142</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="GitBetter-143"><a href="#GitBetter-143"><span class="linenos">143</span></a>
-</span><span id="GitBetter-144"><a href="#GitBetter-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-145"><a href="#GitBetter-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-146"><a href="#GitBetter-146"><span class="linenos">146</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="GitBetter-147"><a href="#GitBetter-147"><span class="linenos">147</span></a>
-</span><span id="GitBetter-148"><a href="#GitBetter-148"><span class="linenos">148</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-149"><a href="#GitBetter-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-150"><a href="#GitBetter-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter-151"><a href="#GitBetter-151"><span class="linenos">151</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-152"><a href="#GitBetter-152"><span class="linenos">152</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-153"><a href="#GitBetter-153"><span class="linenos">153</span></a>
-</span><span id="GitBetter-154"><a href="#GitBetter-154"><span class="linenos">154</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-155"><a href="#GitBetter-155"><span class="linenos">155</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-156"><a href="#GitBetter-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-157"><a href="#GitBetter-157"><span class="linenos">157</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter-158"><a href="#GitBetter-158"><span class="linenos">158</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-159"><a href="#GitBetter-159"><span class="linenos">159</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter-160"><a href="#GitBetter-160"><span class="linenos">160</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a>
-</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>
-</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-128"><a href="#GitBetter-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-129"><a href="#GitBetter-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="GitBetter-130"><a href="#GitBetter-130"><span class="linenos">130</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `cmd` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="GitBetter-131"><a href="#GitBetter-131"><span class="linenos">131</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-132"><a href="#GitBetter-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="GitBetter-133"><a href="#GitBetter-133"><span class="linenos">133</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="GitBetter-134"><a href="#GitBetter-134"><span class="linenos">134</span></a>        <span class="p">)</span>
+</span><span id="GitBetter-135"><a href="#GitBetter-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter-136"><a href="#GitBetter-136"><span class="linenos">136</span></a>
+</span><span id="GitBetter-137"><a href="#GitBetter-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-138"><a href="#GitBetter-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-139"><a href="#GitBetter-139"><span class="linenos">139</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="GitBetter-140"><a href="#GitBetter-140"><span class="linenos">140</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span><span id="GitBetter-141"><a href="#GitBetter-141"><span class="linenos">141</span></a>
+</span><span id="GitBetter-142"><a href="#GitBetter-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">do_cmd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-143"><a href="#GitBetter-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Execute arbitrary command in the terminal so you don&#39;t have to quit gitbetter to run other programs/commands.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-144"><a href="#GitBetter-144"><span class="linenos">144</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+</span><span id="GitBetter-145"><a href="#GitBetter-145"><span class="linenos">145</span></a>
+</span><span id="GitBetter-146"><a href="#GitBetter-146"><span class="linenos">146</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-147"><a href="#GitBetter-147"><span class="linenos">147</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="GitBetter-148"><a href="#GitBetter-148"><span class="linenos">148</span></a>
+</span><span id="GitBetter-149"><a href="#GitBetter-149"><span class="linenos">149</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-150"><a href="#GitBetter-150"><span class="linenos">150</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter-151"><a href="#GitBetter-151"><span class="linenos">151</span></a>
+</span><span id="GitBetter-152"><a href="#GitBetter-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-153"><a href="#GitBetter-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-154"><a href="#GitBetter-154"><span class="linenos">154</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="GitBetter-155"><a href="#GitBetter-155"><span class="linenos">155</span></a>
+</span><span id="GitBetter-156"><a href="#GitBetter-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-157"><a href="#GitBetter-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-158"><a href="#GitBetter-158"><span class="linenos">158</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="GitBetter-159"><a href="#GitBetter-159"><span class="linenos">159</span></a>
+</span><span id="GitBetter-160"><a href="#GitBetter-160"><span class="linenos">160</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>
+</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>
+</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>
+</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span><span id="GitBetter-175"><a href="#GitBetter-175"><span class="linenos">175</span></a>
-</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a>
-</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>
-</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>
-</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>
-</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>
+</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>
+</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
 </span><span id="GitBetter-194"><a href="#GitBetter-194"><span class="linenos">194</span></a>
-</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>
-</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>
-</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>
-</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>
-</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-211"><a href="#GitBetter-211"><span class="linenos">211</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>
+</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>
+</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter-211"><a href="#GitBetter-211"><span class="linenos">211</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
 </span><span id="GitBetter-212"><a href="#GitBetter-212"><span class="linenos">212</span></a>
-</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-214"><a href="#GitBetter-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-214"><a href="#GitBetter-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span><span id="GitBetter-216"><a href="#GitBetter-216"><span class="linenos">216</span></a>
-</span><span id="GitBetter-217"><a href="#GitBetter-217"><span class="linenos">217</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-220"><a href="#GitBetter-220"><span class="linenos">220</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a>
-</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>
-</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>
-</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>
-</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter-217"><a href="#GitBetter-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a>
+</span><span id="GitBetter-220"><a href="#GitBetter-220"><span class="linenos">220</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a>
+</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>
+</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>
+</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>
+</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>
+</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>
-</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>
-</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>
-</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>
-</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>
-</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>
-</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>
-</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>
+</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>
+</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>
+</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
 </span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>
-</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>
-</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a>
+</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a>
+</span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a>
+</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a>
+</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a>
+</span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a>
+</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a>
+</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a>
+</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a>
+</span><span id="GitBetter-287"><a href="#GitBetter-287"><span class="linenos">287</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter-288"><a href="#GitBetter-288"><span class="linenos">288</span></a>
+</span><span id="GitBetter-289"><a href="#GitBetter-289"><span class="linenos">289</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-290"><a href="#GitBetter-290"><span class="linenos">290</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>GitBetter Shell.</p>
 </div>
 
 
-                            <div id="GitBetter.do_cd" class="classattr">
-                                        <input id="GitBetter.do_cd-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="GitBetter.default" class="classattr">
+                                        <input id="GitBetter.default-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">do_cd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+        <span class="name">default</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">line</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
-                <label class="view-source-button" for="GitBetter.do_cd-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="GitBetter.default-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#GitBetter.do_cd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cd-106"><a href="#GitBetter.do_cd-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_cd-107"><a href="#GitBetter.do_cd-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_cd-108"><a href="#GitBetter.do_cd-108"><span class="linenos">108</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+    <a class="headerlink" href="#GitBetter.default"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.default-107"><a href="#GitBetter.default-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">line</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.default-108"><a href="#GitBetter.default-108"><span class="linenos">108</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter.default-109"><a href="#GitBetter.default-109"><span class="linenos">109</span></a>            <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
+</span><span id="GitBetter.default-110"><a href="#GitBetter.default-110"><span class="linenos">110</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="GitBetter.default-111"><a href="#GitBetter.default-111"><span class="linenos">111</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">default</span><span class="p">(</span><span class="n">line</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Change current working directory to <code>path</code>.</p>
+            <div class="docstring"><p>Called on an input line when the command prefix is not recognized.</p>
+
+<p>If this method is not overridden, it prints an error message and
+returns.</p>
 </div>
 
 
                             </div>
-                            <div id="GitBetter.do_cwd" class="classattr">
-                                        <input id="GitBetter.do_cwd-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="GitBetter.do_help" class="classattr">
+                                        <input id="GitBetter.do_help-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">do_cwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+        <span class="name">do_help</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
-                <label class="view-source-button" for="GitBetter.do_cwd-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="GitBetter.do_help-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#GitBetter.do_cwd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cwd-110"><a href="#GitBetter.do_cwd-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="nf">do_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_cwd-111"><a href="#GitBetter.do_cwd-111"><span class="linenos">111</span></a>        <span class="sd">&quot;&quot;&quot;Print the current working directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_cwd-112"><a href="#GitBetter.do_cwd-112"><span class="linenos">112</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">())</span>
+    <a class="headerlink" href="#GitBetter.do_help"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_help-113"><a href="#GitBetter.do_help-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_help</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_help-114"><a href="#GitBetter.do_help-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;List available commands with &quot;help&quot; or detailed help with &quot;help cmd&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_help-115"><a href="#GitBetter.do_help-115"><span class="linenos">115</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">do_help</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="GitBetter.do_help-116"><a href="#GitBetter.do_help-116"><span class="linenos">116</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">arg</span><span class="p">:</span>
+</span><span id="GitBetter.do_help-117"><a href="#GitBetter.do_help-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span><span id="GitBetter.do_help-118"><a href="#GitBetter.do_help-118"><span class="linenos">118</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span><span class="p">:</span>
+</span><span id="GitBetter.do_help-119"><a href="#GitBetter.do_help-119"><span class="linenos">119</span></a>                <span class="nb">print</span><span class="p">(</span>
+</span><span id="GitBetter.do_help-120"><a href="#GitBetter.do_help-120"><span class="linenos">120</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
+</span><span id="GitBetter.do_help-121"><a href="#GitBetter.do_help-121"><span class="linenos">121</span></a>                <span class="p">)</span>
+</span><span id="GitBetter.do_help-122"><a href="#GitBetter.do_help-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Print the current working directory.</p>
+            <div class="docstring"><p>List available commands with "help" or detailed help with "help cmd".</p>
+</div>
+
+
+                            </div>
+                            <div id="GitBetter.do_toggle_unrecognized_command_behavior" class="classattr">
+                                        <input id="GitBetter.do_toggle_unrecognized_command_behavior-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">do_toggle_unrecognized_command_behavior</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="GitBetter.do_toggle_unrecognized_command_behavior-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#GitBetter.do_toggle_unrecognized_command_behavior"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_toggle_unrecognized_command_behavior-128"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-129"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-130"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-130"><span class="linenos">130</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `cmd` command in front of the input, i.e. `os.system(your_input)`.</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-131"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-131"><span class="linenos">131</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-132"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-133"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-133"><span class="linenos">133</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-134"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-134"><span class="linenos">134</span></a>        <span class="p">)</span>
+</span><span id="GitBetter.do_toggle_unrecognized_command_behavior-135"><a href="#GitBetter.do_toggle_unrecognized_command_behavior-135"><span class="linenos">135</span></a>        <span class="nb">print</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">unrecognized_command_behavior_status</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.
+When on (the default), <code><a href="#GitBetter">GitBetter</a></code> will treat unrecognized commands as if you added the <code>cmd</code> command in front of the input, i.e. <code>os.system(your_input)</code>.
+When off, an <code>unknown syntax</code> message will be printed and no commands will be executed.</p>
+</div>
+
+
+                            </div>
+                            <div id="GitBetter.do_cd" class="classattr">
+                                        <input id="GitBetter.do_cd-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">do_cd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="GitBetter.do_cd-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#GitBetter.do_cd"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cd-137"><a href="#GitBetter.do_cd-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">do_cd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_cd-138"><a href="#GitBetter.do_cd-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Change current working directory to `path`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_cd-139"><a href="#GitBetter.do_cd-139"><span class="linenos">139</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="GitBetter.do_cd-140"><a href="#GitBetter.do_cd-140"><span class="linenos">140</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prompt</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;gitbetter::</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&gt;&quot;</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Change current working directory to <code>path</code>.</p>
 </div>
 
 
                             </div>
                             <div id="GitBetter.do_cmd" class="classattr">
                                         <input id="GitBetter.do_cmd-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -850,17 +976,17 @@
         <span class="def">def</span>
         <span class="name">do_cmd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">command</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_cmd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_cmd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cmd-114"><a href="#GitBetter.do_cmd-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_cmd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_cmd-115"><a href="#GitBetter.do_cmd-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Execute arbitrary command in the terminal so you don&#39;t have to quit gitbetter to run other programs/commands.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_cmd-116"><a href="#GitBetter.do_cmd-116"><span class="linenos">116</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_cmd-142"><a href="#GitBetter.do_cmd-142"><span class="linenos">142</span></a>    <span class="k">def</span> <span class="nf">do_cmd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_cmd-143"><a href="#GitBetter.do_cmd-143"><span class="linenos">143</span></a>        <span class="sd">&quot;&quot;&quot;Execute arbitrary command in the terminal so you don&#39;t have to quit gitbetter to run other programs/commands.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_cmd-144"><a href="#GitBetter.do_cmd-144"><span class="linenos">144</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="n">command</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute arbitrary command in the terminal so you don't have to quit gitbetter to run other programs/commands.</p>
 </div>
 
 
@@ -872,19 +998,19 @@
         <span class="def">def</span>
         <span class="name">do_git</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_git-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_git"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_git-118"><a href="#GitBetter.do_git-118"><span class="linenos">118</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_git-119"><a href="#GitBetter.do_git-119"><span class="linenos">119</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
-</span><span id="GitBetter.do_git-120"><a href="#GitBetter.do_git-120"><span class="linenos">120</span></a>
-</span><span id="GitBetter.do_git-121"><a href="#GitBetter.do_git-121"><span class="linenos">121</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_git-122"><a href="#GitBetter.do_git-122"><span class="linenos">122</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_git-146"><a href="#GitBetter.do_git-146"><span class="linenos">146</span></a>    <span class="k">def</span> <span class="nf">do_git</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_git-147"><a href="#GitBetter.do_git-147"><span class="linenos">147</span></a>        <span class="sd">&quot;&quot;&quot;Directly execute `git {arg}`.</span>
+</span><span id="GitBetter.do_git-148"><a href="#GitBetter.do_git-148"><span class="linenos">148</span></a>
+</span><span id="GitBetter.do_git-149"><a href="#GitBetter.do_git-149"><span class="linenos">149</span></a><span class="sd">        i.e. You can still do everything directly invoking git can do.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_git-150"><a href="#GitBetter.do_git-150"><span class="linenos">150</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Directly execute <code>git {arg}</code>.</p>
 
 <p>i.e. You can still do everything directly invoking git can do.</p>
 </div>
@@ -898,17 +1024,17 @@
         <span class="def">def</span>
         <span class="name">do_new_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-124"><a href="#GitBetter.do_new_repo-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_repo-125"><a href="#GitBetter.do_new_repo-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_repo-126"><a href="#GitBetter.do_new_repo-126"><span class="linenos">126</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-152"><a href="#GitBetter.do_new_repo-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_repo-153"><a href="#GitBetter.do_new_repo-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_repo-154"><a href="#GitBetter.do_new_repo-154"><span class="linenos">154</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a new git repo in this directory.</p>
 </div>
 
 
@@ -920,17 +1046,17 @@
         <span class="def">def</span>
         <span class="name">do_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-128"><a href="#GitBetter.do_new_branch-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_branch-129"><a href="#GitBetter.do_new_branch-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_branch-130"><a href="#GitBetter.do_new_branch-130"><span class="linenos">130</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-156"><a href="#GitBetter.do_new_branch-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_branch-157"><a href="#GitBetter.do_new_branch-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named after the supplied arg.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_branch-158"><a href="#GitBetter.do_new_branch-158"><span class="linenos">158</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch named after the supplied arg.</p>
 </div>
 
 
@@ -943,21 +1069,21 @@
         <span class="def">def</span>
         <span class="name">do_new_gh_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_gh_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_gh_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-132"><a href="#GitBetter.do_new_gh_remote-132"><span class="linenos">132</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_new_gh_remote-133"><a href="#GitBetter.do_new_gh_remote-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_gh_remote-134"><a href="#GitBetter.do_new_gh_remote-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter.do_new_gh_remote-135"><a href="#GitBetter.do_new_gh_remote-135"><span class="linenos">135</span></a>
-</span><span id="GitBetter.do_new_gh_remote-136"><a href="#GitBetter.do_new_gh_remote-136"><span class="linenos">136</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_gh_remote-137"><a href="#GitBetter.do_new_gh_remote-137"><span class="linenos">137</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="GitBetter.do_new_gh_remote-138"><a href="#GitBetter.do_new_gh_remote-138"><span class="linenos">138</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-160"><a href="#GitBetter.do_new_gh_remote-160"><span class="linenos">160</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_new_gh_remote-161"><a href="#GitBetter.do_new_gh_remote-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_gh_remote-162"><a href="#GitBetter.do_new_gh_remote-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter.do_new_gh_remote-163"><a href="#GitBetter.do_new_gh_remote-163"><span class="linenos">163</span></a>
+</span><span id="GitBetter.do_new_gh_remote-164"><a href="#GitBetter.do_new_gh_remote-164"><span class="linenos">164</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_gh_remote-165"><a href="#GitBetter.do_new_gh_remote-165"><span class="linenos">165</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
+</span><span id="GitBetter.do_new_gh_remote-166"><a href="#GitBetter.do_new_gh_remote-166"><span class="linenos">166</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a remote GitHub repository for this repo.</p>
 
 <p>GitHub CLI must be installed and configured for this to work.</p>
 </div>
@@ -971,17 +1097,17 @@
         <span class="def">def</span>
         <span class="name">do_initcommit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-140"><a href="#GitBetter.do_initcommit-140"><span class="linenos">140</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_initcommit-141"><a href="#GitBetter.do_initcommit-141"><span class="linenos">141</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_initcommit-142"><a href="#GitBetter.do_initcommit-142"><span class="linenos">142</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-168"><a href="#GitBetter.do_initcommit-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_initcommit-169"><a href="#GitBetter.do_initcommit-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_initcommit-170"><a href="#GitBetter.do_initcommit-170"><span class="linenos">170</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with message "Initial Commit".</p>
 </div>
 
 
@@ -993,17 +1119,17 @@
         <span class="def">def</span>
         <span class="name">do_undo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-144"><a href="#GitBetter.do_undo-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_undo-145"><a href="#GitBetter.do_undo-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_undo-146"><a href="#GitBetter.do_undo-146"><span class="linenos">146</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-172"><a href="#GitBetter.do_undo-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_undo-173"><a href="#GitBetter.do_undo-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_undo-174"><a href="#GitBetter.do_undo-174"><span class="linenos">174</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo all uncommitted changes.</p>
 </div>
 
 
@@ -1016,19 +1142,19 @@
         <span class="def">def</span>
         <span class="name">do_add</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-148"><a href="#GitBetter.do_add-148"><span class="linenos">148</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_add-149"><a href="#GitBetter.do_add-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_add-150"><a href="#GitBetter.do_add-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter.do_add-151"><a href="#GitBetter.do_add-151"><span class="linenos">151</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add-152"><a href="#GitBetter.do_add-152"><span class="linenos">152</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-176"><a href="#GitBetter.do_add-176"><span class="linenos">176</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_add-177"><a href="#GitBetter.do_add-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_add-178"><a href="#GitBetter.do_add-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter.do_add-179"><a href="#GitBetter.do_add-179"><span class="linenos">179</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add-180"><a href="#GitBetter.do_add-180"><span class="linenos">180</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage a list of files.
 If no files are given, all files will be added.</p>
 </div>
 
@@ -1041,21 +1167,21 @@
         <span class="def">def</span>
         <span class="name">do_commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-154"><a href="#GitBetter.do_commit-154"><span class="linenos">154</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-155"><a href="#GitBetter.do_commit-155"><span class="linenos">155</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commit-156"><a href="#GitBetter.do_commit-156"><span class="linenos">156</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-157"><a href="#GitBetter.do_commit-157"><span class="linenos">157</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter.do_commit-158"><a href="#GitBetter.do_commit-158"><span class="linenos">158</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-159"><a href="#GitBetter.do_commit-159"><span class="linenos">159</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter.do_commit-160"><a href="#GitBetter.do_commit-160"><span class="linenos">160</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-182"><a href="#GitBetter.do_commit-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-183"><a href="#GitBetter.do_commit-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commit-184"><a href="#GitBetter.do_commit-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-185"><a href="#GitBetter.do_commit-185"><span class="linenos">185</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter.do_commit-186"><a href="#GitBetter.do_commit-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-187"><a href="#GitBetter.do_commit-187"><span class="linenos">187</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter.do_commit-188"><a href="#GitBetter.do_commit-188"><span class="linenos">188</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Commit staged files with this message.</p>
 </div>
 
 
@@ -1068,18 +1194,18 @@
         <span class="def">def</span>
         <span class="name">do_commitf</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitf-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitf"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-162"><a href="#GitBetter.do_commitf-162"><span class="linenos">162</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_commitf-163"><a href="#GitBetter.do_commitf-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitf-164"><a href="#GitBetter.do_commitf-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitf-165"><a href="#GitBetter.do_commitf-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-190"><a href="#GitBetter.do_commitf-190"><span class="linenos">190</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_commitf-191"><a href="#GitBetter.do_commitf-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitf-192"><a href="#GitBetter.do_commitf-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitf-193"><a href="#GitBetter.do_commitf-193"><span class="linenos">193</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit a list of files.</p>
 </div>
 
 
@@ -1091,22 +1217,22 @@
         <span class="def">def</span>
         <span class="name">do_commitall</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitall-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitall"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-167"><a href="#GitBetter.do_commitall-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-168"><a href="#GitBetter.do_commitall-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitall-169"><a href="#GitBetter.do_commitall-169"><span class="linenos">169</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-170"><a href="#GitBetter.do_commitall-170"><span class="linenos">170</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter.do_commitall-171"><a href="#GitBetter.do_commitall-171"><span class="linenos">171</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-172"><a href="#GitBetter.do_commitall-172"><span class="linenos">172</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter.do_commitall-173"><a href="#GitBetter.do_commitall-173"><span class="linenos">173</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter.do_commitall-174"><a href="#GitBetter.do_commitall-174"><span class="linenos">174</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-195"><a href="#GitBetter.do_commitall-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-196"><a href="#GitBetter.do_commitall-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitall-197"><a href="#GitBetter.do_commitall-197"><span class="linenos">197</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-198"><a href="#GitBetter.do_commitall-198"><span class="linenos">198</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter.do_commitall-199"><a href="#GitBetter.do_commitall-199"><span class="linenos">199</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-200"><a href="#GitBetter.do_commitall-200"><span class="linenos">200</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter.do_commitall-201"><a href="#GitBetter.do_commitall-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter.do_commitall-202"><a href="#GitBetter.do_commitall-202"><span class="linenos">202</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with this message.</p>
 </div>
 
 
@@ -1118,17 +1244,17 @@
         <span class="def">def</span>
         <span class="name">do_switch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_switch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_switch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-176"><a href="#GitBetter.do_switch-176"><span class="linenos">176</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_switch-177"><a href="#GitBetter.do_switch-177"><span class="linenos">177</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_switch-178"><a href="#GitBetter.do_switch-178"><span class="linenos">178</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-204"><a href="#GitBetter.do_switch-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_switch-205"><a href="#GitBetter.do_switch-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_switch-206"><a href="#GitBetter.do_switch-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to this branch.</p>
 </div>
 
 
@@ -1140,18 +1266,18 @@
         <span class="def">def</span>
         <span class="name">do_add_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-180"><a href="#GitBetter.do_add_url-180"><span class="linenos">180</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_add_url-181"><a href="#GitBetter.do_add_url-181"><span class="linenos">181</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add_url-182"><a href="#GitBetter.do_add_url-182"><span class="linenos">182</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter.do_add_url-183"><a href="#GitBetter.do_add_url-183"><span class="linenos">183</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-208"><a href="#GitBetter.do_add_url-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_add_url-209"><a href="#GitBetter.do_add_url-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add_url-210"><a href="#GitBetter.do_add_url-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter.do_add_url-211"><a href="#GitBetter.do_add_url-211"><span class="linenos">211</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add remote url for repo and push repo.</p>
 </div>
 
 
@@ -1163,17 +1289,17 @@
         <span class="def">def</span>
         <span class="name">do_push_new</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push_new-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push_new"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-185"><a href="#GitBetter.do_push_new-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push_new-186"><a href="#GitBetter.do_push_new-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push_new-187"><a href="#GitBetter.do_push_new-187"><span class="linenos">187</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-213"><a href="#GitBetter.do_push_new-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push_new-214"><a href="#GitBetter.do_push_new-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push_new-215"><a href="#GitBetter.do_push_new-215"><span class="linenos">215</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push this new branch to origin with -u flag.</p>
 </div>
 
 
@@ -1185,19 +1311,19 @@
         <span class="def">def</span>
         <span class="name">do_push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-189"><a href="#GitBetter.do_push-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push-190"><a href="#GitBetter.do_push-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="GitBetter.do_push-191"><a href="#GitBetter.do_push-191"><span class="linenos">191</span></a>
-</span><span id="GitBetter.do_push-192"><a href="#GitBetter.do_push-192"><span class="linenos">192</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push-193"><a href="#GitBetter.do_push-193"><span class="linenos">193</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-217"><a href="#GitBetter.do_push-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push-218"><a href="#GitBetter.do_push-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter.do_push-219"><a href="#GitBetter.do_push-219"><span class="linenos">219</span></a>
+</span><span id="GitBetter.do_push-220"><a href="#GitBetter.do_push-220"><span class="linenos">220</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push-221"><a href="#GitBetter.do_push-221"><span class="linenos">221</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git push</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git push</code> accepts.</p>
 </div>
@@ -1211,19 +1337,19 @@
         <span class="def">def</span>
         <span class="name">do_pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-195"><a href="#GitBetter.do_pull-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull-196"><a href="#GitBetter.do_pull-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="GitBetter.do_pull-197"><a href="#GitBetter.do_pull-197"><span class="linenos">197</span></a>
-</span><span id="GitBetter.do_pull-198"><a href="#GitBetter.do_pull-198"><span class="linenos">198</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull-199"><a href="#GitBetter.do_pull-199"><span class="linenos">199</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-223"><a href="#GitBetter.do_pull-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull-224"><a href="#GitBetter.do_pull-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter.do_pull-225"><a href="#GitBetter.do_pull-225"><span class="linenos">225</span></a>
+</span><span id="GitBetter.do_pull-226"><a href="#GitBetter.do_pull-226"><span class="linenos">226</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull-227"><a href="#GitBetter.do_pull-227"><span class="linenos">227</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git pull</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git pull</code> accepts.</p>
 </div>
@@ -1237,17 +1363,17 @@
         <span class="def">def</span>
         <span class="name">do_list_branches</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_list_branches-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_list_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_list_branches-201"><a href="#GitBetter.do_list_branches-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_list_branches-202"><a href="#GitBetter.do_list_branches-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_list_branches-203"><a href="#GitBetter.do_list_branches-203"><span class="linenos">203</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_list_branches-229"><a href="#GitBetter.do_list_branches-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_list_branches-230"><a href="#GitBetter.do_list_branches-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_list_branches-231"><a href="#GitBetter.do_list_branches-231"><span class="linenos">231</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Show local and remote branches.</p>
 </div>
 
 
@@ -1259,17 +1385,17 @@
         <span class="def">def</span>
         <span class="name">do_loggy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_loggy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_loggy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-205"><a href="#GitBetter.do_loggy-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_loggy-206"><a href="#GitBetter.do_loggy-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_loggy-207"><a href="#GitBetter.do_loggy-207"><span class="linenos">207</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-233"><a href="#GitBetter.do_loggy-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_loggy-234"><a href="#GitBetter.do_loggy-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_loggy-235"><a href="#GitBetter.do_loggy-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
@@ -1281,17 +1407,17 @@
         <span class="def">def</span>
         <span class="name">do_merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-209"><a href="#GitBetter.do_merge-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_merge-210"><a href="#GitBetter.do_merge-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_merge-211"><a href="#GitBetter.do_merge-211"><span class="linenos">211</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-237"><a href="#GitBetter.do_merge-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_merge-238"><a href="#GitBetter.do_merge-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_merge-239"><a href="#GitBetter.do_merge-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge supplied <code>branch_name</code> with the currently active branch.</p>
 </div>
 
 
@@ -1303,17 +1429,17 @@
         <span class="def">def</span>
         <span class="name">do_tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-213"><a href="#GitBetter.do_tag-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_tag-214"><a href="#GitBetter.do_tag-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_tag-215"><a href="#GitBetter.do_tag-215"><span class="linenos">215</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-241"><a href="#GitBetter.do_tag-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_tag-242"><a href="#GitBetter.do_tag-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_tag-243"><a href="#GitBetter.do_tag-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Tag current commit with <code>tag_id</code>.</p>
 </div>
 
 
@@ -1326,18 +1452,18 @@
         <span class="def">def</span>
         <span class="name">do_amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-217"><a href="#GitBetter.do_amend-217"><span class="linenos">217</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_amend-218"><a href="#GitBetter.do_amend-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_amend-219"><a href="#GitBetter.do_amend-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_amend-220"><a href="#GitBetter.do_amend-220"><span class="linenos">220</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-245"><a href="#GitBetter.do_amend-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_amend-246"><a href="#GitBetter.do_amend-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_amend-247"><a href="#GitBetter.do_amend-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_amend-248"><a href="#GitBetter.do_amend-248"><span class="linenos">248</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage files and add to previous commit.</p>
 </div>
 
 
@@ -1350,18 +1476,18 @@
         <span class="def">def</span>
         <span class="name">do_delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-222"><a href="#GitBetter.do_delete_branch-222"><span class="linenos">222</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_delete_branch-223"><a href="#GitBetter.do_delete_branch-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_branch-224"><a href="#GitBetter.do_delete_branch-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_branch-225"><a href="#GitBetter.do_delete_branch-225"><span class="linenos">225</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-250"><a href="#GitBetter.do_delete_branch-250"><span class="linenos">250</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_delete_branch-251"><a href="#GitBetter.do_delete_branch-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_branch-252"><a href="#GitBetter.do_delete_branch-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_branch-253"><a href="#GitBetter.do_delete_branch-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete branch.</p>
 </div>
 
 
@@ -1373,17 +1499,17 @@
         <span class="def">def</span>
         <span class="name">do_pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-227"><a href="#GitBetter.do_pull_branch-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull_branch-228"><a href="#GitBetter.do_pull_branch-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull_branch-229"><a href="#GitBetter.do_pull_branch-229"><span class="linenos">229</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-255"><a href="#GitBetter.do_pull_branch-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull_branch-256"><a href="#GitBetter.do_pull_branch-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull_branch-257"><a href="#GitBetter.do_pull_branch-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull this branch from the origin.</p>
 </div>
 
 
@@ -1395,20 +1521,20 @@
         <span class="def">def</span>
         <span class="name">do_ignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_ignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_ignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-231"><a href="#GitBetter.do_ignore-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_ignore-232"><a href="#GitBetter.do_ignore-232"><span class="linenos">232</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_ignore-233"><a href="#GitBetter.do_ignore-233"><span class="linenos">233</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter.do_ignore-234"><a href="#GitBetter.do_ignore-234"><span class="linenos">234</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-235"><a href="#GitBetter.do_ignore-235"><span class="linenos">235</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-236"><a href="#GitBetter.do_ignore-236"><span class="linenos">236</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_ignore-261"><a href="#GitBetter.do_ignore-261"><span class="linenos">261</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter.do_ignore-262"><a href="#GitBetter.do_ignore-262"><span class="linenos">262</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-263"><a href="#GitBetter.do_ignore-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-264"><a href="#GitBetter.do_ignore-264"><span class="linenos">264</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add the list of patterns to <code>.gitignore</code>.</p>
 </div>
 
 
@@ -1420,21 +1546,21 @@
         <span class="def">def</span>
         <span class="name">do_make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-238"><a href="#GitBetter.do_make_private-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_private-239"><a href="#GitBetter.do_make_private-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter.do_make_private-240"><a href="#GitBetter.do_make_private-240"><span class="linenos">240</span></a>
-</span><span id="GitBetter.do_make_private-241"><a href="#GitBetter.do_make_private-241"><span class="linenos">241</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_private-242"><a href="#GitBetter.do_make_private-242"><span class="linenos">242</span></a>
-</span><span id="GitBetter.do_make_private-243"><a href="#GitBetter.do_make_private-243"><span class="linenos">243</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_private-244"><a href="#GitBetter.do_make_private-244"><span class="linenos">244</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a>
+</span><span id="GitBetter.do_make_private-269"><a href="#GitBetter.do_make_private-269"><span class="linenos">269</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_private-270"><a href="#GitBetter.do_make_private-270"><span class="linenos">270</span></a>
+</span><span id="GitBetter.do_make_private-271"><a href="#GitBetter.do_make_private-271"><span class="linenos">271</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_private-272"><a href="#GitBetter.do_make_private-272"><span class="linenos">272</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo private.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1450,21 +1576,21 @@
         <span class="def">def</span>
         <span class="name">do_make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-246"><a href="#GitBetter.do_make_public-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_public-247"><a href="#GitBetter.do_make_public-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter.do_make_public-248"><a href="#GitBetter.do_make_public-248"><span class="linenos">248</span></a>
-</span><span id="GitBetter.do_make_public-249"><a href="#GitBetter.do_make_public-249"><span class="linenos">249</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_public-250"><a href="#GitBetter.do_make_public-250"><span class="linenos">250</span></a>
-</span><span id="GitBetter.do_make_public-251"><a href="#GitBetter.do_make_public-251"><span class="linenos">251</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_public-252"><a href="#GitBetter.do_make_public-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a>
+</span><span id="GitBetter.do_make_public-277"><a href="#GitBetter.do_make_public-277"><span class="linenos">277</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_public-278"><a href="#GitBetter.do_make_public-278"><span class="linenos">278</span></a>
+</span><span id="GitBetter.do_make_public-279"><a href="#GitBetter.do_make_public-279"><span class="linenos">279</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_public-280"><a href="#GitBetter.do_make_public-280"><span class="linenos">280</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo public.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1480,23 +1606,23 @@
         <span class="def">def</span>
         <span class="name">do_delete_gh_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_gh_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_gh_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-254"><a href="#GitBetter.do_delete_gh_repo-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_gh_repo-255"><a href="#GitBetter.do_delete_gh_repo-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter.do_delete_gh_repo-256"><a href="#GitBetter.do_delete_gh_repo-256"><span class="linenos">256</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-257"><a href="#GitBetter.do_delete_gh_repo-257"><span class="linenos">257</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_delete_gh_repo-258"><a href="#GitBetter.do_delete_gh_repo-258"><span class="linenos">258</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-259"><a href="#GitBetter.do_delete_gh_repo-259"><span class="linenos">259</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter.do_delete_gh_repo-260"><a href="#GitBetter.do_delete_gh_repo-260"><span class="linenos">260</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-261"><a href="#GitBetter.do_delete_gh_repo-261"><span class="linenos">261</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_gh_repo-262"><a href="#GitBetter.do_delete_gh_repo-262"><span class="linenos">262</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-287"><a href="#GitBetter.do_delete_gh_repo-287"><span class="linenos">287</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter.do_delete_gh_repo-288"><a href="#GitBetter.do_delete_gh_repo-288"><span class="linenos">288</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-289"><a href="#GitBetter.do_delete_gh_repo-289"><span class="linenos">289</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_gh_repo-290"><a href="#GitBetter.do_delete_gh_repo-290"><span class="linenos">290</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete this repo from GitHub.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1515,27 +1641,25 @@
                 <dd id="GitBetter.precmd" class="function">precmd</dd>
                 <dd id="GitBetter.postcmd" class="function">postcmd</dd>
                 <dd id="GitBetter.preloop" class="function">preloop</dd>
                 <dd id="GitBetter.postloop" class="function">postloop</dd>
                 <dd id="GitBetter.parseline" class="function">parseline</dd>
                 <dd id="GitBetter.onecmd" class="function">onecmd</dd>
                 <dd id="GitBetter.emptyline" class="function">emptyline</dd>
-                <dd id="GitBetter.default" class="function">default</dd>
                 <dd id="GitBetter.completedefault" class="function">completedefault</dd>
                 <dd id="GitBetter.completenames" class="function">completenames</dd>
                 <dd id="GitBetter.complete" class="function">complete</dd>
                 <dd id="GitBetter.get_names" class="function">get_names</dd>
                 <dd id="GitBetter.complete_help" class="function">complete_help</dd>
                 <dd id="GitBetter.print_topics" class="function">print_topics</dd>
                 <dd id="GitBetter.columnize" class="function">columnize</dd>
 
             </div>
             <div><dt>argshell.argshell.ArgShell</dt>
                                 <dd id="GitBetter.do_quit" class="function">do_quit</dd>
-                <dd id="GitBetter.do_help" class="function">do_help</dd>
                 <dd id="GitBetter.cmdloop" class="function">cmdloop</dd>
 
             </div>
                                 </dl>
                             </div>
                 </section>
                 <section id="main">
@@ -1545,16 +1669,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-265"><a href="#main-265"><span class="linenos">265</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-266"><a href="#main-266"><span class="linenos">266</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-293"><a href="#main-293"><span class="linenos">293</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-294"><a href="#main-294"><span class="linenos">294</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -6,16 +6,18 @@
     * new_remote_parser
     * commit_files_parser
     * amend_files_parser
     * delete_branch_parser
     * recurse_files
     * files_postparser
     * GitBetter
+          o default
+          o do_help
+          o do_toggle_unrecognized_command_behavior
           o do_cd
-          o do_cwd
           o do_cmd
           o do_git
           o do_new_repo
           o do_new_branch
           o do_new_gh_remote
           o do_initcommit
           o do_undo
@@ -152,188 +154,223 @@
 _96    return args
 _97
 _98
 _99class GitBetter(ArgShell):
 100    """GitBetter Shell."""
 101
 102    intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
-103    prompt = "gitbetter>"
-104
-105    def do_cd(self, path: str):
-106        """Change current working directory to `path`."""
-107        os.chdir(path)
-108
-109    def do_cwd(self, _: str):
-110        """Print the current working directory."""
-111        print(Pathier.cwd())
-112
-113    def do_cmd(self, command: str):
-114        """Execute arbitrary command in the terminal so you don't have to
-quit gitbetter to run other programs/commands."""
-115        os.system(command)
-116
-117    def do_git(self, arg: str):
-118        """Directly execute `git {arg}`.
-119
-120        i.e. You can still do everything directly invoking git can do."""
-121        git.execute(arg)
+103    prompt = f"gitbetter::{Pathier.cwd()}>"
+104    execute_in_terminal_if_unrecognized = True
+105
+106    def default(self, line: str):
+107        if self.execute_in_terminal_if_unrecognized:
+108            os.system(line)
+109        else:
+110            super().default(line)
+111
+112    def do_help(self, arg: str):
+113        """List available commands with "help" or detailed help with "help
+cmd"."""
+114        super().do_help(arg)
+115        if not arg:
+116            print(self.unrecognized_command_behavior_status)
+117            if self.execute_in_terminal_if_unrecognized:
+118                print(
+119                    "^Essentially makes this shell function as a super-shell
+of whatever shell you launched gitbetter from.^"
+120                )
+121        print()
 122
-123    def do_new_repo(self, _: str):
-124        """Create a new git repo in this directory."""
-125        git.new_repo()
+123    @property
+124    def unrecognized_command_behavior_status(self):
+125        return f"Unrecognized command behavior: {'Execute with os.system()'
+if self.execute_in_terminal_if_unrecognized else 'Print unknown syntax error'}"
 126
-127    def do_new_branch(self, name: str):
-128        """Create and switch to a new branch named after the supplied
+127    def do_toggle_unrecognized_command_behavior(self, arg: str):
+128        """Toggle whether the shell will attempt to execute unrecognized
+commands as system commands in the terminal.
+129        When on (the default), `GitBetter` will treat unrecognized commands
+as if you added the `cmd` command in front of the input, i.e. `os.system
+(your_input)`.
+130        When off, an `unknown syntax` message will be printed and no
+commands will be executed."""
+131        self.execute_in_terminal_if_unrecognized = (
+132            not self.execute_in_terminal_if_unrecognized
+133        )
+134        print(self.unrecognized_command_behavior_status)
+135
+136    def do_cd(self, path: str):
+137        """Change current working directory to `path`."""
+138        os.chdir(path)
+139        self.prompt = f"gitbetter::{Pathier.cwd()}>"
+140
+141    def do_cmd(self, command: str):
+142        """Execute arbitrary command in the terminal so you don't have to
+quit gitbetter to run other programs/commands."""
+143        os.system(command)
+144
+145    def do_git(self, arg: str):
+146        """Directly execute `git {arg}`.
+147
+148        i.e. You can still do everything directly invoking git can do."""
+149        git.execute(arg)
+150
+151    def do_new_repo(self, _: str):
+152        """Create a new git repo in this directory."""
+153        git.new_repo()
+154
+155    def do_new_branch(self, name: str):
+156        """Create and switch to a new branch named after the supplied
 arg."""
-129        git.create_new_branch(name)
-130
-131    @with_parser(new_remote_parser)
-132    def do_new_gh_remote(self, args: Namespace):
-133        """Create a remote GitHub repository for this repo.
-134
-135        GitHub CLI must be installed and configured for this to work."""
-136        name = Pathier.cwd().stem
-137        git.create_remote(name, args.public)
-138
-139    def do_initcommit(self, _: str):
-140        """Stage and commit all files with message "Initial Commit"."""
-141        git.initcommit()
-142
-143    def do_undo(self, _: str):
-144        """Undo all uncommitted changes."""
-145        git.undo()
-146
-147    @with_parser(amend_files_parser, [files_postparser])
-148    def do_add(self, args: Namespace):
-149        """Stage a list of files.
-150        If no files are given, all files will be added."""
-151        git.add(None if not args.files else args.files)
-152
-153    def do_commit(self, message: str):
-154        """Commit staged files with this message."""
-155        if not message.startswith('"'):
-156            message = '"' + message
-157        if not message.endswith('"'):
-158            message += '"'
-159        git.commit(f"-m {message}")
-160
-161    @with_parser(commit_files_parser, [files_postparser])
-162    def do_commitf(self, args: Namespace):
-163        """Stage and commit a list of files."""
-164        git.commit_files(args.files, args.message)
-165
-166    def do_commitall(self, message: str):
-167        """Stage and commit all files with this message."""
-168        if not message.startswith('"'):
-169            message = '"' + message
-170        if not message.endswith('"'):
-171            message += '"'
-172        git.add()
-173        git.commit(f"-m {message}")
+157        git.create_new_branch(name)
+158
+159    @with_parser(new_remote_parser)
+160    def do_new_gh_remote(self, args: Namespace):
+161        """Create a remote GitHub repository for this repo.
+162
+163        GitHub CLI must be installed and configured for this to work."""
+164        name = Pathier.cwd().stem
+165        git.create_remote(name, args.public)
+166
+167    def do_initcommit(self, _: str):
+168        """Stage and commit all files with message "Initial Commit"."""
+169        git.initcommit()
+170
+171    def do_undo(self, _: str):
+172        """Undo all uncommitted changes."""
+173        git.undo()
 174
-175    def do_switch(self, branch_name: str):
-176        """Switch to this branch."""
-177        git.switch_branch(branch_name)
-178
-179    def do_add_url(self, url: str):
-180        """Add remote url for repo and push repo."""
-181        git.add_remote_url(url)
-182        git.push("-u origin main")
-183
-184    def do_push_new(self, branch_name: str):
-185        """Push this new branch to origin with -u flag."""
-186        git.push_new_branch(branch_name)
-187
-188    def do_push(self, args: str):
-189        """Execute `git push`.
-190
-191        `args` can be any additional args that `git push` accepts."""
-192        git.push(args)
+175    @with_parser(amend_files_parser, [files_postparser])
+176    def do_add(self, args: Namespace):
+177        """Stage a list of files.
+178        If no files are given, all files will be added."""
+179        git.add(None if not args.files else args.files)
+180
+181    def do_commit(self, message: str):
+182        """Commit staged files with this message."""
+183        if not message.startswith('"'):
+184            message = '"' + message
+185        if not message.endswith('"'):
+186            message += '"'
+187        git.commit(f"-m {message}")
+188
+189    @with_parser(commit_files_parser, [files_postparser])
+190    def do_commitf(self, args: Namespace):
+191        """Stage and commit a list of files."""
+192        git.commit_files(args.files, args.message)
 193
-194    def do_pull(self, args: str):
-195        """Execute `git pull`.
-196
-197        `args` can be any additional args that `git pull` accepts."""
-198        git.pull(args)
-199
-200    def do_list_branches(self, _: str):
-201        """Show local and remote branches."""
-202        git.list_branches()
-203
-204    def do_loggy(self, _: str):
-205        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-206        git.loggy()
-207
-208    def do_merge(self, branch_name: str):
-209        """Merge supplied `branch_name` with the currently active branch."""
-210        git.merge(branch_name)
+194    def do_commitall(self, message: str):
+195        """Stage and commit all files with this message."""
+196        if not message.startswith('"'):
+197            message = '"' + message
+198        if not message.endswith('"'):
+199            message += '"'
+200        git.add()
+201        git.commit(f"-m {message}")
+202
+203    def do_switch(self, branch_name: str):
+204        """Switch to this branch."""
+205        git.switch_branch(branch_name)
+206
+207    def do_add_url(self, url: str):
+208        """Add remote url for repo and push repo."""
+209        git.add_remote_url(url)
+210        git.push("-u origin main")
 211
-212    def do_tag(self, tag_id: str):
-213        """Tag current commit with `tag_id`."""
-214        git.tag(tag_id)
+212    def do_push_new(self, branch_name: str):
+213        """Push this new branch to origin with -u flag."""
+214        git.push_new_branch(branch_name)
 215
-216    @with_parser(amend_files_parser, [files_postparser])
-217    def do_amend(self, args: Namespace):
-218        """Stage files and add to previous commit."""
-219        git.amend(args.files)
-220
-221    @with_parser(delete_branch_parser)
-222    def do_delete_branch(self, args: Namespace):
-223        """Delete branch."""
-224        git.delete_branch(args.branch, not args.remote)
-225
-226    def do_pull_branch(self, branch: str):
-227        """Pull this branch from the origin."""
-228        git.pull_branch(branch)
-229
-230    def do_ignore(self, patterns: str):
-231        """Add the list of patterns to `.gitignore`."""
-232        patterns = "\n".join(patterns.split())
-233        path = Pathier(".gitignore")
-234        path.append("\n")
-235        path.append(patterns, False)
-236
-237    def do_make_private(self, owner: str):
-238        """Make the GitHub remote for this repo private.
+216    def do_push(self, args: str):
+217        """Execute `git push`.
+218
+219        `args` can be any additional args that `git push` accepts."""
+220        git.push(args)
+221
+222    def do_pull(self, args: str):
+223        """Execute `git pull`.
+224
+225        `args` can be any additional args that `git pull` accepts."""
+226        git.pull(args)
+227
+228    def do_list_branches(self, _: str):
+229        """Show local and remote branches."""
+230        git.list_branches()
+231
+232    def do_loggy(self, _: str):
+233        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+234        git.loggy()
+235
+236    def do_merge(self, branch_name: str):
+237        """Merge supplied `branch_name` with the currently active branch."""
+238        git.merge(branch_name)
 239
-240        Expects an argument for the repo owner, i.e. the `OWNER` in
+240    def do_tag(self, tag_id: str):
+241        """Tag current commit with `tag_id`."""
+242        git.tag(tag_id)
+243
+244    @with_parser(amend_files_parser, [files_postparser])
+245    def do_amend(self, args: Namespace):
+246        """Stage files and add to previous commit."""
+247        git.amend(args.files)
+248
+249    @with_parser(delete_branch_parser)
+250    def do_delete_branch(self, args: Namespace):
+251        """Delete branch."""
+252        git.delete_branch(args.branch, not args.remote)
+253
+254    def do_pull_branch(self, branch: str):
+255        """Pull this branch from the origin."""
+256        git.pull_branch(branch)
+257
+258    def do_ignore(self, patterns: str):
+259        """Add the list of patterns to `.gitignore`."""
+260        patterns = "\n".join(patterns.split())
+261        path = Pathier(".gitignore")
+262        path.append("\n")
+263        path.append(patterns, False)
+264
+265    def do_make_private(self, owner: str):
+266        """Make the GitHub remote for this repo private.
+267
+268        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-241
-242        This repo must exist and GitHub CLI must be installed and
+269
+270        This repo must exist and GitHub CLI must be installed and
 configured."""
-243        git.make_private(owner, Pathier.cwd().stem)
-244
-245    def do_make_public(self, owner: str):
-246        """Make the GitHub remote for this repo public.
-247
-248        Expects an argument for the repo owner, i.e. the `OWNER` in
+271        git.make_private(owner, Pathier.cwd().stem)
+272
+273    def do_make_public(self, owner: str):
+274        """Make the GitHub remote for this repo public.
+275
+276        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-249
-250        This repo must exist and GitHub CLI must be installed and
+277
+278        This repo must exist and GitHub CLI must be installed and
 configured."""
-251        git.make_public(owner, Pathier.cwd().stem)
-252
-253    def do_delete_gh_repo(self, owner: str):
-254        """Delete this repo from GitHub.
-255
-256        Expects an argument for the repo owner, i.e. the `OWNER` in
+279        git.make_public(owner, Pathier.cwd().stem)
+280
+281    def do_delete_gh_repo(self, owner: str):
+282        """Delete this repo from GitHub.
+283
+284        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-257
-258        GitHub CLI must be installed and configured.
-259
-260        May require you to reauthorize and rerun command."""
-261        git.delete_remote(owner, Pathier.cwd().stem)
-262
-263
-264def main():
-265    GitBetter().cmdloop()
-266
-267
-268if __name__ == "__main__":
-269    main()
+285
+286        GitHub CLI must be installed and configured.
+287
+288        May require you to reauthorize and rerun command."""
+289        git.delete_remote(owner, Pathier.cwd().stem)
+290
+291
+292def main():
+293    GitBetter().cmdloop()
+294
+295
+296if __name__ == "__main__":
+297    main()
   ⁰
 def new_remote_parser() -> argshell.argshell.ArgShellParser: View Source
 10def new_remote_parser() -> ArgShellParser:
 11    parser = ArgShellParser()
 12    parser.add_argument(
 13        "--public",
 14        action="store_true",
@@ -433,423 +470,496 @@
 97    return args
   ⁰
 class GitBetter(argshell.argshell.ArgShell): View Source
 100class GitBetter(ArgShell):
 101    """GitBetter Shell."""
 102
 103    intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
-104    prompt = "gitbetter>"
-105
-106    def do_cd(self, path: str):
-107        """Change current working directory to `path`."""
-108        os.chdir(path)
-109
-110    def do_cwd(self, _: str):
-111        """Print the current working directory."""
-112        print(Pathier.cwd())
-113
-114    def do_cmd(self, command: str):
-115        """Execute arbitrary command in the terminal so you don't have to
-quit gitbetter to run other programs/commands."""
-116        os.system(command)
-117
-118    def do_git(self, arg: str):
-119        """Directly execute `git {arg}`.
-120
-121        i.e. You can still do everything directly invoking git can do."""
-122        git.execute(arg)
+104    prompt = f"gitbetter::{Pathier.cwd()}>"
+105    execute_in_terminal_if_unrecognized = True
+106
+107    def default(self, line: str):
+108        if self.execute_in_terminal_if_unrecognized:
+109            os.system(line)
+110        else:
+111            super().default(line)
+112
+113    def do_help(self, arg: str):
+114        """List available commands with "help" or detailed help with "help
+cmd"."""
+115        super().do_help(arg)
+116        if not arg:
+117            print(self.unrecognized_command_behavior_status)
+118            if self.execute_in_terminal_if_unrecognized:
+119                print(
+120                    "^Essentially makes this shell function as a super-shell
+of whatever shell you launched gitbetter from.^"
+121                )
+122        print()
 123
-124    def do_new_repo(self, _: str):
-125        """Create a new git repo in this directory."""
-126        git.new_repo()
+124    @property
+125    def unrecognized_command_behavior_status(self):
+126        return f"Unrecognized command behavior: {'Execute with os.system()'
+if self.execute_in_terminal_if_unrecognized else 'Print unknown syntax error'}"
 127
-128    def do_new_branch(self, name: str):
-129        """Create and switch to a new branch named after the supplied
+128    def do_toggle_unrecognized_command_behavior(self, arg: str):
+129        """Toggle whether the shell will attempt to execute unrecognized
+commands as system commands in the terminal.
+130        When on (the default), `GitBetter` will treat unrecognized commands
+as if you added the `cmd` command in front of the input, i.e. `os.system
+(your_input)`.
+131        When off, an `unknown syntax` message will be printed and no
+commands will be executed."""
+132        self.execute_in_terminal_if_unrecognized = (
+133            not self.execute_in_terminal_if_unrecognized
+134        )
+135        print(self.unrecognized_command_behavior_status)
+136
+137    def do_cd(self, path: str):
+138        """Change current working directory to `path`."""
+139        os.chdir(path)
+140        self.prompt = f"gitbetter::{Pathier.cwd()}>"
+141
+142    def do_cmd(self, command: str):
+143        """Execute arbitrary command in the terminal so you don't have to
+quit gitbetter to run other programs/commands."""
+144        os.system(command)
+145
+146    def do_git(self, arg: str):
+147        """Directly execute `git {arg}`.
+148
+149        i.e. You can still do everything directly invoking git can do."""
+150        git.execute(arg)
+151
+152    def do_new_repo(self, _: str):
+153        """Create a new git repo in this directory."""
+154        git.new_repo()
+155
+156    def do_new_branch(self, name: str):
+157        """Create and switch to a new branch named after the supplied
 arg."""
-130        git.create_new_branch(name)
-131
-132    @with_parser(new_remote_parser)
-133    def do_new_gh_remote(self, args: Namespace):
-134        """Create a remote GitHub repository for this repo.
-135
-136        GitHub CLI must be installed and configured for this to work."""
-137        name = Pathier.cwd().stem
-138        git.create_remote(name, args.public)
-139
-140    def do_initcommit(self, _: str):
-141        """Stage and commit all files with message "Initial Commit"."""
-142        git.initcommit()
-143
-144    def do_undo(self, _: str):
-145        """Undo all uncommitted changes."""
-146        git.undo()
-147
-148    @with_parser(amend_files_parser, [files_postparser])
-149    def do_add(self, args: Namespace):
-150        """Stage a list of files.
-151        If no files are given, all files will be added."""
-152        git.add(None if not args.files else args.files)
-153
-154    def do_commit(self, message: str):
-155        """Commit staged files with this message."""
-156        if not message.startswith('"'):
-157            message = '"' + message
-158        if not message.endswith('"'):
-159            message += '"'
-160        git.commit(f"-m {message}")
-161
-162    @with_parser(commit_files_parser, [files_postparser])
-163    def do_commitf(self, args: Namespace):
-164        """Stage and commit a list of files."""
-165        git.commit_files(args.files, args.message)
-166
-167    def do_commitall(self, message: str):
-168        """Stage and commit all files with this message."""
-169        if not message.startswith('"'):
-170            message = '"' + message
-171        if not message.endswith('"'):
-172            message += '"'
-173        git.add()
-174        git.commit(f"-m {message}")
+158        git.create_new_branch(name)
+159
+160    @with_parser(new_remote_parser)
+161    def do_new_gh_remote(self, args: Namespace):
+162        """Create a remote GitHub repository for this repo.
+163
+164        GitHub CLI must be installed and configured for this to work."""
+165        name = Pathier.cwd().stem
+166        git.create_remote(name, args.public)
+167
+168    def do_initcommit(self, _: str):
+169        """Stage and commit all files with message "Initial Commit"."""
+170        git.initcommit()
+171
+172    def do_undo(self, _: str):
+173        """Undo all uncommitted changes."""
+174        git.undo()
 175
-176    def do_switch(self, branch_name: str):
-177        """Switch to this branch."""
-178        git.switch_branch(branch_name)
-179
-180    def do_add_url(self, url: str):
-181        """Add remote url for repo and push repo."""
-182        git.add_remote_url(url)
-183        git.push("-u origin main")
-184
-185    def do_push_new(self, branch_name: str):
-186        """Push this new branch to origin with -u flag."""
-187        git.push_new_branch(branch_name)
-188
-189    def do_push(self, args: str):
-190        """Execute `git push`.
-191
-192        `args` can be any additional args that `git push` accepts."""
-193        git.push(args)
+176    @with_parser(amend_files_parser, [files_postparser])
+177    def do_add(self, args: Namespace):
+178        """Stage a list of files.
+179        If no files are given, all files will be added."""
+180        git.add(None if not args.files else args.files)
+181
+182    def do_commit(self, message: str):
+183        """Commit staged files with this message."""
+184        if not message.startswith('"'):
+185            message = '"' + message
+186        if not message.endswith('"'):
+187            message += '"'
+188        git.commit(f"-m {message}")
+189
+190    @with_parser(commit_files_parser, [files_postparser])
+191    def do_commitf(self, args: Namespace):
+192        """Stage and commit a list of files."""
+193        git.commit_files(args.files, args.message)
 194
-195    def do_pull(self, args: str):
-196        """Execute `git pull`.
-197
-198        `args` can be any additional args that `git pull` accepts."""
-199        git.pull(args)
-200
-201    def do_list_branches(self, _: str):
-202        """Show local and remote branches."""
-203        git.list_branches()
-204
-205    def do_loggy(self, _: str):
-206        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-207        git.loggy()
-208
-209    def do_merge(self, branch_name: str):
-210        """Merge supplied `branch_name` with the currently active branch."""
-211        git.merge(branch_name)
+195    def do_commitall(self, message: str):
+196        """Stage and commit all files with this message."""
+197        if not message.startswith('"'):
+198            message = '"' + message
+199        if not message.endswith('"'):
+200            message += '"'
+201        git.add()
+202        git.commit(f"-m {message}")
+203
+204    def do_switch(self, branch_name: str):
+205        """Switch to this branch."""
+206        git.switch_branch(branch_name)
+207
+208    def do_add_url(self, url: str):
+209        """Add remote url for repo and push repo."""
+210        git.add_remote_url(url)
+211        git.push("-u origin main")
 212
-213    def do_tag(self, tag_id: str):
-214        """Tag current commit with `tag_id`."""
-215        git.tag(tag_id)
+213    def do_push_new(self, branch_name: str):
+214        """Push this new branch to origin with -u flag."""
+215        git.push_new_branch(branch_name)
 216
-217    @with_parser(amend_files_parser, [files_postparser])
-218    def do_amend(self, args: Namespace):
-219        """Stage files and add to previous commit."""
-220        git.amend(args.files)
-221
-222    @with_parser(delete_branch_parser)
-223    def do_delete_branch(self, args: Namespace):
-224        """Delete branch."""
-225        git.delete_branch(args.branch, not args.remote)
-226
-227    def do_pull_branch(self, branch: str):
-228        """Pull this branch from the origin."""
-229        git.pull_branch(branch)
-230
-231    def do_ignore(self, patterns: str):
-232        """Add the list of patterns to `.gitignore`."""
-233        patterns = "\n".join(patterns.split())
-234        path = Pathier(".gitignore")
-235        path.append("\n")
-236        path.append(patterns, False)
-237
-238    def do_make_private(self, owner: str):
-239        """Make the GitHub remote for this repo private.
+217    def do_push(self, args: str):
+218        """Execute `git push`.
+219
+220        `args` can be any additional args that `git push` accepts."""
+221        git.push(args)
+222
+223    def do_pull(self, args: str):
+224        """Execute `git pull`.
+225
+226        `args` can be any additional args that `git pull` accepts."""
+227        git.pull(args)
+228
+229    def do_list_branches(self, _: str):
+230        """Show local and remote branches."""
+231        git.list_branches()
+232
+233    def do_loggy(self, _: str):
+234        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+235        git.loggy()
+236
+237    def do_merge(self, branch_name: str):
+238        """Merge supplied `branch_name` with the currently active branch."""
+239        git.merge(branch_name)
 240
-241        Expects an argument for the repo owner, i.e. the `OWNER` in
+241    def do_tag(self, tag_id: str):
+242        """Tag current commit with `tag_id`."""
+243        git.tag(tag_id)
+244
+245    @with_parser(amend_files_parser, [files_postparser])
+246    def do_amend(self, args: Namespace):
+247        """Stage files and add to previous commit."""
+248        git.amend(args.files)
+249
+250    @with_parser(delete_branch_parser)
+251    def do_delete_branch(self, args: Namespace):
+252        """Delete branch."""
+253        git.delete_branch(args.branch, not args.remote)
+254
+255    def do_pull_branch(self, branch: str):
+256        """Pull this branch from the origin."""
+257        git.pull_branch(branch)
+258
+259    def do_ignore(self, patterns: str):
+260        """Add the list of patterns to `.gitignore`."""
+261        patterns = "\n".join(patterns.split())
+262        path = Pathier(".gitignore")
+263        path.append("\n")
+264        path.append(patterns, False)
+265
+266    def do_make_private(self, owner: str):
+267        """Make the GitHub remote for this repo private.
+268
+269        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-242
-243        This repo must exist and GitHub CLI must be installed and
+270
+271        This repo must exist and GitHub CLI must be installed and
 configured."""
-244        git.make_private(owner, Pathier.cwd().stem)
-245
-246    def do_make_public(self, owner: str):
-247        """Make the GitHub remote for this repo public.
-248
-249        Expects an argument for the repo owner, i.e. the `OWNER` in
+272        git.make_private(owner, Pathier.cwd().stem)
+273
+274    def do_make_public(self, owner: str):
+275        """Make the GitHub remote for this repo public.
+276
+277        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-250
-251        This repo must exist and GitHub CLI must be installed and
+278
+279        This repo must exist and GitHub CLI must be installed and
 configured."""
-252        git.make_public(owner, Pathier.cwd().stem)
-253
-254    def do_delete_gh_repo(self, owner: str):
-255        """Delete this repo from GitHub.
-256
-257        Expects an argument for the repo owner, i.e. the `OWNER` in
+280        git.make_public(owner, Pathier.cwd().stem)
+281
+282    def do_delete_gh_repo(self, owner: str):
+283        """Delete this repo from GitHub.
+284
+285        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-258
-259        GitHub CLI must be installed and configured.
-260
-261        May require you to reauthorize and rerun command."""
-262        git.delete_remote(owner, Pathier.cwd().stem)
+286
+287        GitHub CLI must be installed and configured.
+288
+289        May require you to reauthorize and rerun command."""
+290        git.delete_remote(owner, Pathier.cwd().stem)
 GitBetter Shell.
 ⁰
+def default(self, line: str): View Source
+107    def default(self, line: str):
+108        if self.execute_in_terminal_if_unrecognized:
+109            os.system(line)
+110        else:
+111            super().default(line)
+Called on an input line when the command prefix is not recognized.
+If this method is not overridden, it prints an error message and returns.
+⁰
+def do_help(self, arg: str): View Source
+113    def do_help(self, arg: str):
+114        """List available commands with "help" or detailed help with "help
+cmd"."""
+115        super().do_help(arg)
+116        if not arg:
+117            print(self.unrecognized_command_behavior_status)
+118            if self.execute_in_terminal_if_unrecognized:
+119                print(
+120                    "^Essentially makes this shell function as a super-shell
+of whatever shell you launched gitbetter from.^"
+121                )
+122        print()
+List available commands with "help" or detailed help with "help cmd".
+⁰
+def do_toggle_unrecognized_command_behavior(self, arg: str): View Source
+128    def do_toggle_unrecognized_command_behavior(self, arg: str):
+129        """Toggle whether the shell will attempt to execute unrecognized
+commands as system commands in the terminal.
+130        When on (the default), `GitBetter` will treat unrecognized commands
+as if you added the `cmd` command in front of the input, i.e. `os.system
+(your_input)`.
+131        When off, an `unknown syntax` message will be printed and no
+commands will be executed."""
+132        self.execute_in_terminal_if_unrecognized = (
+133            not self.execute_in_terminal_if_unrecognized
+134        )
+135        print(self.unrecognized_command_behavior_status)
+Toggle whether the shell will attempt to execute unrecognized commands as
+system commands in the terminal. When on (the default), GitBetter will treat
+unrecognized commands as if you added the cmd command in front of the input,
+i.e. os.system(your_input). When off, an unknown syntax message will be printed
+and no commands will be executed.
+⁰
 def do_cd(self, path: str): View Source
-106    def do_cd(self, path: str):
-107        """Change current working directory to `path`."""
-108        os.chdir(path)
+137    def do_cd(self, path: str):
+138        """Change current working directory to `path`."""
+139        os.chdir(path)
+140        self.prompt = f"gitbetter::{Pathier.cwd()}>"
 Change current working directory to path.
 ⁰
-def do_cwd(self, _: str): View Source
-110    def do_cwd(self, _: str):
-111        """Print the current working directory."""
-112        print(Pathier.cwd())
-Print the current working directory.
-⁰
 def do_cmd(self, command: str): View Source
-114    def do_cmd(self, command: str):
-115        """Execute arbitrary command in the terminal so you don't have to
+142    def do_cmd(self, command: str):
+143        """Execute arbitrary command in the terminal so you don't have to
 quit gitbetter to run other programs/commands."""
-116        os.system(command)
+144        os.system(command)
 Execute arbitrary command in the terminal so you don't have to quit gitbetter
 to run other programs/commands.
 ⁰
 def do_git(self, arg: str): View Source
-118    def do_git(self, arg: str):
-119        """Directly execute `git {arg}`.
-120
-121        i.e. You can still do everything directly invoking git can do."""
-122        git.execute(arg)
+146    def do_git(self, arg: str):
+147        """Directly execute `git {arg}`.
+148
+149        i.e. You can still do everything directly invoking git can do."""
+150        git.execute(arg)
 Directly execute git {arg}.
 i.e. You can still do everything directly invoking git can do.
 ⁰
 def do_new_repo(self, _: str): View Source
-124    def do_new_repo(self, _: str):
-125        """Create a new git repo in this directory."""
-126        git.new_repo()
+152    def do_new_repo(self, _: str):
+153        """Create a new git repo in this directory."""
+154        git.new_repo()
 Create a new git repo in this directory.
 ⁰
 def do_new_branch(self, name: str): View Source
-128    def do_new_branch(self, name: str):
-129        """Create and switch to a new branch named after the supplied
+156    def do_new_branch(self, name: str):
+157        """Create and switch to a new branch named after the supplied
 arg."""
-130        git.create_new_branch(name)
+158        git.create_new_branch(name)
 Create and switch to a new branch named after the supplied arg.
 ⁰
 @with_parser(new_remote_parser)
 def do_new_gh_remote(self, args: argshell.argshell.Namespace): View Source
-132    @with_parser(new_remote_parser)
-133    def do_new_gh_remote(self, args: Namespace):
-134        """Create a remote GitHub repository for this repo.
-135
-136        GitHub CLI must be installed and configured for this to work."""
-137        name = Pathier.cwd().stem
-138        git.create_remote(name, args.public)
+160    @with_parser(new_remote_parser)
+161    def do_new_gh_remote(self, args: Namespace):
+162        """Create a remote GitHub repository for this repo.
+163
+164        GitHub CLI must be installed and configured for this to work."""
+165        name = Pathier.cwd().stem
+166        git.create_remote(name, args.public)
 Create a remote GitHub repository for this repo.
 GitHub CLI must be installed and configured for this to work.
 ⁰
 def do_initcommit(self, _: str): View Source
-140    def do_initcommit(self, _: str):
-141        """Stage and commit all files with message "Initial Commit"."""
-142        git.initcommit()
+168    def do_initcommit(self, _: str):
+169        """Stage and commit all files with message "Initial Commit"."""
+170        git.initcommit()
 Stage and commit all files with message "Initial Commit".
 ⁰
 def do_undo(self, _: str): View Source
-144    def do_undo(self, _: str):
-145        """Undo all uncommitted changes."""
-146        git.undo()
+172    def do_undo(self, _: str):
+173        """Undo all uncommitted changes."""
+174        git.undo()
 Undo all uncommitted changes.
 ⁰
 @with_parser(amend_files_parser, [files_postparser])
 def do_add(self, args: argshell.argshell.Namespace): View Source
-148    @with_parser(amend_files_parser, [files_postparser])
-149    def do_add(self, args: Namespace):
-150        """Stage a list of files.
-151        If no files are given, all files will be added."""
-152        git.add(None if not args.files else args.files)
+176    @with_parser(amend_files_parser, [files_postparser])
+177    def do_add(self, args: Namespace):
+178        """Stage a list of files.
+179        If no files are given, all files will be added."""
+180        git.add(None if not args.files else args.files)
 Stage a list of files. If no files are given, all files will be added.
 ⁰
 def do_commit(self, message: str): View Source
-154    def do_commit(self, message: str):
-155        """Commit staged files with this message."""
-156        if not message.startswith('"'):
-157            message = '"' + message
-158        if not message.endswith('"'):
-159            message += '"'
-160        git.commit(f"-m {message}")
+182    def do_commit(self, message: str):
+183        """Commit staged files with this message."""
+184        if not message.startswith('"'):
+185            message = '"' + message
+186        if not message.endswith('"'):
+187            message += '"'
+188        git.commit(f"-m {message}")
 Commit staged files with this message.
 ⁰
 @with_parser(commit_files_parser, [files_postparser])
 def do_commitf(self, args: argshell.argshell.Namespace): View Source
-162    @with_parser(commit_files_parser, [files_postparser])
-163    def do_commitf(self, args: Namespace):
-164        """Stage and commit a list of files."""
-165        git.commit_files(args.files, args.message)
+190    @with_parser(commit_files_parser, [files_postparser])
+191    def do_commitf(self, args: Namespace):
+192        """Stage and commit a list of files."""
+193        git.commit_files(args.files, args.message)
 Stage and commit a list of files.
 ⁰
 def do_commitall(self, message: str): View Source
-167    def do_commitall(self, message: str):
-168        """Stage and commit all files with this message."""
-169        if not message.startswith('"'):
-170            message = '"' + message
-171        if not message.endswith('"'):
-172            message += '"'
-173        git.add()
-174        git.commit(f"-m {message}")
+195    def do_commitall(self, message: str):
+196        """Stage and commit all files with this message."""
+197        if not message.startswith('"'):
+198            message = '"' + message
+199        if not message.endswith('"'):
+200            message += '"'
+201        git.add()
+202        git.commit(f"-m {message}")
 Stage and commit all files with this message.
 ⁰
 def do_switch(self, branch_name: str): View Source
-176    def do_switch(self, branch_name: str):
-177        """Switch to this branch."""
-178        git.switch_branch(branch_name)
+204    def do_switch(self, branch_name: str):
+205        """Switch to this branch."""
+206        git.switch_branch(branch_name)
 Switch to this branch.
 ⁰
 def do_add_url(self, url: str): View Source
-180    def do_add_url(self, url: str):
-181        """Add remote url for repo and push repo."""
-182        git.add_remote_url(url)
-183        git.push("-u origin main")
+208    def do_add_url(self, url: str):
+209        """Add remote url for repo and push repo."""
+210        git.add_remote_url(url)
+211        git.push("-u origin main")
 Add remote url for repo and push repo.
 ⁰
 def do_push_new(self, branch_name: str): View Source
-185    def do_push_new(self, branch_name: str):
-186        """Push this new branch to origin with -u flag."""
-187        git.push_new_branch(branch_name)
+213    def do_push_new(self, branch_name: str):
+214        """Push this new branch to origin with -u flag."""
+215        git.push_new_branch(branch_name)
 Push this new branch to origin with -u flag.
 ⁰
 def do_push(self, args: str): View Source
-189    def do_push(self, args: str):
-190        """Execute `git push`.
-191
-192        `args` can be any additional args that `git push` accepts."""
-193        git.push(args)
+217    def do_push(self, args: str):
+218        """Execute `git push`.
+219
+220        `args` can be any additional args that `git push` accepts."""
+221        git.push(args)
 Execute git push.
 args can be any additional args that git push accepts.
 ⁰
 def do_pull(self, args: str): View Source
-195    def do_pull(self, args: str):
-196        """Execute `git pull`.
-197
-198        `args` can be any additional args that `git pull` accepts."""
-199        git.pull(args)
+223    def do_pull(self, args: str):
+224        """Execute `git pull`.
+225
+226        `args` can be any additional args that `git pull` accepts."""
+227        git.pull(args)
 Execute git pull.
 args can be any additional args that git pull accepts.
 ⁰
 def do_list_branches(self, _: str): View Source
-201    def do_list_branches(self, _: str):
-202        """Show local and remote branches."""
-203        git.list_branches()
+229    def do_list_branches(self, _: str):
+230        """Show local and remote branches."""
+231        git.list_branches()
 Show local and remote branches.
 ⁰
 def do_loggy(self, _: str): View Source
-205    def do_loggy(self, _: str):
-206        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-207        git.loggy()
+233    def do_loggy(self, _: str):
+234        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+235        git.loggy()
 Execute git --oneline --name-only --abbrev-commit --graph.
 ⁰
 def do_merge(self, branch_name: str): View Source
-209    def do_merge(self, branch_name: str):
-210        """Merge supplied `branch_name` with the currently active branch."""
-211        git.merge(branch_name)
+237    def do_merge(self, branch_name: str):
+238        """Merge supplied `branch_name` with the currently active branch."""
+239        git.merge(branch_name)
 Merge supplied branch_name with the currently active branch.
 ⁰
 def do_tag(self, tag_id: str): View Source
-213    def do_tag(self, tag_id: str):
-214        """Tag current commit with `tag_id`."""
-215        git.tag(tag_id)
+241    def do_tag(self, tag_id: str):
+242        """Tag current commit with `tag_id`."""
+243        git.tag(tag_id)
 Tag current commit with tag_id.
 ⁰
 @with_parser(amend_files_parser, [files_postparser])
 def do_amend(self, args: argshell.argshell.Namespace): View Source
-217    @with_parser(amend_files_parser, [files_postparser])
-218    def do_amend(self, args: Namespace):
-219        """Stage files and add to previous commit."""
-220        git.amend(args.files)
+245    @with_parser(amend_files_parser, [files_postparser])
+246    def do_amend(self, args: Namespace):
+247        """Stage files and add to previous commit."""
+248        git.amend(args.files)
 Stage files and add to previous commit.
 ⁰
 @with_parser(delete_branch_parser)
 def do_delete_branch(self, args: argshell.argshell.Namespace): View Source
-222    @with_parser(delete_branch_parser)
-223    def do_delete_branch(self, args: Namespace):
-224        """Delete branch."""
-225        git.delete_branch(args.branch, not args.remote)
+250    @with_parser(delete_branch_parser)
+251    def do_delete_branch(self, args: Namespace):
+252        """Delete branch."""
+253        git.delete_branch(args.branch, not args.remote)
 Delete branch.
 ⁰
 def do_pull_branch(self, branch: str): View Source
-227    def do_pull_branch(self, branch: str):
-228        """Pull this branch from the origin."""
-229        git.pull_branch(branch)
+255    def do_pull_branch(self, branch: str):
+256        """Pull this branch from the origin."""
+257        git.pull_branch(branch)
 Pull this branch from the origin.
 ⁰
 def do_ignore(self, patterns: str): View Source
-231    def do_ignore(self, patterns: str):
-232        """Add the list of patterns to `.gitignore`."""
-233        patterns = "\n".join(patterns.split())
-234        path = Pathier(".gitignore")
-235        path.append("\n")
-236        path.append(patterns, False)
+259    def do_ignore(self, patterns: str):
+260        """Add the list of patterns to `.gitignore`."""
+261        patterns = "\n".join(patterns.split())
+262        path = Pathier(".gitignore")
+263        path.append("\n")
+264        path.append(patterns, False)
 Add the list of patterns to .gitignore.
 ⁰
 def do_make_private(self, owner: str): View Source
-238    def do_make_private(self, owner: str):
-239        """Make the GitHub remote for this repo private.
-240
-241        Expects an argument for the repo owner, i.e. the `OWNER` in
+266    def do_make_private(self, owner: str):
+267        """Make the GitHub remote for this repo private.
+268
+269        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-242
-243        This repo must exist and GitHub CLI must be installed and
+270
+271        This repo must exist and GitHub CLI must be installed and
 configured."""
-244        git.make_private(owner, Pathier.cwd().stem)
+272        git.make_private(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo private.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_make_public(self, owner: str): View Source
-246    def do_make_public(self, owner: str):
-247        """Make the GitHub remote for this repo public.
-248
-249        Expects an argument for the repo owner, i.e. the `OWNER` in
+274    def do_make_public(self, owner: str):
+275        """Make the GitHub remote for this repo public.
+276
+277        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-250
-251        This repo must exist and GitHub CLI must be installed and
+278
+279        This repo must exist and GitHub CLI must be installed and
 configured."""
-252        git.make_public(owner, Pathier.cwd().stem)
+280        git.make_public(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo public.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_delete_gh_repo(self, owner: str): View Source
-254    def do_delete_gh_repo(self, owner: str):
-255        """Delete this repo from GitHub.
-256
-257        Expects an argument for the repo owner, i.e. the `OWNER` in
+282    def do_delete_gh_repo(self, owner: str):
+283        """Delete this repo from GitHub.
+284
+285        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-258
-259        GitHub CLI must be installed and configured.
-260
-261        May require you to reauthorize and rerun command."""
-262        git.delete_remote(owner, Pathier.cwd().stem)
+286
+287        GitHub CLI must be installed and configured.
+288
+289        May require you to reauthorize and rerun command."""
+290        git.delete_remote(owner, Pathier.cwd().stem)
 Delete this repo from GitHub.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 GitHub CLI must be installed and configured.
 May require you to reauthorize and rerun command.
 ** Inherited Members **
   ⁰
 def main(): View Source
-265def main():
-266    GitBetter().cmdloop()
+293def main():
+294    GitBetter().cmdloop()
```

### Comparing `gitbetter-0.1.1/src/gitbetter/git.py` & `gitbetter-0.2.0/src/gitbetter/git.py`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.1/src/gitbetter/gitbetter.py` & `gitbetter-0.2.0/src/gitbetter/gitbetter.py`

 * *Files 26% similar despite different names*

```diff
@@ -96,23 +96,51 @@
     return args
 
 
 class GitBetter(ArgShell):
     """GitBetter Shell."""
 
     intro = "Starting gitbetter...\nEnter 'help' or '?' for command help."
-    prompt = "gitbetter>"
+    prompt = f"gitbetter::{Pathier.cwd()}>"
+    execute_in_terminal_if_unrecognized = True
+
+    def default(self, line: str):
+        if self.execute_in_terminal_if_unrecognized:
+            os.system(line)
+        else:
+            super().default(line)
+
+    def do_help(self, arg: str):
+        """List available commands with "help" or detailed help with "help cmd"."""
+        super().do_help(arg)
+        if not arg:
+            print(self.unrecognized_command_behavior_status)
+            if self.execute_in_terminal_if_unrecognized:
+                print(
+                    "^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^"
+                )
+        print()
+
+    @property
+    def unrecognized_command_behavior_status(self):
+        return f"Unrecognized command behavior: {'Execute with os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown syntax error'}"
+
+    def do_toggle_unrecognized_command_behavior(self, arg: str):
+        """Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.
+        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `cmd` command in front of the input, i.e. `os.system(your_input)`.
+        When off, an `unknown syntax` message will be printed and no commands will be executed."""
+        self.execute_in_terminal_if_unrecognized = (
+            not self.execute_in_terminal_if_unrecognized
+        )
+        print(self.unrecognized_command_behavior_status)
 
     def do_cd(self, path: str):
         """Change current working directory to `path`."""
         os.chdir(path)
-
-    def do_cwd(self, _: str):
-        """Print the current working directory."""
-        print(Pathier.cwd())
+        self.prompt = f"gitbetter::{Pathier.cwd()}>"
 
     def do_cmd(self, command: str):
         """Execute arbitrary command in the terminal so you don't have to quit gitbetter to run other programs/commands."""
         os.system(command)
 
     def do_git(self, arg: str):
         """Directly execute `git {arg}`.
```

### Comparing `gitbetter-0.1.1/LICENSE.txt` & `gitbetter-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-0.1.1/pyproject.toml` & `gitbetter-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,66 +5,66 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e31 2e31 220d  rsion = "0.1.1".
+000000b0: 7273 696f 6e20 3d20 2230 2e32 2e30 220d  rsion = "0.2.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
-000000d0: 203d 2022 3e3d 332e 3922 0d0a 6465 7065   = ">=3.9"..depe
-000000e0: 6e64 656e 6369 6573 203d 205b 2261 7267  ndencies = ["arg
-000000f0: 7368 656c 6c22 2c20 2270 6174 6869 6572  shell", "pathier
-00000100: 222c 2022 7079 7465 7374 225d 0d0a 7265  ", "pytest"]..re
-00000110: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
-00000120: 6422 0d0a 6b65 7977 6f72 6473 203d 205b  d"..keywords = [
-00000130: 2267 6974 222c 2022 7368 656c 6c22 2c20  "git", "shell", 
-00000140: 2263 6c69 222c 2022 7465 726d 696e 616c  "cli", "terminal
-00000150: 222c 2022 636f 6d6d 6974 225d 0d0a 636c  ", "commit"]..cl
-00000160: 6173 7369 6669 6572 7320 3d20 5b0d 0a20  assifiers = [.. 
-00000170: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
-00000180: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000190: 6f6e 203a 3a20 3322 2c0d 0a20 2020 2022  on :: 3",..    "
-000001a0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000001b0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-000001c0: 6963 656e 7365 222c 0d0a 2020 2020 224f  icense",..    "O
-000001d0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000001e0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000001f0: 7422 2c0d 0a20 2020 205d 0d0a 0d0a 5b5b  t",..    ]....[[
-00000200: 7072 6f6a 6563 742e 6175 7468 6f72 735d  project.authors]
-00000210: 5d0d 0a6e 616d 6520 3d20 224d 6174 7420  ]..name = "Matt 
-00000220: 4d61 6e65 7322 0d0a 656d 6169 6c20 3d20  Manes"..email = 
-00000230: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
-00000240: 220d 0a0d 0a5b 7072 6f6a 6563 742e 7572  "....[project.ur
-00000250: 6c73 5d0d 0a22 486f 6d65 7061 6765 2220  ls].."Homepage" 
-00000260: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
-00000270: 622e 636f 6d2f 6d61 7474 2d6d 616e 6573  b.com/matt-manes
-00000280: 2f67 6974 6265 7474 6572 220d 0a22 446f  /gitbetter".."Do
-00000290: 6375 6d65 6e74 6174 696f 6e22 203d 2022  cumentation" = "
-000002a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000002b0: 6f6d 2f6d 6174 742d 6d61 6e65 732f 6769  om/matt-manes/gi
-000002c0: 7462 6574 7465 722f 7472 6565 2f6d 6169  tbetter/tree/mai
-000002d0: 6e2f 646f 6373 220d 0a22 536f 7572 6365  n/docs".."Source
-000002e0: 2063 6f64 6522 203d 2022 6874 7470 733a   code" = "https:
-000002f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
-00000300: 742d 6d61 6e65 732f 6769 7462 6574 7465  t-manes/gitbette
-00000310: 722f 7472 6565 2f6d 6169 6e2f 7372 632f  r/tree/main/src/
-00000320: 6769 7462 6574 7465 7222 0d0a 0d0a 5b74  gitbetter"....[t
-00000330: 6f6f 6c2e 7079 7465 7374 2e69 6e69 5f6f  ool.pytest.ini_o
-00000340: 7074 696f 6e73 5d0d 0a61 6464 6f70 7473  ptions]..addopts
-00000350: 203d 205b 0d0a 2020 2020 222d 2d69 6d70   = [..    "--imp
-00000360: 6f72 742d 6d6f 6465 3d69 6d70 6f72 746c  ort-mode=importl
-00000370: 6962 222c 0d0a 2020 2020 5d0d 0a70 7974  ib",..    ]..pyt
-00000380: 686f 6e70 6174 6820 3d20 2273 7263 220d  honpath = "src".
-00000390: 0a0d 0a5b 746f 6f6c 2e68 6174 6368 2e62  ...[tool.hatch.b
-000003a0: 7569 6c64 2e74 6172 6765 7473 2e73 6469  uild.targets.sdi
-000003b0: 7374 5d0d 0a65 7863 6c75 6465 203d 205b  st]..exclude = [
-000003c0: 0d0a 2020 2020 222e 636f 7665 7261 6765  ..    ".coverage
-000003d0: 222c 0d0a 2020 2020 222e 7079 7465 7374  ",..    ".pytest
-000003e0: 5f63 6163 6865 222c 0d0a 2020 2020 222e  _cache",..    ".
-000003f0: 7673 636f 6465 222c 0d0a 2020 2020 2274  vscode",..    "t
-00000400: 6573 7473 222c 0d0a 2020 2020 222e 6769  ests",..    ".gi
-00000410: 7469 676e 6f72 6522 0d0a 2020 2020 5d0d  tignore"..    ].
-00000420: 0a5b 7072 6f6a 6563 742e 7363 7269 7074  .[project.script
-00000430: 735d 0d0a 6769 7462 6574 7465 7220 3d20  s]..gitbetter = 
-00000440: 2267 6974 6265 7474 6572 2e67 6974 6265  "gitbetter.gitbe
-00000450: 7474 6572 3a6d 6169 6e22 0d0a            tter:main"..
+000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
+000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
+000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
+00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
+00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
+00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords = 
+00000130: 5b22 6769 7422 2c20 2273 6865 6c6c 222c  ["git", "shell",
+00000140: 2022 636c 6922 2c20 2274 6572 6d69 6e61   "cli", "termina
+00000150: 6c22 2c20 2263 6f6d 6d69 7422 5d0d 0a63  l", "commit"]..c
+00000160: 6c61 7373 6966 6965 7273 203d 205b 0d0a  lassifiers = [..
+00000170: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
+00000180: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000190: 686f 6e20 3a3a 2033 222c 0d0a 2020 2020  hon :: 3",..    
+000001a0: 224c 6963 656e 7365 203a 3a20 4f53 4920  "License :: OSI 
+000001b0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000001c0: 4c69 6365 6e73 6522 2c0d 0a20 2020 2022  License",..    "
+000001d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001e0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001f0: 6e74 222c 0d0a 2020 2020 5d0d 0a0d 0a5b  nt",..    ]....[
+00000200: 5b70 726f 6a65 6374 2e61 7574 686f 7273  [project.authors
+00000210: 5d5d 0d0a 6e61 6d65 203d 2022 4d61 7474  ]]..name = "Matt
+00000220: 204d 616e 6573 220d 0a65 6d61 696c 203d   Manes"..email =
+00000230: 2022 6d61 7474 6d61 6e65 7340 706d 2e6d   "mattmanes@pm.m
+00000240: 6522 0d0a 0d0a 5b70 726f 6a65 6374 2e75  e"....[project.u
+00000250: 726c 735d 0d0a 2248 6f6d 6570 6167 6522  rls].."Homepage"
+00000260: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+00000270: 7562 2e63 6f6d 2f6d 6174 742d 6d61 6e65  ub.com/matt-mane
+00000280: 732f 6769 7462 6574 7465 7222 0d0a 2244  s/gitbetter".."D
+00000290: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
+000002a0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000002b0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f67  com/matt-manes/g
+000002c0: 6974 6265 7474 6572 2f74 7265 652f 6d61  itbetter/tree/ma
+000002d0: 696e 2f64 6f63 7322 0d0a 2253 6f75 7263  in/docs".."Sourc
+000002e0: 6520 636f 6465 2220 3d20 2268 7474 7073  e code" = "https
+000002f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+00000300: 7474 2d6d 616e 6573 2f67 6974 6265 7474  tt-manes/gitbett
+00000310: 6572 2f74 7265 652f 6d61 696e 2f73 7263  er/tree/main/src
+00000320: 2f67 6974 6265 7474 6572 220d 0a0d 0a5b  /gitbetter"....[
+00000330: 746f 6f6c 2e70 7974 6573 742e 696e 695f  tool.pytest.ini_
+00000340: 6f70 7469 6f6e 735d 0d0a 6164 646f 7074  options]..addopt
+00000350: 7320 3d20 5b0d 0a20 2020 2022 2d2d 696d  s = [..    "--im
+00000360: 706f 7274 2d6d 6f64 653d 696d 706f 7274  port-mode=import
+00000370: 6c69 6222 2c0d 0a20 2020 205d 0d0a 7079  lib",..    ]..py
+00000380: 7468 6f6e 7061 7468 203d 2022 7372 6322  thonpath = "src"
+00000390: 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463 682e  ....[tool.hatch.
+000003a0: 6275 696c 642e 7461 7267 6574 732e 7364  build.targets.sd
+000003b0: 6973 745d 0d0a 6578 636c 7564 6520 3d20  ist]..exclude = 
+000003c0: 5b0d 0a20 2020 2022 2e63 6f76 6572 6167  [..    ".coverag
+000003d0: 6522 2c0d 0a20 2020 2022 2e70 7974 6573  e",..    ".pytes
+000003e0: 745f 6361 6368 6522 2c0d 0a20 2020 2022  t_cache",..    "
+000003f0: 2e76 7363 6f64 6522 2c0d 0a20 2020 2022  .vscode",..    "
+00000400: 7465 7374 7322 2c0d 0a20 2020 2022 2e67  tests",..    ".g
+00000410: 6974 6967 6e6f 7265 220d 0a20 2020 205d  itignore"..    ]
+00000420: 0d0a 5b70 726f 6a65 6374 2e73 6372 6970  ..[project.scrip
+00000430: 7473 5d0d 0a67 6974 6265 7474 6572 203d  ts]..gitbetter =
+00000440: 2022 6769 7462 6574 7465 722e 6769 7462   "gitbetter.gitb
+00000450: 6574 7465 723a 6d61 696e 220d 0a         etter:main"..
```

### Comparing `gitbetter-0.1.1/PKG-INFO` & `gitbetter-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,125 +1,120 @@
-Metadata-Version: 2.1
-Name: gitbetter
-Version: 0.1.1
-Summary: Custom git shell to type less and commit more.
-Project-URL: Homepage, https://github.com/matt-manes/gitbetter
-Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
-Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
-Author-email: Matt Manes <mattmanes@pm.me>
-License-File: LICENSE.txt
-Keywords: cli,commit,git,shell,terminal
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Requires-Dist: argshell
-Requires-Dist: pathier
-Requires-Dist: pytest
-Description-Content-Type: text/markdown
-
-# gitbetter
-
-Custom git shell to type less and commit more.
-
-## Installation
-
-Install with:
-
-<pre>
-pip install gitbetter
-</pre>
-
-## Usage
-Launch from a terminal by entering `gitbetter`.<br>
-Type `help` or `?` for a list of commands.<br>
-Type `help {command}` for detailed help with a specific command.<br>
-<pre>
->gitbetter
-Starting gitbetter...
-Enter 'help' or '?' for command help.
-gitbetter>help
-
-Documented commands (type help <topic>):
-========================================
-add      commitall       help           make_public    pull_branch  undo
-add_url  commitf         ignore         merge          push
-amend    cwd             initcommit     new_branch     push_new
-cd       delete_branch   list_branches  new_gh_remote  quit
-cmd      delete_gh_repo  loggy          new_repo       switch
-commit   git             make_private   pull           tag
-
-gitbetter>help commitf
-Stage and commit a list of files.
-Parser help for commitf:
-usage: gitbetter [-h] -m MESSAGE [-r] [files ...]
-
-positional arguments:
-  files                 List of files to stage and commit.
-
-options:
-  -h, --help            show this help message and exit
-  -m MESSAGE, --message MESSAGE
-                        The commit message to use.
-  -r, --recursive       If a file name is not found in the current working directory, search for it in subfolders. This avoids having to type paths to files in subfolders,
-                        but if you have multiple files in different subfolders with the same name that have changes they will all be staged and committed.
-gitbetter>help loggy
-Execute `git --oneline --name-only --abbrev-commit --graph`.
-gitbetter>loggy
-*   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
-|\
-| * b4478a3 feat: new print statement
-| | test.py
-* | eb89c2e docs: update readme
-|/
-|   README.md
-* fc6b7ac (origin/main) docs: update readme
-| README.md
-* 2a75c0c docs: added a comment
-| test.py
-* d22129a feat: new print statement
-| gitbetter_test.py
-* 1a002d7 chore: add items to ignore
-| .gitignore
-* 92cb7e7 Initial commit
-  .gitignore
-  LICENSE.txt
-  README.md
-  gitbetter_test.py
-  test.py
-  test.txt
-</pre>
-
-Bindings can be accessed programmatically:
-<pre>
->>> from gitbetter import git
->>> git.loggy()
-*   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
-|\
-| * b4478a3 feat: new print statement
-| | test.py
-* | eb89c2e docs: update readme
-|/
-|   README.md
-* fc6b7ac (origin/main) docs: update readme
-| README.md
-* 2a75c0c docs: added a comment
-| test.py
-* d22129a feat: new print statement
-| gitbetter_test.py
-* 1a002d7 chore: add items to ignore
-| .gitignore
-* 92cb7e7 Initial commit
-  .gitignore
-  LICENSE.txt
-  README.md
-  gitbetter_test.py
-  test.py
-  test.txt
->>> git.list_branches()
-* main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
-  remotes/origin/main fc6b7ac docs: update readme
-</pre>
-
-### Future Features
-* Redirect the output of git commands so the bindings return the output instead of only being able to print.
+# gitbetter
+
+Custom git shell. Type less, commit more.
+
+## Installation
+
+Install with:
+
+<pre>
+pip install gitbetter
+</pre>
+
+## Usage
+Launch from a terminal by entering `gitbetter`.<br>
+Type `help` or `?` for a list of commands.<br>
+Type `help {command}` for detailed help with a specific command.<br>
+By default, If you enter a command that isn't built into `gitbetter`, it will be executed directly with `os.system()`,
+allowing you to perform any command not defined by `gitbetter` that your shell supports without having to exit.<br>
+To toggle this behavior, run the `toggle_unrecognized_command_behavior` 
+(`gitbetter` uses `tab` for autocomplete, so you can type `"tog"`+`tab` instead of typing out the whole command name).<br>
+When toggled to off, an unrecognized syntax message will be printed if you type in a command `gitbetter` doesn't recognize.<br>
+The current state of this setting is printed at the bottom when running the `help` command.<br>
+You can still execute a command in the shell regardless of this setting with the `cmd` command.
+<pre>
+C:\gitbetter>gitbetter
+Starting gitbetter...
+Enter 'help' or '?' for command help.
+gitbetter::C:\gitbetter>help
+
+Documented commands (type help <topic>):
+========================================
+add        delete_branch   make_private   push
+add_url    delete_gh_repo  make_public    push_new
+amend      git             merge          quit
+cd         help            new_branch     switch
+cmd        ignore          new_gh_remote  tag
+commit     initcommit      new_repo       toggle_unrecognized_command_behavior
+commitall  list_branches   pull           undo
+commitf    loggy           pull_branch
+
+Unrecognized command behavior: Execute with os.system()
+^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^
+
+gitbetter::C:\gitbetter>help commitf
+Stage and commit a list of files.
+Parser help for commitf:
+usage: gitbetter [-h] -m MESSAGE [-r] [files ...]
+
+positional arguments:
+  files                 List of files to stage and commit.
+
+options:
+  -h, --help            show this help message and exit
+  -m MESSAGE, --message MESSAGE
+                        The commit message to use.
+  -r, --recursive       If a file name is not found in the current working directory, search for it in subfolders. This avoids having to type paths to files in subfolders,
+                        but if you have multiple files in different subfolders with the same name that have changes they will all be staged and committed.
+                        
+gitbetter::C:\gitbetter>help loggy
+Execute `git --oneline --name-only --abbrev-commit --graph`.
+
+gitbetter::C:\gitbetter>loggy
+*   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
+|\
+| * b4478a3 feat: new print statement
+| | test.py
+* | eb89c2e docs: update readme
+|/
+|   README.md
+* fc6b7ac (origin/main) docs: update readme
+| README.md
+* 2a75c0c docs: added a comment
+| test.py
+* d22129a feat: new print statement
+| gitbetter_test.py
+* 1a002d7 chore: add items to ignore
+| .gitignore
+* 92cb7e7 Initial commit
+  .gitignore
+  LICENSE.txt
+  README.md
+  gitbetter_test.py
+  test.py
+  test.txt
+</pre>
+
+Bindings can be accessed programmatically:
+<pre>
+>>> from gitbetter import git
+>>> git.loggy()
+*   3e780ec (HEAD -> main, tag: v1.0.0) Merge branch 'my-feature'
+|\
+| * b4478a3 feat: new print statement
+| | test.py
+* | eb89c2e docs: update readme
+|/
+|   README.md
+* fc6b7ac (origin/main) docs: update readme
+| README.md
+* 2a75c0c docs: added a comment
+| test.py
+* d22129a feat: new print statement
+| gitbetter_test.py
+* 1a002d7 chore: add items to ignore
+| .gitignore
+* 92cb7e7 Initial commit
+  .gitignore
+  LICENSE.txt
+  README.md
+  gitbetter_test.py
+  test.py
+  test.txt
+>>> git.list_branches()
+* main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
+  remotes/origin/main fc6b7ac docs: update readme
+</pre>
+
+### Future Features
+* Redirect the output of git commands so the bindings return the output instead of only being able to print.
 * Make pushing to remote after creating it smoother (make it so you don't manually have to add the url).
```

