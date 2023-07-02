# Comparing `tmp/gitbetter-2.1.0.tar.gz` & `tmp/gitbetter-2.1.1.tar.gz`

## Comparing `gitbetter-2.1.0.tar` & `gitbetter-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 gitbetter-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    34198 2020-02-02 00:00:00.000000 gitbetter-2.1.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-2.1.0/docs/index.html
--rw-r--r--   0        0        0   178505 2020-02-02 00:00:00.000000 gitbetter-2.1.0/docs/search.js
--rw-r--r--   0        0        0   592512 2020-02-02 00:00:00.000000 gitbetter-2.1.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   525542 2020-02-02 00:00:00.000000 gitbetter-2.1.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0    58253 2020-02-02 00:00:00.000000 gitbetter-2.1.0/docs/gitbetter/parsers.html
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-2.1.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0    19336 2020-02-02 00:00:00.000000 gitbetter-2.1.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    17352 2020-02-02 00:00:00.000000 gitbetter-2.1.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 gitbetter-2.1.0/src/gitbetter/parsers.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 gitbetter-2.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 gitbetter-2.1.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 gitbetter-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 gitbetter-2.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34198 2020-02-02 00:00:00.000000 gitbetter-2.1.1/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-2.1.1/docs/index.html
+-rw-r--r--   0        0        0   177413 2020-02-02 00:00:00.000000 gitbetter-2.1.1/docs/search.js
+-rw-r--r--   0        0        0   592512 2020-02-02 00:00:00.000000 gitbetter-2.1.1/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   520108 2020-02-02 00:00:00.000000 gitbetter-2.1.1/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0    51389 2020-02-02 00:00:00.000000 gitbetter-2.1.1/docs/gitbetter/parsers.html
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-2.1.1/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0    19336 2020-02-02 00:00:00.000000 gitbetter-2.1.1/src/gitbetter/git.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 gitbetter-2.1.1/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 gitbetter-2.1.1/src/gitbetter/parsers.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 gitbetter-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-2.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 gitbetter-2.1.1/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 gitbetter-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 gitbetter-2.1.1/PKG-INFO
```

### Comparing `gitbetter-2.1.0/CHANGELOG.md` & `gitbetter-2.1.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## v2.1.0 (2023-06-20)
+
+#### Performance improvements
+
+* do_ignore will commit the gitignore file after adding patterns
+#### Refactorings
+
+* sort class contents and remove unused import
+
 ## v2.0.1 (2023-06-18)
 
 #### Fixes
 
 * fix amend() calling wrong add function
 
 ## v2.0.0 (2023-06-13)
```

### Comparing `gitbetter-2.1.0/docs/gitbetter.html` & `gitbetter-2.1.1/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-2.1.0/docs/search.js` & `gitbetter-2.1.1/docs/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2166,22 +2166,14 @@
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_commitall",
         "kind": "function",
         "doc": "<p>Stage and commit all modified and untracked files with this message.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">add</span> <span class=\"o\">.</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">commit</span> <span class=\"o\">-</span><span class=\"n\">m</span> <span class=\"s2\">&quot;</span><span class=\"si\">{message}</span><span class=\"s2\">&quot;</span>\n</code></pre>\n</div>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">message</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.gitbetter.GitBetter.do_commitf",
-        "modulename": "gitbetter.gitbetter",
-        "qualname": "GitBetter.do_commitf",
-        "kind": "function",
-        "doc": "<p>Stage and commit a list of files.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
-        "funcdef": "def"
-    }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_delete_branch",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_delete_branch",
         "kind": "function",
         "doc": "<p>Delete branch.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
@@ -2291,22 +2283,14 @@
         "modulename": "gitbetter.parsers",
         "qualname": "new_remote_parser",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.parsers.commit_files_parser",
-        "modulename": "gitbetter.parsers",
-        "qualname": "commit_files_parser",
-        "kind": "function",
-        "doc": "<p></p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span>:</span></span>",
-        "funcdef": "def"
-    }, {
         "fullname": "gitbetter.parsers.add_files_parser",
         "modulename": "gitbetter.parsers",
         "qualname": "add_files_parser",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span>:</span></span>",
         "funcdef": "def"
```

### Comparing `gitbetter-2.1.0/docs/gitbetter/git.html` & `gitbetter-2.1.1/docs/gitbetter/git.html`

 * *Files identical despite different names*

### Comparing `gitbetter-2.1.0/docs/gitbetter/gitbetter.html` & `gitbetter-2.1.1/docs/gitbetter/gitbetter.html`

 * *Files 0% similar despite different names*

```diff
@@ -282,17 +282,14 @@
                         <li>
                                 <a class="function" href="#GitBetter.do_branches">do_branches</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_commitall">do_commitall</a>
                         </li>
                         <li>
-                                <a class="function" href="#GitBetter.do_commitf">do_commitf</a>
-                        </li>
-                        <li>
                                 <a class="function" href="#GitBetter.do_delete_branch">do_delete_branch</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_delete_gh_repo">do_delete_gh_repo</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_ignore">do_ignore</a>
@@ -798,90 +795,85 @@
 </span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all modified and untracked files with this message.</span>
 </span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
 </span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a><span class="sd">        &gt;&gt;&gt; git commit -m \&quot;{message}\&quot; &quot;&quot;&quot;</span>
 </span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a>        <span class="n">message</span> <span class="o">=</span> <span class="n">message</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">,</span> <span class="s2">&quot;&#39;&quot;</span><span class="p">)</span>
 </span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_all</span><span class="p">()</span>
 </span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a>
-</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">commit_files_parser</span><span class="p">)</span>
-</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a>
-</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a>
+</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
 </span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a>
-</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">()</span>
 </span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>
-</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>
-</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">()</span>
+</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns/file names to `.gitignore` and commit with the message `chore: add to gitignore`.&quot;&quot;&quot;</span>
+</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">ignore</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">([</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">],</span> <span class="s2">&quot;chore: add to gitignore&quot;</span><span class="p">)</span>
 </span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a>
-</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns/file names to `.gitignore` and commit with the message `chore: add to gitignore`.&quot;&quot;&quot;</span>
-</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">ignore</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">([</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">],</span> <span class="s2">&quot;chore: add to gitignore&quot;</span><span class="p">)</span>
+</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">add_files_parser</span><span class="p">)</span>
+</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a>
-</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">add_files_parser</span><span class="p">)</span>
-</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>
-</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git --oneline --name-only --abbrev-commit --graph&quot;&quot;&quot;</span>
-</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>
-</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a>
-</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">()</span>
-</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>
-</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a>
-</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">()</span>
-</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>
-</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch with this `name`.&quot;&quot;&quot;</span>
-</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a>
-</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a>
-</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>
-</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git --oneline --name-only --abbrev-commit --graph&quot;&quot;&quot;</span>
+</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>
+</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a>
+</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">()</span>
+</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a>
+</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a>
+</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">()</span>
+</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a>
+</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch with this `name`.&quot;&quot;&quot;</span>
+</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a>
+</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a>
+</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a>
+</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>
+</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>        <span class="sd">&quot;&quot;&quot;Push current branch to origin with `-u` flag.</span>
+</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a><span class="sd">        &gt;&gt;&gt; git push -u origin {this_branch}&quot;&quot;&quot;</span>
+</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">current_branch</span><span class="p">)</span>
 </span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a>
-</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>        <span class="sd">&quot;&quot;&quot;Push current branch to origin with `-u` flag.</span>
-</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a><span class="sd">        &gt;&gt;&gt; git push -u origin {this_branch}&quot;&quot;&quot;</span>
-</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">current_branch</span><span class="p">)</span>
+</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.</span>
+</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a><span class="sd">        &gt;&gt;&gt; git checkout .&quot;&quot;&quot;</span>
+</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>
-</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.</span>
-</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a><span class="sd">        &gt;&gt;&gt; git checkout .&quot;&quot;&quot;</span>
-</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>
+</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>
 </span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>
-</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>
-</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
-</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a>
-</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>
-</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="GitArgShell">
                             <input id="GitArgShell-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -1467,82 +1459,77 @@
 </span><span id="GitBetter-446"><a href="#GitBetter-446"><span class="linenos">446</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all modified and untracked files with this message.</span>
 </span><span id="GitBetter-447"><a href="#GitBetter-447"><span class="linenos">447</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
 </span><span id="GitBetter-448"><a href="#GitBetter-448"><span class="linenos">448</span></a><span class="sd">        &gt;&gt;&gt; git commit -m \&quot;{message}\&quot; &quot;&quot;&quot;</span>
 </span><span id="GitBetter-449"><a href="#GitBetter-449"><span class="linenos">449</span></a>        <span class="n">message</span> <span class="o">=</span> <span class="n">message</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">,</span> <span class="s2">&quot;&#39;&quot;</span><span class="p">)</span>
 </span><span id="GitBetter-450"><a href="#GitBetter-450"><span class="linenos">450</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">add_all</span><span class="p">()</span>
 </span><span id="GitBetter-451"><a href="#GitBetter-451"><span class="linenos">451</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="GitBetter-452"><a href="#GitBetter-452"><span class="linenos">452</span></a>
-</span><span id="GitBetter-453"><a href="#GitBetter-453"><span class="linenos">453</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">commit_files_parser</span><span class="p">)</span>
-</span><span id="GitBetter-454"><a href="#GitBetter-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-455"><a href="#GitBetter-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-456"><a href="#GitBetter-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="GitBetter-453"><a href="#GitBetter-453"><span class="linenos">453</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter-454"><a href="#GitBetter-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-455"><a href="#GitBetter-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-456"><a href="#GitBetter-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span><span id="GitBetter-457"><a href="#GitBetter-457"><span class="linenos">457</span></a>
-</span><span id="GitBetter-458"><a href="#GitBetter-458"><span class="linenos">458</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter-459"><a href="#GitBetter-459"><span class="linenos">459</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-460"><a href="#GitBetter-460"><span class="linenos">460</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-461"><a href="#GitBetter-461"><span class="linenos">461</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="GitBetter-458"><a href="#GitBetter-458"><span class="linenos">458</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter-459"><a href="#GitBetter-459"><span class="linenos">459</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter-460"><a href="#GitBetter-460"><span class="linenos">460</span></a>
+</span><span id="GitBetter-461"><a href="#GitBetter-461"><span class="linenos">461</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
 </span><span id="GitBetter-462"><a href="#GitBetter-462"><span class="linenos">462</span></a>
-</span><span id="GitBetter-463"><a href="#GitBetter-463"><span class="linenos">463</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter-464"><a href="#GitBetter-464"><span class="linenos">464</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter-463"><a href="#GitBetter-463"><span class="linenos">463</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-464"><a href="#GitBetter-464"><span class="linenos">464</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">()</span>
 </span><span id="GitBetter-465"><a href="#GitBetter-465"><span class="linenos">465</span></a>
-</span><span id="GitBetter-466"><a href="#GitBetter-466"><span class="linenos">466</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter-467"><a href="#GitBetter-467"><span class="linenos">467</span></a>
-</span><span id="GitBetter-468"><a href="#GitBetter-468"><span class="linenos">468</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-469"><a href="#GitBetter-469"><span class="linenos">469</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">()</span>
+</span><span id="GitBetter-466"><a href="#GitBetter-466"><span class="linenos">466</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-467"><a href="#GitBetter-467"><span class="linenos">467</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns/file names to `.gitignore` and commit with the message `chore: add to gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-468"><a href="#GitBetter-468"><span class="linenos">468</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">ignore</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter-469"><a href="#GitBetter-469"><span class="linenos">469</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">([</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">],</span> <span class="s2">&quot;chore: add to gitignore&quot;</span><span class="p">)</span>
 </span><span id="GitBetter-470"><a href="#GitBetter-470"><span class="linenos">470</span></a>
-</span><span id="GitBetter-471"><a href="#GitBetter-471"><span class="linenos">471</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-472"><a href="#GitBetter-472"><span class="linenos">472</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns/file names to `.gitignore` and commit with the message `chore: add to gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-473"><a href="#GitBetter-473"><span class="linenos">473</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">ignore</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter-474"><a href="#GitBetter-474"><span class="linenos">474</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">([</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">],</span> <span class="s2">&quot;chore: add to gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-471"><a href="#GitBetter-471"><span class="linenos">471</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">add_files_parser</span><span class="p">)</span>
+</span><span id="GitBetter-472"><a href="#GitBetter-472"><span class="linenos">472</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-473"><a href="#GitBetter-473"><span class="linenos">473</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-474"><a href="#GitBetter-474"><span class="linenos">474</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span><span id="GitBetter-475"><a href="#GitBetter-475"><span class="linenos">475</span></a>
-</span><span id="GitBetter-476"><a href="#GitBetter-476"><span class="linenos">476</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">add_files_parser</span><span class="p">)</span>
-</span><span id="GitBetter-477"><a href="#GitBetter-477"><span class="linenos">477</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-478"><a href="#GitBetter-478"><span class="linenos">478</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-479"><a href="#GitBetter-479"><span class="linenos">479</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-480"><a href="#GitBetter-480"><span class="linenos">480</span></a>
-</span><span id="GitBetter-481"><a href="#GitBetter-481"><span class="linenos">481</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-482"><a href="#GitBetter-482"><span class="linenos">482</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git --oneline --name-only --abbrev-commit --graph&quot;&quot;&quot;</span>
-</span><span id="GitBetter-483"><a href="#GitBetter-483"><span class="linenos">483</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="GitBetter-484"><a href="#GitBetter-484"><span class="linenos">484</span></a>
-</span><span id="GitBetter-485"><a href="#GitBetter-485"><span class="linenos">485</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter-486"><a href="#GitBetter-486"><span class="linenos">486</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter-487"><a href="#GitBetter-487"><span class="linenos">487</span></a>
-</span><span id="GitBetter-488"><a href="#GitBetter-488"><span class="linenos">488</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-489"><a href="#GitBetter-489"><span class="linenos">489</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">()</span>
-</span><span id="GitBetter-490"><a href="#GitBetter-490"><span class="linenos">490</span></a>
-</span><span id="GitBetter-491"><a href="#GitBetter-491"><span class="linenos">491</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter-492"><a href="#GitBetter-492"><span class="linenos">492</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter-493"><a href="#GitBetter-493"><span class="linenos">493</span></a>
-</span><span id="GitBetter-494"><a href="#GitBetter-494"><span class="linenos">494</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-495"><a href="#GitBetter-495"><span class="linenos">495</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">()</span>
-</span><span id="GitBetter-496"><a href="#GitBetter-496"><span class="linenos">496</span></a>
-</span><span id="GitBetter-497"><a href="#GitBetter-497"><span class="linenos">497</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-498"><a href="#GitBetter-498"><span class="linenos">498</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch with this `name`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-499"><a href="#GitBetter-499"><span class="linenos">499</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
-</span><span id="GitBetter-500"><a href="#GitBetter-500"><span class="linenos">500</span></a>
-</span><span id="GitBetter-501"><a href="#GitBetter-501"><span class="linenos">501</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter-502"><a href="#GitBetter-502"><span class="linenos">502</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-503"><a href="#GitBetter-503"><span class="linenos">503</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter-504"><a href="#GitBetter-504"><span class="linenos">504</span></a>
-</span><span id="GitBetter-505"><a href="#GitBetter-505"><span class="linenos">505</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-506"><a href="#GitBetter-506"><span class="linenos">506</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="GitBetter-507"><a href="#GitBetter-507"><span class="linenos">507</span></a>
-</span><span id="GitBetter-508"><a href="#GitBetter-508"><span class="linenos">508</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-509"><a href="#GitBetter-509"><span class="linenos">509</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-510"><a href="#GitBetter-510"><span class="linenos">510</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="GitBetter-476"><a href="#GitBetter-476"><span class="linenos">476</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-477"><a href="#GitBetter-477"><span class="linenos">477</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git --oneline --name-only --abbrev-commit --graph&quot;&quot;&quot;</span>
+</span><span id="GitBetter-478"><a href="#GitBetter-478"><span class="linenos">478</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="GitBetter-479"><a href="#GitBetter-479"><span class="linenos">479</span></a>
+</span><span id="GitBetter-480"><a href="#GitBetter-480"><span class="linenos">480</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter-481"><a href="#GitBetter-481"><span class="linenos">481</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter-482"><a href="#GitBetter-482"><span class="linenos">482</span></a>
+</span><span id="GitBetter-483"><a href="#GitBetter-483"><span class="linenos">483</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-484"><a href="#GitBetter-484"><span class="linenos">484</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">()</span>
+</span><span id="GitBetter-485"><a href="#GitBetter-485"><span class="linenos">485</span></a>
+</span><span id="GitBetter-486"><a href="#GitBetter-486"><span class="linenos">486</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter-487"><a href="#GitBetter-487"><span class="linenos">487</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter-488"><a href="#GitBetter-488"><span class="linenos">488</span></a>
+</span><span id="GitBetter-489"><a href="#GitBetter-489"><span class="linenos">489</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-490"><a href="#GitBetter-490"><span class="linenos">490</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">()</span>
+</span><span id="GitBetter-491"><a href="#GitBetter-491"><span class="linenos">491</span></a>
+</span><span id="GitBetter-492"><a href="#GitBetter-492"><span class="linenos">492</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-493"><a href="#GitBetter-493"><span class="linenos">493</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch with this `name`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-494"><a href="#GitBetter-494"><span class="linenos">494</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+</span><span id="GitBetter-495"><a href="#GitBetter-495"><span class="linenos">495</span></a>
+</span><span id="GitBetter-496"><a href="#GitBetter-496"><span class="linenos">496</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter-497"><a href="#GitBetter-497"><span class="linenos">497</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-498"><a href="#GitBetter-498"><span class="linenos">498</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter-499"><a href="#GitBetter-499"><span class="linenos">499</span></a>
+</span><span id="GitBetter-500"><a href="#GitBetter-500"><span class="linenos">500</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-501"><a href="#GitBetter-501"><span class="linenos">501</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="GitBetter-502"><a href="#GitBetter-502"><span class="linenos">502</span></a>
+</span><span id="GitBetter-503"><a href="#GitBetter-503"><span class="linenos">503</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-504"><a href="#GitBetter-504"><span class="linenos">504</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-505"><a href="#GitBetter-505"><span class="linenos">505</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+</span><span id="GitBetter-506"><a href="#GitBetter-506"><span class="linenos">506</span></a>
+</span><span id="GitBetter-507"><a href="#GitBetter-507"><span class="linenos">507</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-508"><a href="#GitBetter-508"><span class="linenos">508</span></a>        <span class="sd">&quot;&quot;&quot;Push current branch to origin with `-u` flag.</span>
+</span><span id="GitBetter-509"><a href="#GitBetter-509"><span class="linenos">509</span></a><span class="sd">        &gt;&gt;&gt; git push -u origin {this_branch}&quot;&quot;&quot;</span>
+</span><span id="GitBetter-510"><a href="#GitBetter-510"><span class="linenos">510</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">current_branch</span><span class="p">)</span>
 </span><span id="GitBetter-511"><a href="#GitBetter-511"><span class="linenos">511</span></a>
-</span><span id="GitBetter-512"><a href="#GitBetter-512"><span class="linenos">512</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-513"><a href="#GitBetter-513"><span class="linenos">513</span></a>        <span class="sd">&quot;&quot;&quot;Push current branch to origin with `-u` flag.</span>
-</span><span id="GitBetter-514"><a href="#GitBetter-514"><span class="linenos">514</span></a><span class="sd">        &gt;&gt;&gt; git push -u origin {this_branch}&quot;&quot;&quot;</span>
-</span><span id="GitBetter-515"><a href="#GitBetter-515"><span class="linenos">515</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">current_branch</span><span class="p">)</span>
-</span><span id="GitBetter-516"><a href="#GitBetter-516"><span class="linenos">516</span></a>
-</span><span id="GitBetter-517"><a href="#GitBetter-517"><span class="linenos">517</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-518"><a href="#GitBetter-518"><span class="linenos">518</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.</span>
-</span><span id="GitBetter-519"><a href="#GitBetter-519"><span class="linenos">519</span></a><span class="sd">        &gt;&gt;&gt; git checkout .&quot;&quot;&quot;</span>
-</span><span id="GitBetter-520"><a href="#GitBetter-520"><span class="linenos">520</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="GitBetter-512"><a href="#GitBetter-512"><span class="linenos">512</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-513"><a href="#GitBetter-513"><span class="linenos">513</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.</span>
+</span><span id="GitBetter-514"><a href="#GitBetter-514"><span class="linenos">514</span></a><span class="sd">        &gt;&gt;&gt; git checkout .&quot;&quot;&quot;</span>
+</span><span id="GitBetter-515"><a href="#GitBetter-515"><span class="linenos">515</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>GitBetter Shell.</p>
 </div>
 
 
@@ -3592,54 +3579,30 @@
 <span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">commit</span> <span class="o">-</span><span class="n">m</span> <span class="s2">&quot;</span><span class="si">{message}</span><span class="s2">&quot;</span>
 </code></pre>
 </div>
 </div>
 
 
                             </div>
-                            <div id="GitBetter.do_commitf" class="classattr">
-                                        <input id="GitBetter.do_commitf-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-                    <div class="decorator">@with_parser(parsers.commit_files_parser)</div>
-
-        <span class="def">def</span>
-        <span class="name">do_commitf</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
-
-                <label class="view-source-button" for="GitBetter.do_commitf-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#GitBetter.do_commitf"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-453"><a href="#GitBetter.do_commitf-453"><span class="linenos">453</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">commit_files_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_commitf-454"><a href="#GitBetter.do_commitf-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitf-455"><a href="#GitBetter.do_commitf-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitf-456"><a href="#GitBetter.do_commitf-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span></pre></div>
-
-
-            <div class="docstring"><p>Stage and commit a list of files.</p>
-</div>
-
-
-                            </div>
                             <div id="GitBetter.do_delete_branch" class="classattr">
                                         <input id="GitBetter.do_delete_branch-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
                     <div class="decorator">@with_parser(parsers.delete_branch_parser)</div>
 
         <span class="def">def</span>
         <span class="name">do_delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-458"><a href="#GitBetter.do_delete_branch-458"><span class="linenos">458</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_delete_branch-459"><a href="#GitBetter.do_delete_branch-459"><span class="linenos">459</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_branch-460"><a href="#GitBetter.do_delete_branch-460"><span class="linenos">460</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_branch-461"><a href="#GitBetter.do_delete_branch-461"><span class="linenos">461</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-453"><a href="#GitBetter.do_delete_branch-453"><span class="linenos">453</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_delete_branch-454"><a href="#GitBetter.do_delete_branch-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_branch-455"><a href="#GitBetter.do_delete_branch-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_branch-456"><a href="#GitBetter.do_delete_branch-456"><span class="linenos">456</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete branch.</p>
 </div>
 
 
@@ -3651,21 +3614,21 @@
         <span class="def">def</span>
         <span class="name">do_delete_gh_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_gh_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_gh_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-463"><a href="#GitBetter.do_delete_gh_repo-463"><span class="linenos">463</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_gh_repo-464"><a href="#GitBetter.do_delete_gh_repo-464"><span class="linenos">464</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter.do_delete_gh_repo-465"><a href="#GitBetter.do_delete_gh_repo-465"><span class="linenos">465</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-466"><a href="#GitBetter.do_delete_gh_repo-466"><span class="linenos">466</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter.do_delete_gh_repo-467"><a href="#GitBetter.do_delete_gh_repo-467"><span class="linenos">467</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-468"><a href="#GitBetter.do_delete_gh_repo-468"><span class="linenos">468</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_gh_repo-469"><a href="#GitBetter.do_delete_gh_repo-469"><span class="linenos">469</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-458"><a href="#GitBetter.do_delete_gh_repo-458"><span class="linenos">458</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_gh_repo-459"><a href="#GitBetter.do_delete_gh_repo-459"><span class="linenos">459</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter.do_delete_gh_repo-460"><a href="#GitBetter.do_delete_gh_repo-460"><span class="linenos">460</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-461"><a href="#GitBetter.do_delete_gh_repo-461"><span class="linenos">461</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter.do_delete_gh_repo-462"><a href="#GitBetter.do_delete_gh_repo-462"><span class="linenos">462</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-463"><a href="#GitBetter.do_delete_gh_repo-463"><span class="linenos">463</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_gh_repo-464"><a href="#GitBetter.do_delete_gh_repo-464"><span class="linenos">464</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete this repo from GitHub.</p>
 
 <p>GitHub CLI must be installed and configured.</p>
 
@@ -3681,18 +3644,18 @@
         <span class="def">def</span>
         <span class="name">do_ignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_ignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_ignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-471"><a href="#GitBetter.do_ignore-471"><span class="linenos">471</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_ignore-472"><a href="#GitBetter.do_ignore-472"><span class="linenos">472</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns/file names to `.gitignore` and commit with the message `chore: add to gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_ignore-473"><a href="#GitBetter.do_ignore-473"><span class="linenos">473</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">ignore</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter.do_ignore-474"><a href="#GitBetter.do_ignore-474"><span class="linenos">474</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">([</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">],</span> <span class="s2">&quot;chore: add to gitignore&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-466"><a href="#GitBetter.do_ignore-466"><span class="linenos">466</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_ignore-467"><a href="#GitBetter.do_ignore-467"><span class="linenos">467</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns/file names to `.gitignore` and commit with the message `chore: add to gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_ignore-468"><a href="#GitBetter.do_ignore-468"><span class="linenos">468</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">ignore</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter.do_ignore-469"><a href="#GitBetter.do_ignore-469"><span class="linenos">469</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">([</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">],</span> <span class="s2">&quot;chore: add to gitignore&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add the list of patterns/file names to <code>.gitignore</code> and commit with the message <code>chore: add to gitignore</code>.</p>
 </div>
 
 
@@ -3705,18 +3668,18 @@
         <span class="def">def</span>
         <span class="name">do_initcommit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-476"><a href="#GitBetter.do_initcommit-476"><span class="linenos">476</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">add_files_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_initcommit-477"><a href="#GitBetter.do_initcommit-477"><span class="linenos">477</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_initcommit-478"><a href="#GitBetter.do_initcommit-478"><span class="linenos">478</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_initcommit-479"><a href="#GitBetter.do_initcommit-479"><span class="linenos">479</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-471"><a href="#GitBetter.do_initcommit-471"><span class="linenos">471</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">add_files_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_initcommit-472"><a href="#GitBetter.do_initcommit-472"><span class="linenos">472</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_initcommit-473"><a href="#GitBetter.do_initcommit-473"><span class="linenos">473</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_initcommit-474"><a href="#GitBetter.do_initcommit-474"><span class="linenos">474</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with message "Initial Commit".</p>
 </div>
 
 
@@ -3728,17 +3691,17 @@
         <span class="def">def</span>
         <span class="name">do_loggy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_loggy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_loggy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-481"><a href="#GitBetter.do_loggy-481"><span class="linenos">481</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_loggy-482"><a href="#GitBetter.do_loggy-482"><span class="linenos">482</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git --oneline --name-only --abbrev-commit --graph&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_loggy-483"><a href="#GitBetter.do_loggy-483"><span class="linenos">483</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-476"><a href="#GitBetter.do_loggy-476"><span class="linenos">476</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_loggy-477"><a href="#GitBetter.do_loggy-477"><span class="linenos">477</span></a>        <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git --oneline --name-only --abbrev-commit --graph&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_loggy-478"><a href="#GitBetter.do_loggy-478"><span class="linenos">478</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="o">--</span><span class="n">oneline</span> <span class="o">--</span><span class="n">name</span><span class="o">-</span><span class="n">only</span> <span class="o">--</span><span class="n">abbrev</span><span class="o">-</span><span class="n">commit</span> <span class="o">--</span><span class="n">graph</span>
 </code></pre>
 </div>
@@ -3753,19 +3716,19 @@
         <span class="def">def</span>
         <span class="name">do_make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-485"><a href="#GitBetter.do_make_private-485"><span class="linenos">485</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_private-486"><a href="#GitBetter.do_make_private-486"><span class="linenos">486</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter.do_make_private-487"><a href="#GitBetter.do_make_private-487"><span class="linenos">487</span></a>
-</span><span id="GitBetter.do_make_private-488"><a href="#GitBetter.do_make_private-488"><span class="linenos">488</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_private-489"><a href="#GitBetter.do_make_private-489"><span class="linenos">489</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-480"><a href="#GitBetter.do_make_private-480"><span class="linenos">480</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_private-481"><a href="#GitBetter.do_make_private-481"><span class="linenos">481</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter.do_make_private-482"><a href="#GitBetter.do_make_private-482"><span class="linenos">482</span></a>
+</span><span id="GitBetter.do_make_private-483"><a href="#GitBetter.do_make_private-483"><span class="linenos">483</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_private-484"><a href="#GitBetter.do_make_private-484"><span class="linenos">484</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo private.</p>
 
 <p>This repo must exist and GitHub CLI must be installed and configured.</p>
 </div>
@@ -3779,19 +3742,19 @@
         <span class="def">def</span>
         <span class="name">do_make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-491"><a href="#GitBetter.do_make_public-491"><span class="linenos">491</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_public-492"><a href="#GitBetter.do_make_public-492"><span class="linenos">492</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter.do_make_public-493"><a href="#GitBetter.do_make_public-493"><span class="linenos">493</span></a>
-</span><span id="GitBetter.do_make_public-494"><a href="#GitBetter.do_make_public-494"><span class="linenos">494</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_public-495"><a href="#GitBetter.do_make_public-495"><span class="linenos">495</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-486"><a href="#GitBetter.do_make_public-486"><span class="linenos">486</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_public-487"><a href="#GitBetter.do_make_public-487"><span class="linenos">487</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter.do_make_public-488"><a href="#GitBetter.do_make_public-488"><span class="linenos">488</span></a>
+</span><span id="GitBetter.do_make_public-489"><a href="#GitBetter.do_make_public-489"><span class="linenos">489</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_public-490"><a href="#GitBetter.do_make_public-490"><span class="linenos">490</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo public.</p>
 
 <p>This repo must exist and GitHub CLI must be installed and configured.</p>
 </div>
@@ -3805,17 +3768,17 @@
         <span class="def">def</span>
         <span class="name">do_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-497"><a href="#GitBetter.do_new_branch-497"><span class="linenos">497</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_branch-498"><a href="#GitBetter.do_new_branch-498"><span class="linenos">498</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch with this `name`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_branch-499"><a href="#GitBetter.do_new_branch-499"><span class="linenos">499</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_branch-492"><a href="#GitBetter.do_new_branch-492"><span class="linenos">492</span></a>    <span class="k">def</span> <span class="nf">do_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_branch-493"><a href="#GitBetter.do_new_branch-493"><span class="linenos">493</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch with this `name`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_branch-494"><a href="#GitBetter.do_new_branch-494"><span class="linenos">494</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch with this <code>name</code>.</p>
 </div>
 
 
@@ -3828,20 +3791,20 @@
         <span class="def">def</span>
         <span class="name">do_new_gh_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_gh_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_gh_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-501"><a href="#GitBetter.do_new_gh_remote-501"><span class="linenos">501</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">new_remote_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_new_gh_remote-502"><a href="#GitBetter.do_new_gh_remote-502"><span class="linenos">502</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_gh_remote-503"><a href="#GitBetter.do_new_gh_remote-503"><span class="linenos">503</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
-</span><span id="GitBetter.do_new_gh_remote-504"><a href="#GitBetter.do_new_gh_remote-504"><span class="linenos">504</span></a>
-</span><span id="GitBetter.do_new_gh_remote-505"><a href="#GitBetter.do_new_gh_remote-505"><span class="linenos">505</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_gh_remote-506"><a href="#GitBetter.do_new_gh_remote-506"><span class="linenos">506</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-496"><a href="#GitBetter.do_new_gh_remote-496"><span class="linenos">496</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">parsers</span><span class="o">.</span><span class="n">new_remote_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_new_gh_remote-497"><a href="#GitBetter.do_new_gh_remote-497"><span class="linenos">497</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_gh_remote-498"><a href="#GitBetter.do_new_gh_remote-498"><span class="linenos">498</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
+</span><span id="GitBetter.do_new_gh_remote-499"><a href="#GitBetter.do_new_gh_remote-499"><span class="linenos">499</span></a>
+</span><span id="GitBetter.do_new_gh_remote-500"><a href="#GitBetter.do_new_gh_remote-500"><span class="linenos">500</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_gh_remote-501"><a href="#GitBetter.do_new_gh_remote-501"><span class="linenos">501</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a remote GitHub repository for this repo.</p>
 
 <p>GitHub CLI must be installed and configured for this to work.</p>
 </div>
@@ -3855,17 +3818,17 @@
         <span class="def">def</span>
         <span class="name">do_new_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_new_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_new_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-508"><a href="#GitBetter.do_new_repo-508"><span class="linenos">508</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_new_repo-509"><a href="#GitBetter.do_new_repo-509"><span class="linenos">509</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_repo-510"><a href="#GitBetter.do_new_repo-510"><span class="linenos">510</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_repo-503"><a href="#GitBetter.do_new_repo-503"><span class="linenos">503</span></a>    <span class="k">def</span> <span class="nf">do_new_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_new_repo-504"><a href="#GitBetter.do_new_repo-504"><span class="linenos">504</span></a>        <span class="sd">&quot;&quot;&quot;Create a new git repo in this directory.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_new_repo-505"><a href="#GitBetter.do_new_repo-505"><span class="linenos">505</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">new_repo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a new git repo in this directory.</p>
 </div>
 
 
@@ -3877,18 +3840,18 @@
         <span class="def">def</span>
         <span class="name">do_push_new</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push_new-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push_new"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-512"><a href="#GitBetter.do_push_new-512"><span class="linenos">512</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push_new-513"><a href="#GitBetter.do_push_new-513"><span class="linenos">513</span></a>        <span class="sd">&quot;&quot;&quot;Push current branch to origin with `-u` flag.</span>
-</span><span id="GitBetter.do_push_new-514"><a href="#GitBetter.do_push_new-514"><span class="linenos">514</span></a><span class="sd">        &gt;&gt;&gt; git push -u origin {this_branch}&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push_new-515"><a href="#GitBetter.do_push_new-515"><span class="linenos">515</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">current_branch</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-507"><a href="#GitBetter.do_push_new-507"><span class="linenos">507</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push_new-508"><a href="#GitBetter.do_push_new-508"><span class="linenos">508</span></a>        <span class="sd">&quot;&quot;&quot;Push current branch to origin with `-u` flag.</span>
+</span><span id="GitBetter.do_push_new-509"><a href="#GitBetter.do_push_new-509"><span class="linenos">509</span></a><span class="sd">        &gt;&gt;&gt; git push -u origin {this_branch}&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push_new-510"><a href="#GitBetter.do_push_new-510"><span class="linenos">510</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">current_branch</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push current branch to origin with <code>-u</code> flag.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">push</span> <span class="o">-</span><span class="n">u</span> <span class="n">origin</span> <span class="p">{</span><span class="n">this_branch</span><span class="p">}</span>
@@ -3905,18 +3868,18 @@
         <span class="def">def</span>
         <span class="name">do_undo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-517"><a href="#GitBetter.do_undo-517"><span class="linenos">517</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_undo-518"><a href="#GitBetter.do_undo-518"><span class="linenos">518</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.</span>
-</span><span id="GitBetter.do_undo-519"><a href="#GitBetter.do_undo-519"><span class="linenos">519</span></a><span class="sd">        &gt;&gt;&gt; git checkout .&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_undo-520"><a href="#GitBetter.do_undo-520"><span class="linenos">520</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-512"><a href="#GitBetter.do_undo-512"><span class="linenos">512</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_undo-513"><a href="#GitBetter.do_undo-513"><span class="linenos">513</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.</span>
+</span><span id="GitBetter.do_undo-514"><a href="#GitBetter.do_undo-514"><span class="linenos">514</span></a><span class="sd">        &gt;&gt;&gt; git checkout .&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_undo-515"><a href="#GitBetter.do_undo-515"><span class="linenos">515</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo all uncommitted changes.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">checkout</span> <span class="o">.</span>
@@ -3963,16 +3926,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-523"><a href="#main-523"><span class="linenos">523</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-524"><a href="#main-524"><span class="linenos">524</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-518"><a href="#main-518"><span class="linenos">518</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-519"><a href="#main-519"><span class="linenos">519</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -83,15 +83,14 @@
           o do_version
           o do_whatchanged
           o do_worktree
           o do_add_url
           o do_amend
           o do_branches
           o do_commitall
-          o do_commitf
           o do_delete_branch
           o do_delete_gh_repo
           o do_ignore
           o do_initcommit
           o do_loggy
           o do_make_private
           o do_make_public
@@ -573,93 +572,88 @@
 message.
 446        >>> git add .
 447        >>> git commit -m \"{message}\" """
 448        message = message.strip('"').replace('"', "'")
 449        self.git.add_all()
 450        self.git.commit(f'-m "{message}"')
 451
-452    @with_parser(parsers.commit_files_parser)
-453    def do_commitf(self, args: Namespace):
-454        """Stage and commit a list of files."""
-455        self.git.commit_files(args.files, args.message)
+452    @with_parser(parsers.delete_branch_parser)
+453    def do_delete_branch(self, args: Namespace):
+454        """Delete branch."""
+455        self.git.delete_branch(args.branch, not args.remote)
 456
-457    @with_parser(parsers.delete_branch_parser)
-458    def do_delete_branch(self, args: Namespace):
-459        """Delete branch."""
-460        self.git.delete_branch(args.branch, not args.remote)
+457    def do_delete_gh_repo(self):
+458        """Delete this repo from GitHub.
+459
+460        GitHub CLI must be installed and configured.
 461
-462    def do_delete_gh_repo(self):
-463        """Delete this repo from GitHub.
+462        May require you to reauthorize and rerun command."""
+463        self.git.delete_remote()
 464
-465        GitHub CLI must be installed and configured.
-466
-467        May require you to reauthorize and rerun command."""
-468        self.git.delete_remote()
-469
-470    def do_ignore(self, patterns: str):
-471        """Add the list of patterns/file names to `.gitignore` and commit
+465    def do_ignore(self, patterns: str):
+466        """Add the list of patterns/file names to `.gitignore` and commit
 with the message `chore: add to gitignore`."""
-472        self.git.ignore(patterns.split())
-473        self.git.commit_files([".gitignore"], "chore: add to gitignore")
+467        self.git.ignore(patterns.split())
+468        self.git.commit_files([".gitignore"], "chore: add to gitignore")
+469
+470    @with_parser(parsers.add_files_parser)
+471    def do_initcommit(self, args: Namespace):
+472        """Stage and commit all files with message "Initial Commit"."""
+473        self.git.initcommit(args.files)
 474
-475    @with_parser(parsers.add_files_parser)
-476    def do_initcommit(self, args: Namespace):
-477        """Stage and commit all files with message "Initial Commit"."""
-478        self.git.initcommit(args.files)
-479
-480    def do_loggy(self, _: str):
-481        """>>> git --oneline --name-only --abbrev-commit --graph"""
-482        self.git.loggy()
-483
-484    def do_make_private(self):
-485        """Make the GitHub remote for this repo private.
-486
-487        This repo must exist and GitHub CLI must be installed and
+475    def do_loggy(self, _: str):
+476        """>>> git --oneline --name-only --abbrev-commit --graph"""
+477        self.git.loggy()
+478
+479    def do_make_private(self):
+480        """Make the GitHub remote for this repo private.
+481
+482        This repo must exist and GitHub CLI must be installed and
 configured."""
-488        self.git.make_private()
-489
-490    def do_make_public(self):
-491        """Make the GitHub remote for this repo public.
-492
-493        This repo must exist and GitHub CLI must be installed and
+483        self.git.make_private()
+484
+485    def do_make_public(self):
+486        """Make the GitHub remote for this repo public.
+487
+488        This repo must exist and GitHub CLI must be installed and
 configured."""
-494        self.git.make_public()
-495
-496    def do_new_branch(self, name: str):
-497        """Create and switch to a new branch with this `name`."""
-498        self.git.create_new_branch(name)
-499
-500    @with_parser(parsers.new_remote_parser)
-501    def do_new_gh_remote(self, args: Namespace):
-502        """Create a remote GitHub repository for this repo.
-503
-504        GitHub CLI must be installed and configured for this to work."""
-505        self.git.create_remote_from_cwd(args.public)
-506
-507    def do_new_repo(self, _: str):
-508        """Create a new git repo in this directory."""
-509        self.git.new_repo()
+489        self.git.make_public()
+490
+491    def do_new_branch(self, name: str):
+492        """Create and switch to a new branch with this `name`."""
+493        self.git.create_new_branch(name)
+494
+495    @with_parser(parsers.new_remote_parser)
+496    def do_new_gh_remote(self, args: Namespace):
+497        """Create a remote GitHub repository for this repo.
+498
+499        GitHub CLI must be installed and configured for this to work."""
+500        self.git.create_remote_from_cwd(args.public)
+501
+502    def do_new_repo(self, _: str):
+503        """Create a new git repo in this directory."""
+504        self.git.new_repo()
+505
+506    def do_push_new(self, _: str):
+507        """Push current branch to origin with `-u` flag.
+508        >>> git push -u origin {this_branch}"""
+509        self.git.push_new_branch(self.git.current_branch)
 510
-511    def do_push_new(self, _: str):
-512        """Push current branch to origin with `-u` flag.
-513        >>> git push -u origin {this_branch}"""
-514        self.git.push_new_branch(self.git.current_branch)
+511    def do_undo(self, _: str):
+512        """Undo all uncommitted changes.
+513        >>> git checkout ."""
+514        self.git.undo()
 515
-516    def do_undo(self, _: str):
-517        """Undo all uncommitted changes.
-518        >>> git checkout ."""
-519        self.git.undo()
+516
+517def main():
+518    GitBetter().cmdloop()
+519
 520
-521
-522def main():
-523    GitBetter().cmdloop()
-524
-525
-526if __name__ == "__main__":
-527    main()
+521if __name__ == "__main__":
+522    main()
   ⁰
 class GitArgShell(argshell.argshell.ArgShell): View Source
 10class GitArgShell(ArgShell):
 11    git_header = "Built in Git commands (type '{command} -h' or '{command} --
 help'):"
 12    convenience_header = "Convenience commands (type 'help {command}'):"
 13
@@ -1202,85 +1196,80 @@
 message.
 447        >>> git add .
 448        >>> git commit -m \"{message}\" """
 449        message = message.strip('"').replace('"', "'")
 450        self.git.add_all()
 451        self.git.commit(f'-m "{message}"')
 452
-453    @with_parser(parsers.commit_files_parser)
-454    def do_commitf(self, args: Namespace):
-455        """Stage and commit a list of files."""
-456        self.git.commit_files(args.files, args.message)
+453    @with_parser(parsers.delete_branch_parser)
+454    def do_delete_branch(self, args: Namespace):
+455        """Delete branch."""
+456        self.git.delete_branch(args.branch, not args.remote)
 457
-458    @with_parser(parsers.delete_branch_parser)
-459    def do_delete_branch(self, args: Namespace):
-460        """Delete branch."""
-461        self.git.delete_branch(args.branch, not args.remote)
+458    def do_delete_gh_repo(self):
+459        """Delete this repo from GitHub.
+460
+461        GitHub CLI must be installed and configured.
 462
-463    def do_delete_gh_repo(self):
-464        """Delete this repo from GitHub.
+463        May require you to reauthorize and rerun command."""
+464        self.git.delete_remote()
 465
-466        GitHub CLI must be installed and configured.
-467
-468        May require you to reauthorize and rerun command."""
-469        self.git.delete_remote()
-470
-471    def do_ignore(self, patterns: str):
-472        """Add the list of patterns/file names to `.gitignore` and commit
+466    def do_ignore(self, patterns: str):
+467        """Add the list of patterns/file names to `.gitignore` and commit
 with the message `chore: add to gitignore`."""
-473        self.git.ignore(patterns.split())
-474        self.git.commit_files([".gitignore"], "chore: add to gitignore")
+468        self.git.ignore(patterns.split())
+469        self.git.commit_files([".gitignore"], "chore: add to gitignore")
+470
+471    @with_parser(parsers.add_files_parser)
+472    def do_initcommit(self, args: Namespace):
+473        """Stage and commit all files with message "Initial Commit"."""
+474        self.git.initcommit(args.files)
 475
-476    @with_parser(parsers.add_files_parser)
-477    def do_initcommit(self, args: Namespace):
-478        """Stage and commit all files with message "Initial Commit"."""
-479        self.git.initcommit(args.files)
-480
-481    def do_loggy(self, _: str):
-482        """>>> git --oneline --name-only --abbrev-commit --graph"""
-483        self.git.loggy()
-484
-485    def do_make_private(self):
-486        """Make the GitHub remote for this repo private.
-487
-488        This repo must exist and GitHub CLI must be installed and
+476    def do_loggy(self, _: str):
+477        """>>> git --oneline --name-only --abbrev-commit --graph"""
+478        self.git.loggy()
+479
+480    def do_make_private(self):
+481        """Make the GitHub remote for this repo private.
+482
+483        This repo must exist and GitHub CLI must be installed and
 configured."""
-489        self.git.make_private()
-490
-491    def do_make_public(self):
-492        """Make the GitHub remote for this repo public.
-493
-494        This repo must exist and GitHub CLI must be installed and
+484        self.git.make_private()
+485
+486    def do_make_public(self):
+487        """Make the GitHub remote for this repo public.
+488
+489        This repo must exist and GitHub CLI must be installed and
 configured."""
-495        self.git.make_public()
-496
-497    def do_new_branch(self, name: str):
-498        """Create and switch to a new branch with this `name`."""
-499        self.git.create_new_branch(name)
-500
-501    @with_parser(parsers.new_remote_parser)
-502    def do_new_gh_remote(self, args: Namespace):
-503        """Create a remote GitHub repository for this repo.
-504
-505        GitHub CLI must be installed and configured for this to work."""
-506        self.git.create_remote_from_cwd(args.public)
-507
-508    def do_new_repo(self, _: str):
-509        """Create a new git repo in this directory."""
-510        self.git.new_repo()
+490        self.git.make_public()
+491
+492    def do_new_branch(self, name: str):
+493        """Create and switch to a new branch with this `name`."""
+494        self.git.create_new_branch(name)
+495
+496    @with_parser(parsers.new_remote_parser)
+497    def do_new_gh_remote(self, args: Namespace):
+498        """Create a remote GitHub repository for this repo.
+499
+500        GitHub CLI must be installed and configured for this to work."""
+501        self.git.create_remote_from_cwd(args.public)
+502
+503    def do_new_repo(self, _: str):
+504        """Create a new git repo in this directory."""
+505        self.git.new_repo()
+506
+507    def do_push_new(self, _: str):
+508        """Push current branch to origin with `-u` flag.
+509        >>> git push -u origin {this_branch}"""
+510        self.git.push_new_branch(self.git.current_branch)
 511
-512    def do_push_new(self, _: str):
-513        """Push current branch to origin with `-u` flag.
-514        >>> git push -u origin {this_branch}"""
-515        self.git.push_new_branch(self.git.current_branch)
-516
-517    def do_undo(self, _: str):
-518        """Undo all uncommitted changes.
-519        >>> git checkout ."""
-520        self.git.undo()
+512    def do_undo(self, _: str):
+513        """Undo all uncommitted changes.
+514        >>> git checkout ."""
+515        self.git.undo()
 GitBetter Shell.
 ⁰
 def default(self, line: str): View Source
 _96    def default(self, line: str):
 _97        if self.execute_in_terminal_if_unrecognized:
 _98            os.system(line)
 _99        else:
@@ -1807,122 +1796,114 @@
 449        message = message.strip('"').replace('"', "'")
 450        self.git.add_all()
 451        self.git.commit(f'-m "{message}"')
 Stage and commit all modified and untracked files with this message.
 >>> git add .
 >>> git commit -m "{message}"
 ⁰
-@with_parser(parsers.commit_files_parser)
-def do_commitf(self, args: argshell.argshell.Namespace): View Source
-453    @with_parser(parsers.commit_files_parser)
-454    def do_commitf(self, args: Namespace):
-455        """Stage and commit a list of files."""
-456        self.git.commit_files(args.files, args.message)
-Stage and commit a list of files.
-⁰
 @with_parser(parsers.delete_branch_parser)
 def do_delete_branch(self, args: argshell.argshell.Namespace): View Source
-458    @with_parser(parsers.delete_branch_parser)
-459    def do_delete_branch(self, args: Namespace):
-460        """Delete branch."""
-461        self.git.delete_branch(args.branch, not args.remote)
+453    @with_parser(parsers.delete_branch_parser)
+454    def do_delete_branch(self, args: Namespace):
+455        """Delete branch."""
+456        self.git.delete_branch(args.branch, not args.remote)
 Delete branch.
 ⁰
 def do_delete_gh_repo(self): View Source
-463    def do_delete_gh_repo(self):
-464        """Delete this repo from GitHub.
-465
-466        GitHub CLI must be installed and configured.
-467
-468        May require you to reauthorize and rerun command."""
-469        self.git.delete_remote()
+458    def do_delete_gh_repo(self):
+459        """Delete this repo from GitHub.
+460
+461        GitHub CLI must be installed and configured.
+462
+463        May require you to reauthorize and rerun command."""
+464        self.git.delete_remote()
 Delete this repo from GitHub.
 GitHub CLI must be installed and configured.
 May require you to reauthorize and rerun command.
 ⁰
 def do_ignore(self, patterns: str): View Source
-471    def do_ignore(self, patterns: str):
-472        """Add the list of patterns/file names to `.gitignore` and commit
+466    def do_ignore(self, patterns: str):
+467        """Add the list of patterns/file names to `.gitignore` and commit
 with the message `chore: add to gitignore`."""
-473        self.git.ignore(patterns.split())
-474        self.git.commit_files([".gitignore"], "chore: add to gitignore")
+468        self.git.ignore(patterns.split())
+469        self.git.commit_files([".gitignore"], "chore: add to gitignore")
 Add the list of patterns/file names to .gitignore and commit with the message
 chore: add to gitignore.
 ⁰
 @with_parser(parsers.add_files_parser)
 def do_initcommit(self, args: argshell.argshell.Namespace): View Source
-476    @with_parser(parsers.add_files_parser)
-477    def do_initcommit(self, args: Namespace):
-478        """Stage and commit all files with message "Initial Commit"."""
-479        self.git.initcommit(args.files)
+471    @with_parser(parsers.add_files_parser)
+472    def do_initcommit(self, args: Namespace):
+473        """Stage and commit all files with message "Initial Commit"."""
+474        self.git.initcommit(args.files)
 Stage and commit all files with message "Initial Commit".
 ⁰
 def do_loggy(self, _: str): View Source
-481    def do_loggy(self, _: str):
-482        """>>> git --oneline --name-only --abbrev-commit --graph"""
-483        self.git.loggy()
+476    def do_loggy(self, _: str):
+477        """>>> git --oneline --name-only --abbrev-commit --graph"""
+478        self.git.loggy()
 >>> git --oneline --name-only --abbrev-commit --graph
 ⁰
 def do_make_private(self): View Source
-485    def do_make_private(self):
-486        """Make the GitHub remote for this repo private.
-487
-488        This repo must exist and GitHub CLI must be installed and
+480    def do_make_private(self):
+481        """Make the GitHub remote for this repo private.
+482
+483        This repo must exist and GitHub CLI must be installed and
 configured."""
-489        self.git.make_private()
+484        self.git.make_private()
 Make the GitHub remote for this repo private.
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_make_public(self): View Source
-491    def do_make_public(self):
-492        """Make the GitHub remote for this repo public.
-493
-494        This repo must exist and GitHub CLI must be installed and
+486    def do_make_public(self):
+487        """Make the GitHub remote for this repo public.
+488
+489        This repo must exist and GitHub CLI must be installed and
 configured."""
-495        self.git.make_public()
+490        self.git.make_public()
 Make the GitHub remote for this repo public.
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_new_branch(self, name: str): View Source
-497    def do_new_branch(self, name: str):
-498        """Create and switch to a new branch with this `name`."""
-499        self.git.create_new_branch(name)
+492    def do_new_branch(self, name: str):
+493        """Create and switch to a new branch with this `name`."""
+494        self.git.create_new_branch(name)
 Create and switch to a new branch with this name.
 ⁰
 @with_parser(parsers.new_remote_parser)
 def do_new_gh_remote(self, args: argshell.argshell.Namespace): View Source
-501    @with_parser(parsers.new_remote_parser)
-502    def do_new_gh_remote(self, args: Namespace):
-503        """Create a remote GitHub repository for this repo.
-504
-505        GitHub CLI must be installed and configured for this to work."""
-506        self.git.create_remote_from_cwd(args.public)
+496    @with_parser(parsers.new_remote_parser)
+497    def do_new_gh_remote(self, args: Namespace):
+498        """Create a remote GitHub repository for this repo.
+499
+500        GitHub CLI must be installed and configured for this to work."""
+501        self.git.create_remote_from_cwd(args.public)
 Create a remote GitHub repository for this repo.
 GitHub CLI must be installed and configured for this to work.
 ⁰
 def do_new_repo(self, _: str): View Source
-508    def do_new_repo(self, _: str):
-509        """Create a new git repo in this directory."""
-510        self.git.new_repo()
+503    def do_new_repo(self, _: str):
+504        """Create a new git repo in this directory."""
+505        self.git.new_repo()
 Create a new git repo in this directory.
 ⁰
 def do_push_new(self, _: str): View Source
-512    def do_push_new(self, _: str):
-513        """Push current branch to origin with `-u` flag.
-514        >>> git push -u origin {this_branch}"""
-515        self.git.push_new_branch(self.git.current_branch)
+507    def do_push_new(self, _: str):
+508        """Push current branch to origin with `-u` flag.
+509        >>> git push -u origin {this_branch}"""
+510        self.git.push_new_branch(self.git.current_branch)
 Push current branch to origin with -u flag.
 >>> git push -u origin {this_branch}
 ⁰
 def do_undo(self, _: str): View Source
-517    def do_undo(self, _: str):
-518        """Undo all uncommitted changes.
-519        >>> git checkout ."""
-520        self.git.undo()
+512    def do_undo(self, _: str):
+513        """Undo all uncommitted changes.
+514        >>> git checkout ."""
+515        self.git.undo()
 Undo all uncommitted changes.
 >>> git checkout .
 ** Inherited Members **
   ⁰
 def main(): View Source
-523def main():
-524    GitBetter().cmdloop()
+518def main():
+519    GitBetter().cmdloop()
```

### Comparing `gitbetter-2.1.0/docs/gitbetter/parsers.html` & `gitbetter-2.1.1/docs/gitbetter/parsers.html`

 * *Files 18% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
                     <a class="function" href="#new_remote_parser">new_remote_parser</a>
             </li>
             <li>
-                    <a class="function" href="#commit_files_parser">commit_files_parser</a>
-            </li>
-            <li>
                     <a class="function" href="#add_files_parser">add_files_parser</a>
             </li>
             <li>
                     <a class="function" href="#delete_branch_parser">delete_branch_parser</a>
             </li>
     </ul>
 
@@ -72,55 +69,40 @@
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>        <span class="s2">&quot;--public&quot;</span><span class="p">,</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Set the new remote visibility as public. Defaults to private. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="p">)</span>
 </span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
 </span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>
-</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">commit_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">add_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
 </span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. &quot;&quot;&quot;</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>    <span class="p">)</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>        <span class="s2">&quot;-m&quot;</span><span class="p">,</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>        <span class="s2">&quot;--message&quot;</span><span class="p">,</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>        <span class="n">required</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The commit message to use. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="p">)</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>    <span class="k">return</span> <span class="n">parser</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a><span class="k">def</span> <span class="nf">add_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. </span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a><span class="s2">        If not given, all files will be added.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. </span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a><span class="s2">        If not given, all files will be added.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>    <span class="p">)</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>    <span class="k">return</span> <span class="n">parser</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>
+</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="p">)</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="p">)</span>
 </span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="k">return</span> <span class="n">parser</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="p">)</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>    <span class="p">)</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
 
 
             </section>
                 <section id="new_remote_parser">
                             <input id="new_remote_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -142,66 +124,36 @@
 </span><span id="new_remote_parser-12"><a href="#new_remote_parser-12"><span class="linenos">12</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
 
 
     
 
                 </section>
-                <section id="commit_files_parser">
-                            <input id="commit_files_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">commit_files_parser</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShellParser</span>:</span></span>
-
-                <label class="view-source-button" for="commit_files_parser-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#commit_files_parser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="commit_files_parser-15"><a href="#commit_files_parser-15"><span class="linenos">15</span></a><span class="k">def</span> <span class="nf">commit_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="commit_files_parser-16"><a href="#commit_files_parser-16"><span class="linenos">16</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="commit_files_parser-17"><a href="#commit_files_parser-17"><span class="linenos">17</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="commit_files_parser-18"><a href="#commit_files_parser-18"><span class="linenos">18</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. &quot;&quot;&quot;</span>
-</span><span id="commit_files_parser-19"><a href="#commit_files_parser-19"><span class="linenos">19</span></a>    <span class="p">)</span>
-</span><span id="commit_files_parser-20"><a href="#commit_files_parser-20"><span class="linenos">20</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="commit_files_parser-21"><a href="#commit_files_parser-21"><span class="linenos">21</span></a>        <span class="s2">&quot;-m&quot;</span><span class="p">,</span>
-</span><span id="commit_files_parser-22"><a href="#commit_files_parser-22"><span class="linenos">22</span></a>        <span class="s2">&quot;--message&quot;</span><span class="p">,</span>
-</span><span id="commit_files_parser-23"><a href="#commit_files_parser-23"><span class="linenos">23</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="commit_files_parser-24"><a href="#commit_files_parser-24"><span class="linenos">24</span></a>        <span class="n">required</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="commit_files_parser-25"><a href="#commit_files_parser-25"><span class="linenos">25</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The commit message to use. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="commit_files_parser-26"><a href="#commit_files_parser-26"><span class="linenos">26</span></a>    <span class="p">)</span>
-</span><span id="commit_files_parser-27"><a href="#commit_files_parser-27"><span class="linenos">27</span></a>    <span class="k">return</span> <span class="n">parser</span>
-</span></pre></div>
-
-
-    
-
-                </section>
                 <section id="add_files_parser">
                             <input id="add_files_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">add_files_parser</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShellParser</span>:</span></span>
 
                 <label class="view-source-button" for="add_files_parser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#add_files_parser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="add_files_parser-30"><a href="#add_files_parser-30"><span class="linenos">30</span></a><span class="k">def</span> <span class="nf">add_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="add_files_parser-31"><a href="#add_files_parser-31"><span class="linenos">31</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="add_files_parser-32"><a href="#add_files_parser-32"><span class="linenos">32</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="add_files_parser-33"><a href="#add_files_parser-33"><span class="linenos">33</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span>
-</span><span id="add_files_parser-34"><a href="#add_files_parser-34"><span class="linenos">34</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="add_files_parser-35"><a href="#add_files_parser-35"><span class="linenos">35</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="add_files_parser-36"><a href="#add_files_parser-36"><span class="linenos">36</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="add_files_parser-37"><a href="#add_files_parser-37"><span class="linenos">37</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. </span>
-</span><span id="add_files_parser-38"><a href="#add_files_parser-38"><span class="linenos">38</span></a><span class="s2">        If not given, all files will be added.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="add_files_parser-39"><a href="#add_files_parser-39"><span class="linenos">39</span></a>    <span class="p">)</span>
-</span><span id="add_files_parser-40"><a href="#add_files_parser-40"><span class="linenos">40</span></a>    <span class="k">return</span> <span class="n">parser</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="add_files_parser-15"><a href="#add_files_parser-15"><span class="linenos">15</span></a><span class="k">def</span> <span class="nf">add_files_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="add_files_parser-16"><a href="#add_files_parser-16"><span class="linenos">16</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
+</span><span id="add_files_parser-17"><a href="#add_files_parser-17"><span class="linenos">17</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="add_files_parser-18"><a href="#add_files_parser-18"><span class="linenos">18</span></a>        <span class="s2">&quot;files&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-19"><a href="#add_files_parser-19"><span class="linenos">19</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="add_files_parser-20"><a href="#add_files_parser-20"><span class="linenos">20</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-21"><a href="#add_files_parser-21"><span class="linenos">21</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="add_files_parser-22"><a href="#add_files_parser-22"><span class="linenos">22</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; List of files to stage and commit. </span>
+</span><span id="add_files_parser-23"><a href="#add_files_parser-23"><span class="linenos">23</span></a><span class="s2">        If not given, all files will be added.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="add_files_parser-24"><a href="#add_files_parser-24"><span class="linenos">24</span></a>    <span class="p">)</span>
+</span><span id="add_files_parser-25"><a href="#add_files_parser-25"><span class="linenos">25</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
 
 
     
 
                 </section>
                 <section id="delete_branch_parser">
@@ -211,27 +163,27 @@
         <span class="def">def</span>
         <span class="name">delete_branch_parser</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShellParser</span>:</span></span>
 
                 <label class="view-source-button" for="delete_branch_parser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_branch_parser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch_parser-43"><a href="#delete_branch_parser-43"><span class="linenos">43</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
-</span><span id="delete_branch_parser-44"><a href="#delete_branch_parser-44"><span class="linenos">44</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
-</span><span id="delete_branch_parser-45"><a href="#delete_branch_parser-45"><span class="linenos">45</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="delete_branch_parser-46"><a href="#delete_branch_parser-46"><span class="linenos">46</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
-</span><span id="delete_branch_parser-47"><a href="#delete_branch_parser-47"><span class="linenos">47</span></a>    <span class="p">)</span>
-</span><span id="delete_branch_parser-48"><a href="#delete_branch_parser-48"><span class="linenos">48</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="delete_branch_parser-49"><a href="#delete_branch_parser-49"><span class="linenos">49</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-50"><a href="#delete_branch_parser-50"><span class="linenos">50</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-51"><a href="#delete_branch_parser-51"><span class="linenos">51</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-52"><a href="#delete_branch_parser-52"><span class="linenos">52</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
-</span><span id="delete_branch_parser-53"><a href="#delete_branch_parser-53"><span class="linenos">53</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="delete_branch_parser-54"><a href="#delete_branch_parser-54"><span class="linenos">54</span></a>    <span class="p">)</span>
-</span><span id="delete_branch_parser-55"><a href="#delete_branch_parser-55"><span class="linenos">55</span></a>    <span class="k">return</span> <span class="n">parser</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch_parser-28"><a href="#delete_branch_parser-28"><span class="linenos">28</span></a><span class="k">def</span> <span class="nf">delete_branch_parser</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">ArgShellParser</span><span class="p">:</span>
+</span><span id="delete_branch_parser-29"><a href="#delete_branch_parser-29"><span class="linenos">29</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">ArgShellParser</span><span class="p">()</span>
+</span><span id="delete_branch_parser-30"><a href="#delete_branch_parser-30"><span class="linenos">30</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="delete_branch_parser-31"><a href="#delete_branch_parser-31"><span class="linenos">31</span></a>        <span class="s2">&quot;branch&quot;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span> <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The name of the branch to delete. &quot;&quot;&quot;</span>
+</span><span id="delete_branch_parser-32"><a href="#delete_branch_parser-32"><span class="linenos">32</span></a>    <span class="p">)</span>
+</span><span id="delete_branch_parser-33"><a href="#delete_branch_parser-33"><span class="linenos">33</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="delete_branch_parser-34"><a href="#delete_branch_parser-34"><span class="linenos">34</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-35"><a href="#delete_branch_parser-35"><span class="linenos">35</span></a>        <span class="s2">&quot;--remote&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-36"><a href="#delete_branch_parser-36"><span class="linenos">36</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-37"><a href="#delete_branch_parser-37"><span class="linenos">37</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Delete the remote and remote-tracking branches along with the local branch.</span>
+</span><span id="delete_branch_parser-38"><a href="#delete_branch_parser-38"><span class="linenos">38</span></a><span class="s2">        By default only the local branch is deleted.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="delete_branch_parser-39"><a href="#delete_branch_parser-39"><span class="linenos">39</span></a>    <span class="p">)</span>
+</span><span id="delete_branch_parser-40"><a href="#delete_branch_parser-40"><span class="linenos">40</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
 
 
   ⁰
 ____ gitbetter [Unknown INPUT type]
 ***** API Documentation *****
     * new_remote_parser
-    * commit_files_parser
     * add_files_parser
     * delete_branch_parser
 built_with_pdoc[pdoc_logo]
 
 ****** gitbetter.parsers ******
 ⁰ View Source
 _1from argshell import ArgShellParser
@@ -21,107 +20,75 @@
 _8        action="store_true",
 _9        help=""" Set the new remote visibility as public. Defaults to
 private. """,
 10    )
 11    return parser
 12
 13
-14def commit_files_parser() -> ArgShellParser:
+14def add_files_parser() -> ArgShellParser:
 15    parser = ArgShellParser()
 16    parser.add_argument(
-17        "files", type=str, nargs="*", help=""" List of files to stage and
-commit. """
-18    )
-19    parser.add_argument(
-20        "-m",
-21        "--message",
-22        type=str,
-23        required=True,
-24        help=""" The commit message to use. """,
-25    )
-26    return parser
-27
-28
-29def add_files_parser() -> ArgShellParser:
-30    parser = ArgShellParser()
-31    parser.add_argument(
-32        "files",
-33        type=str,
-34        nargs="*",
-35        default=None,
-36        help=""" List of files to stage and commit.
-37        If not given, all files will be added.""",
+17        "files",
+18        type=str,
+19        nargs="*",
+20        default=None,
+21        help=""" List of files to stage and commit.
+22        If not given, all files will be added.""",
+23    )
+24    return parser
+25
+26
+27def delete_branch_parser() -> ArgShellParser:
+28    parser = ArgShellParser()
+29    parser.add_argument(
+30        "branch", type=str, help=""" The name of the branch to delete. """
+31    )
+32    parser.add_argument(
+33        "-r",
+34        "--remote",
+35        action="store_true",
+36        help=""" Delete the remote and remote-tracking branches along with
+the local branch.
+37        By default only the local branch is deleted.""",
 38    )
 39    return parser
-40
-41
-42def delete_branch_parser() -> ArgShellParser:
-43    parser = ArgShellParser()
-44    parser.add_argument(
-45        "branch", type=str, help=""" The name of the branch to delete. """
-46    )
-47    parser.add_argument(
-48        "-r",
-49        "--remote",
-50        action="store_true",
-51        help=""" Delete the remote and remote-tracking branches along with
-the local branch.
-52        By default only the local branch is deleted.""",
-53    )
-54    return parser
   ⁰
 def new_remote_parser() -> argshell.argshell.ArgShellParser: View Source
 _5def new_remote_parser() -> ArgShellParser:
 _6    parser = ArgShellParser()
 _7    parser.add_argument(
 _8        "--public",
 _9        action="store_true",
 10        help=""" Set the new remote visibility as public. Defaults to
 private. """,
 11    )
 12    return parser
   ⁰
-def commit_files_parser() -> argshell.argshell.ArgShellParser: View Source
-15def commit_files_parser() -> ArgShellParser:
+def add_files_parser() -> argshell.argshell.ArgShellParser: View Source
+15def add_files_parser() -> ArgShellParser:
 16    parser = ArgShellParser()
 17    parser.add_argument(
-18        "files", type=str, nargs="*", help=""" List of files to stage and
-commit. """
-19    )
-20    parser.add_argument(
-21        "-m",
-22        "--message",
-23        type=str,
-24        required=True,
-25        help=""" The commit message to use. """,
-26    )
-27    return parser
-  ⁰
-def add_files_parser() -> argshell.argshell.ArgShellParser: View Source
-30def add_files_parser() -> ArgShellParser:
-31    parser = ArgShellParser()
-32    parser.add_argument(
-33        "files",
-34        type=str,
-35        nargs="*",
-36        default=None,
-37        help=""" List of files to stage and commit.
-38        If not given, all files will be added.""",
-39    )
-40    return parser
+18        "files",
+19        type=str,
+20        nargs="*",
+21        default=None,
+22        help=""" List of files to stage and commit.
+23        If not given, all files will be added.""",
+24    )
+25    return parser
   ⁰
 def delete_branch_parser() -> argshell.argshell.ArgShellParser: View Source
-43def delete_branch_parser() -> ArgShellParser:
-44    parser = ArgShellParser()
-45    parser.add_argument(
-46        "branch", type=str, help=""" The name of the branch to delete. """
-47    )
-48    parser.add_argument(
-49        "-r",
-50        "--remote",
-51        action="store_true",
-52        help=""" Delete the remote and remote-tracking branches along with
+28def delete_branch_parser() -> ArgShellParser:
+29    parser = ArgShellParser()
+30    parser.add_argument(
+31        "branch", type=str, help=""" The name of the branch to delete. """
+32    )
+33    parser.add_argument(
+34        "-r",
+35        "--remote",
+36        action="store_true",
+37        help=""" Delete the remote and remote-tracking branches along with
 the local branch.
-53        By default only the local branch is deleted.""",
-54    )
-55    return parser
+38        By default only the local branch is deleted.""",
+39    )
+40    return parser
```

### Comparing `gitbetter-2.1.0/src/gitbetter/git.py` & `gitbetter-2.1.1/src/gitbetter/git.py`

 * *Files identical despite different names*

### Comparing `gitbetter-2.1.0/src/gitbetter/gitbetter.py` & `gitbetter-2.1.1/src/gitbetter/gitbetter.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,19 +445,14 @@
         """Stage and commit all modified and untracked files with this message.
         >>> git add .
         >>> git commit -m \"{message}\" """
         message = message.strip('"').replace('"', "'")
         self.git.add_all()
         self.git.commit(f'-m "{message}"')
 
-    @with_parser(parsers.commit_files_parser)
-    def do_commitf(self, args: Namespace):
-        """Stage and commit a list of files."""
-        self.git.commit_files(args.files, args.message)
-
     @with_parser(parsers.delete_branch_parser)
     def do_delete_branch(self, args: Namespace):
         """Delete branch."""
         self.git.delete_branch(args.branch, not args.remote)
 
     def do_delete_gh_repo(self):
         """Delete this repo from GitHub.
```

### Comparing `gitbetter-2.1.0/src/gitbetter/parsers.py` & `gitbetter-2.1.1/src/gitbetter/parsers.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,29 +7,14 @@
         "--public",
         action="store_true",
         help=""" Set the new remote visibility as public. Defaults to private. """,
     )
     return parser
 
 
-def commit_files_parser() -> ArgShellParser:
-    parser = ArgShellParser()
-    parser.add_argument(
-        "files", type=str, nargs="*", help=""" List of files to stage and commit. """
-    )
-    parser.add_argument(
-        "-m",
-        "--message",
-        type=str,
-        required=True,
-        help=""" The commit message to use. """,
-    )
-    return parser
-
-
 def add_files_parser() -> ArgShellParser:
     parser = ArgShellParser()
     parser.add_argument(
         "files",
         type=str,
         nargs="*",
         default=None,
```

### Comparing `gitbetter-2.1.0/LICENSE.txt` & `gitbetter-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-2.1.0/README.md` & `gitbetter-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gitbetter-2.1.0/pyproject.toml` & `gitbetter-2.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -5,66 +5,62 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2232 2e31 2e30 220d  rsion = "2.1.0".
+000000b0: 7273 696f 6e20 3d20 2232 2e31 2e31 220d  rsion = "2.1.1".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords = 
 00000130: 5b22 6769 7422 2c20 2273 6865 6c6c 222c  ["git", "shell",
 00000140: 2022 636c 6922 2c20 2274 6572 6d69 6e61   "cli", "termina
 00000150: 6c22 2c20 2263 6f6d 6d69 7422 5d0d 0a63  l", "commit"]..c
-00000160: 6c61 7373 6966 6965 7273 203d 205b 0d0a  lassifiers = [..
-00000170: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
-00000180: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000190: 686f 6e20 3a3a 2033 222c 0d0a 2020 2020  hon :: 3",..    
-000001a0: 224c 6963 656e 7365 203a 3a20 4f53 4920  "License :: OSI 
-000001b0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000001c0: 4c69 6365 6e73 6522 2c0d 0a20 2020 2022  License",..    "
-000001d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000001e0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000001f0: 6e74 222c 0d0a 2020 2020 5d0d 0a0d 0a5b  nt",..    ]....[
-00000200: 5b70 726f 6a65 6374 2e61 7574 686f 7273  [project.authors
-00000210: 5d5d 0d0a 6e61 6d65 203d 2022 4d61 7474  ]]..name = "Matt
-00000220: 204d 616e 6573 220d 0a65 6d61 696c 203d   Manes"..email =
-00000230: 2022 6d61 7474 6d61 6e65 7340 706d 2e6d   "mattmanes@pm.m
-00000240: 6522 0d0a 0d0a 5b70 726f 6a65 6374 2e75  e"....[project.u
-00000250: 726c 735d 0d0a 2248 6f6d 6570 6167 6522  rls].."Homepage"
-00000260: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-00000270: 7562 2e63 6f6d 2f6d 6174 742d 6d61 6e65  ub.com/matt-mane
-00000280: 732f 6769 7462 6574 7465 7222 0d0a 2244  s/gitbetter".."D
-00000290: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
-000002a0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000002b0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f67  com/matt-manes/g
-000002c0: 6974 6265 7474 6572 2f74 7265 652f 6d61  itbetter/tree/ma
-000002d0: 696e 2f64 6f63 7322 0d0a 2253 6f75 7263  in/docs".."Sourc
-000002e0: 6520 636f 6465 2220 3d20 2268 7474 7073  e code" = "https
-000002f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
-00000300: 7474 2d6d 616e 6573 2f67 6974 6265 7474  tt-manes/gitbett
-00000310: 6572 2f74 7265 652f 6d61 696e 2f73 7263  er/tree/main/src
-00000320: 2f67 6974 6265 7474 6572 220d 0a0d 0a5b  /gitbetter"....[
-00000330: 746f 6f6c 2e70 7974 6573 742e 696e 695f  tool.pytest.ini_
-00000340: 6f70 7469 6f6e 735d 0d0a 6164 646f 7074  options]..addopt
-00000350: 7320 3d20 5b0d 0a20 2020 2022 2d2d 696d  s = [..    "--im
-00000360: 706f 7274 2d6d 6f64 653d 696d 706f 7274  port-mode=import
-00000370: 6c69 6222 2c0d 0a20 2020 205d 0d0a 7079  lib",..    ]..py
-00000380: 7468 6f6e 7061 7468 203d 2022 7372 6322  thonpath = "src"
-00000390: 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463 682e  ....[tool.hatch.
-000003a0: 6275 696c 642e 7461 7267 6574 732e 7364  build.targets.sd
-000003b0: 6973 745d 0d0a 6578 636c 7564 6520 3d20  ist]..exclude = 
-000003c0: 5b0d 0a20 2020 2022 2e63 6f76 6572 6167  [..    ".coverag
-000003d0: 6522 2c0d 0a20 2020 2022 2e70 7974 6573  e",..    ".pytes
-000003e0: 745f 6361 6368 6522 2c0d 0a20 2020 2022  t_cache",..    "
-000003f0: 2e76 7363 6f64 6522 2c0d 0a20 2020 2022  .vscode",..    "
-00000400: 7465 7374 7322 2c0d 0a20 2020 2022 2e67  tests",..    ".g
-00000410: 6974 6967 6e6f 7265 220d 0a20 2020 205d  itignore"..    ]
-00000420: 0d0a 5b70 726f 6a65 6374 2e73 6372 6970  ..[project.scrip
-00000430: 7473 5d0d 0a67 6974 6265 7474 6572 203d  ts]..gitbetter =
-00000440: 2022 6769 7462 6574 7465 722e 6769 7462   "gitbetter.gitb
-00000450: 6574 7465 723a 6d61 696e 220d 0a         etter:main"..
+00000160: 6c61 7373 6966 6965 7273 203d 205b 2250  lassifiers = ["P
+00000170: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000180: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000190: 2033 222c 2022 4c69 6365 6e73 6520 3a3a   3", "License ::
+000001a0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001b0: 204d 4954 204c 6963 656e 7365 222c 2022   MIT License", "
+000001c0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001d0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001e0: 6e74 225d 0d0a 0d0a 5b5b 7072 6f6a 6563  nt"]....[[projec
+000001f0: 742e 6175 7468 6f72 735d 5d0d 0a6e 616d  t.authors]]..nam
+00000200: 6520 3d20 224d 6174 7420 4d61 6e65 7322  e = "Matt Manes"
+00000210: 0d0a 656d 6169 6c20 3d20 226d 6174 746d  ..email = "mattm
+00000220: 616e 6573 4070 6d2e 6d65 220d 0a0d 0a5b  anes@pm.me"....[
+00000230: 7072 6f6a 6563 742e 7572 6c73 5d0d 0a48  project.urls]..H
+00000240: 6f6d 6570 6167 6520 3d20 2268 7474 7073  omepage = "https
+00000250: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+00000260: 7474 2d6d 616e 6573 2f67 6974 6265 7474  tt-manes/gitbett
+00000270: 6572 220d 0a44 6f63 756d 656e 7461 7469  er"..Documentati
+00000280: 6f6e 203d 2022 6874 7470 733a 2f2f 6769  on = "https://gi
+00000290: 7468 7562 2e63 6f6d 2f6d 6174 742d 6d61  thub.com/matt-ma
+000002a0: 6e65 732f 6769 7462 6574 7465 722f 7472  nes/gitbetter/tr
+000002b0: 6565 2f6d 6169 6e2f 646f 6373 220d 0a22  ee/main/docs".."
+000002c0: 536f 7572 6365 2063 6f64 6522 203d 2022  Source code" = "
+000002d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002e0: 6f6d 2f6d 6174 742d 6d61 6e65 732f 6769  om/matt-manes/gi
+000002f0: 7462 6574 7465 722f 7472 6565 2f6d 6169  tbetter/tree/mai
+00000300: 6e2f 7372 632f 6769 7462 6574 7465 7222  n/src/gitbetter"
+00000310: 0d0a 0d0a 5b70 726f 6a65 6374 2e73 6372  ....[project.scr
+00000320: 6970 7473 5d0d 0a67 6974 6265 7474 6572  ipts]..gitbetter
+00000330: 203d 2022 6769 7462 6574 7465 722e 6769   = "gitbetter.gi
+00000340: 7462 6574 7465 723a 6d61 696e 220d 0a0d  tbetter:main"...
+00000350: 0a5b 746f 6f6c 5d0d 0a5b 746f 6f6c 2e70  .[tool]..[tool.p
+00000360: 7974 6573 742e 696e 695f 6f70 7469 6f6e  ytest.ini_option
+00000370: 735d 0d0a 6164 646f 7074 7320 3d20 5b22  s]..addopts = ["
+00000380: 2d2d 696d 706f 7274 2d6d 6f64 653d 696d  --import-mode=im
+00000390: 706f 7274 6c69 6222 5d0d 0a70 7974 686f  portlib"]..pytho
+000003a0: 6e70 6174 6820 3d20 2273 7263 220d 0a0d  npath = "src"...
+000003b0: 0a5b 746f 6f6c 2e68 6174 6368 2e62 7569  .[tool.hatch.bui
+000003c0: 6c64 2e74 6172 6765 7473 2e73 6469 7374  ld.targets.sdist
+000003d0: 5d0d 0a65 7863 6c75 6465 203d 205b 222e  ]..exclude = [".
+000003e0: 636f 7665 7261 6765 222c 2022 2e70 7974  coverage", ".pyt
+000003f0: 6573 745f 6361 6368 6522 2c20 222e 7673  est_cache", ".vs
+00000400: 636f 6465 222c 2022 7465 7374 7322 2c20  code", "tests", 
+00000410: 222e 6769 7469 676e 6f72 6522 5d0d 0a    ".gitignore"]..
```

### Comparing `gitbetter-2.1.0/PKG-INFO` & `gitbetter-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 2.1.0
+Version: 2.1.1
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
```

