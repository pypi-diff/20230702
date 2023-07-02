# Comparing `tmp/databased-2.4.1.tar.gz` & `tmp/databased-2.5.0.tar.gz`

## Comparing `databased-2.4.1.tar` & `databased-2.5.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 databased-2.4.1/CHANGELOG.md
--rw-r--r--   0        0        0    34933 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.4.1/docs/index.html
--rw-r--r--   0        0        0    67193 2020-02-02 00:00:00.000000 databased-2.4.1/docs/search.js
--rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/customshell.html
--rw-r--r--   0        0        0   428406 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/databased.html
--rw-r--r--   0        0        0   127330 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/dbparsers.html
--rw-r--r--   0        0        0   320438 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/dbshell.html
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/customshell.py
--rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/databased.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/dbparsers.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/dbshell.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.4.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.4.1/LICENSE.txt
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.4.1/README.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 databased-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 databased-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 databased-2.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35218 2020-02-02 00:00:00.000000 databased-2.5.0/docs/databased.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.5.0/docs/index.html
+-rw-r--r--   0        0        0    68951 2020-02-02 00:00:00.000000 databased-2.5.0/docs/search.js
+-rw-r--r--   0        0        0    55046 2020-02-02 00:00:00.000000 databased-2.5.0/docs/databased/create_shell.html
+-rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.5.0/docs/databased/customshell.html
+-rw-r--r--   0        0        0   431278 2020-02-02 00:00:00.000000 databased-2.5.0/docs/databased/databased.html
+-rw-r--r--   0        0        0   127330 2020-02-02 00:00:00.000000 databased-2.5.0/docs/databased/dbparsers.html
+-rw-r--r--   0        0        0   310103 2020-02-02 00:00:00.000000 databased-2.5.0/docs/databased/dbshell.html
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 databased-2.5.0/src/databased/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 databased-2.5.0/src/databased/create_shell.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.5.0/src/databased/customshell.py
+-rw-r--r--   0        0        0    22067 2020-02-02 00:00:00.000000 databased-2.5.0/src/databased/databased.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 databased-2.5.0/src/databased/dbparsers.py
+-rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 databased-2.5.0/src/databased/dbshell.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.5.0/README.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 databased-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 databased-2.5.0/PKG-INFO
```

### Comparing `databased-2.4.1/CHANGELOG.md` & `databased-2.5.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## v2.4.1 (2023-06-19)
+
+#### Fixes
+
+* only reprint number of matching rows in do_show if there are any
+#### Performance improvements
+
+* reprint number of results after grid in do_show
+#### Refactorings
+
+* change abbreviated flag in get_info_parser from '-rc' to '-c'
+
 ## v2.4.0 (2023-05-21)
 
 #### Refactorings
 
 * do_query() will attempt to use griddy to display results
 #### Others
```

### Comparing `databased-2.4.1/docs/databased.html` & `databased-2.5.0/docs/databased.html`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
             <input type="search" placeholder="Search..." role="searchbox" aria-label="search"
                    pattern=".+" required>
 
 
         <h2>Submodules</h2>
         <ul>
+                <li><a href="databased/create_shell.html">create_shell</a></li>
                 <li><a href="databased/customshell.html">customshell</a></li>
                 <li><a href="databased/databased.html">databased</a></li>
                 <li><a href="databased/dbparsers.html">dbparsers</a></li>
                 <li><a href="databased/dbshell.html">dbshell</a></li>
         </ul>
 
 
@@ -47,16 +48,17 @@
                 
                         <input id="mod-databased-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-databased-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">databased</span> <span class="kn">import</span> <span class="n">dbparsers</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">2</span></a>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">3</span></a><span class="kn">from</span> <span class="nn">.databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">_connect</span><span class="p">,</span> <span class="n">_disconnect</span><span class="p">,</span> <span class="n">data_to_string</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">4</span></a><span class="kn">from</span> <span class="nn">.dbshell</span> <span class="kn">import</span> <span class="n">DBShell</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">3</span></a><span class="kn">from</span> <span class="nn">.create_shell</span> <span class="kn">import</span> <span class="n">create_shell</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">4</span></a><span class="kn">from</span> <span class="nn">.databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">_connect</span><span class="p">,</span> <span class="n">_disconnect</span><span class="p">,</span> <span class="n">data_to_string</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">5</span></a><span class="kn">from</span> <span class="nn">.dbshell</span> <span class="kn">import</span> <span class="n">DBShell</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
 
 
   ⁰
 [Unknown INPUT type]
 ***** Submodules *****
+    * create_shell
     * customshell
     * databased
     * dbparsers
     * dbshell
 built_with_pdoc[pdoc_logo]
 
 ****** databased ******
 ⁰ View Source
 1from databased import dbparsers
 2
-3from .databased import DataBased, _connect, _disconnect, data_to_string
-4from .dbshell import DBShell
+3from .create_shell import create_shell
+4from .databased import DataBased, _connect, _disconnect, data_to_string
+5from .dbshell import DBShell
```

### Comparing `databased-2.4.1/docs/search.js` & `databased-2.5.0/docs/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -684,14 +684,43 @@
     /** pdoc search index */
     const docs = [{
         "fullname": "databased",
         "modulename": "databased",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
+        "fullname": "databased.create_shell",
+        "modulename": "databased.create_shell",
+        "kind": "module",
+        "doc": "<p></p>\n"
+    }, {
+        "fullname": "databased.create_shell.get_args",
+        "modulename": "databased.create_shell",
+        "qualname": "get_args",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span>:</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "databased.create_shell.create_shell",
+        "modulename": "databased.create_shell",
+        "qualname": "create_shell",
+        "kind": "function",
+        "doc": "<p>Generate a template file in the current working directory for a custom DBShell class.</p>\n\n<p><code>name</code> will be used to name the generated file as well as several components in the file content.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "databased.create_shell.main",
+        "modulename": "databased.create_shell",
+        "qualname": "main",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "databased.customshell",
         "modulename": "databased.customshell",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
         "fullname": "databased.customshell.CustomShell",
         "modulename": "databased.customshell",
@@ -734,16 +763,16 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.vacuum",
         "modulename": "databased.databased",
         "qualname": "DataBased.vacuum",
         "kind": "function",
-        "doc": "<p>Reduce disk size of the database with a <code>VACUUM</code> query.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
+        "doc": "<p>Reduce disk size of the database with a <code>VACUUM</code> query.</p>\n\n<p>Returns space freed up in bytes.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "databased.databased.DataBased.query",
         "modulename": "databased.databased",
         "qualname": "DataBased.query",
         "kind": "function",
         "doc": "<p>Execute an arbitrary query and return the results.</p>\n",
```

### Comparing `databased-2.4.1/docs/databased/customshell.html` & `databased-2.5.0/docs/databased/customshell.html`

 * *Files identical despite different names*

### Comparing `databased-2.4.1/docs/databased/databased.html` & `databased-2.5.0/docs/databased/databased.html`

 * *Files 0% similar despite different names*

```diff
@@ -301,427 +301,431 @@
 </span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
 </span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
 </span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>            <span class="p">)</span>
 </span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
 </span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.&quot;&quot;&quot;</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">        Returns space freed up in bytes.&quot;&quot;&quot;</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">return</span> <span class="n">size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
 </span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="p">)</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>                <span class="p">)</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">        Returns whether the addition was successful or not.</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="p">)</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>                <span class="p">)</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
 </span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">        Returns whether the addition was successful or not.</span>
 </span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        #### :params:</span>
 </span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                    <span class="n">values</span><span class="p">,</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                <span class="p">)</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>                    <span class="n">values</span><span class="p">,</span>
 </span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>                <span class="p">)</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>                <span class="p">)</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
-</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a>
-</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a>    <span class="k">def</span> <span class="nf">add_rows</span><span class="p">(</span>
-</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">]],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
-</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>        <span class="sd">&quot;&quot;&quot;Add multiple rows of values to a table.</span>
-</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a>
-</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a><span class="sd">        Returns a tuple containing the number of successful additions and the number of failed additions.</span>
-</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>
-</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>                <span class="p">)</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a>                <span class="p">)</span>
+</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a>
+</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a>    <span class="k">def</span> <span class="nf">add_rows</span><span class="p">(</span>
+</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">]],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
+</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>        <span class="sd">&quot;&quot;&quot;Add multiple rows of values to a table.</span>
 </span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a>
-</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a><span class="sd">        Returns a tuple containing the number of successful additions and the number of failed additions.</span>
 </span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a>
-</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a><span class="sd">        `values`: A list of tuples of values to be inserted into the table.</span>
-</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a><span class="sd">        Each tuple constitutes a single row to be inserted</span>
-</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a>
-</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
-</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
-</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>        <span class="n">successes</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>        <span class="n">failures</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a>        <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">values</span><span class="p">:</span>
-</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">row</span><span class="p">,</span> <span class="n">columns</span><span class="p">):</span>
-</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>                <span class="n">successes</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>                <span class="n">failures</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">successes</span><span class="p">,</span> <span class="n">failures</span><span class="p">)</span>
-</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a>
-</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
-</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>
-</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
-</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a>
-</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>
-</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a>
-</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
-</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
-</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a>
+</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a>
+</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a><span class="sd">        `values`: A list of tuples of values to be inserted into the table.</span>
+</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a><span class="sd">        Each tuple constitutes a single row to be inserted</span>
+</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>
+</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>        <span class="n">successes</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a>        <span class="n">failures</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>        <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">values</span><span class="p">:</span>
+</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">row</span><span class="p">,</span> <span class="n">columns</span><span class="p">):</span>
+</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a>                <span class="n">successes</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a>                <span class="n">failures</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">successes</span><span class="p">,</span> <span class="n">failures</span><span class="p">)</span>
+</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a>
+</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
+</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a>
+</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
+</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a>
+</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a>
+</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a><span class="sd">        #### :params:</span>
 </span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a>
-</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
-</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a>
-</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
-</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a>
+</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
 </span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a>
-</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
-</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
-</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
+</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
+</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
 </span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a>
-</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
-</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a>
-</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
+</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
+</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
 </span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a>
-</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
 </span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a>
-</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
-</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a>
-</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
-</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a>            <span class="k">return</span> <span class="n">results</span>
-</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a>
-</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
-</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a>
-</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a>
-</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a>
+</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a>
+</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
+</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a>
+</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
+</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a>
+</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
 </span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a>
-</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="sd">        #### :params:</span>
 </span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a>
-</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
-</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a>                <span class="p">[</span>
-</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>                    <span class="n">row</span>
-</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a>                    <span class="p">)</span>
-</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a>                <span class="p">]</span>
-</span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>            <span class="p">)</span>
-</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a>        <span class="k">return</span> <span class="n">results</span>
-</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a>
-</span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-437"><a href="#L-437"><span class="linenos">437</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
-</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a>
-</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a><span class="sd">        Returns the number of deleted records.</span>
-</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a>
-</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a>
+</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a>
+</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
+</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a>                <span class="p">[</span>
+</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a>                    <span class="n">row</span>
+</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a>                    <span class="p">)</span>
+</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a>                <span class="p">]</span>
+</span><span id="L-437"><a href="#L-437"><span class="linenos">437</span></a>            <span class="p">)</span>
+</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a>
+</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
 </span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a>
-</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
-</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
-</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a>
-</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
-</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
-</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
-</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>            <span class="p">)</span>
-</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
-</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
-</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a>                <span class="sa">f</span><span class="s1">&#39;Error deleting rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a>            <span class="p">)</span>
-</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>
-</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
-</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>
-</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>
-</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a><span class="sd">        `table`: The table to update rows in.</span>
+</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a><span class="sd">        Returns the number of deleted records.</span>
+</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a>
+</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>
+</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
+</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a>
+</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
+</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
+</span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a>            <span class="p">)</span>
+</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
+</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
+</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a>                <span class="sa">f</span><span class="s1">&#39;Error deleting rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>            <span class="p">)</span>
+</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a>
+</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
 </span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>
-</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
+</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a><span class="sd">        #### :params:</span>
 </span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a>
-</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a><span class="sd">        `new_value`: The new value to insert.</span>
+</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a><span class="sd">        `table`: The table to update rows in.</span>
 </span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>
-</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
-</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
-</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
+</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>
+</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a><span class="sd">        `new_value`: The new value to insert.</span>
 </span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a>
-</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
-</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>
-</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
-</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a>            <span class="p">)</span>
-</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>            <span class="n">num_updates</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
-</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>                <span class="sa">f</span><span class="s1">&#39;In </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s1"> rows, updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
+</span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a>
+</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
+</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a>
+</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
+</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
 </span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>            <span class="p">)</span>
-</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a>            <span class="k">return</span> <span class="n">num_updates</span>
-</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>            <span class="p">)</span>
-</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>
-</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a>            <span class="n">num_updates</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
+</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a>                <span class="sa">f</span><span class="s1">&#39;In </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s1"> rows, updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>            <span class="p">)</span>
+</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>            <span class="k">return</span> <span class="n">num_updates</span>
+</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>            <span class="p">)</span>
+</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>
-</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
-</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
-</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a>
-</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a>    <span class="nd">@_connect</span>
-</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a>    <span class="p">):</span>
-</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
-</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>
-</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a>
-</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>
+</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
+</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a>
+</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>    <span class="nd">@_connect</span>
+</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a>    <span class="p">):</span>
+</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
 </span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a>
-</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a><span class="sd">        #### :params:</span>
 </span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a>
-</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a>                <span class="p">)</span>
-</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
-</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>                <span class="p">)</span>
-</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>
-</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a>
-</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a>
-</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a>
-</span><span id="L-567"><a href="#L-567"><span class="linenos">567</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
-</span><span id="L-568"><a href="#L-568"><span class="linenos">568</span></a>
-</span><span id="L-569"><a href="#L-569"><span class="linenos">569</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="L-570"><a href="#L-570"><span class="linenos">570</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="L-571"><a href="#L-571"><span class="linenos">571</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>
+</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a>
+</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>                <span class="p">)</span>
+</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
+</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>                <span class="p">)</span>
+</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a>
+</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a>
+</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-567"><a href="#L-567"><span class="linenos">567</span></a>
+</span><span id="L-568"><a href="#L-568"><span class="linenos">568</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="L-569"><a href="#L-569"><span class="linenos">569</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="L-570"><a href="#L-570"><span class="linenos">570</span></a>
+</span><span id="L-571"><a href="#L-571"><span class="linenos">571</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
 </span><span id="L-572"><a href="#L-572"><span class="linenos">572</span></a>
-</span><span id="L-573"><a href="#L-573"><span class="linenos">573</span></a>
-</span><span id="L-574"><a href="#L-574"><span class="linenos">574</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-575"><a href="#L-575"><span class="linenos">575</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-576"><a href="#L-576"><span class="linenos">576</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-577"><a href="#L-577"><span class="linenos">577</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="L-578"><a href="#L-578"><span class="linenos">578</span></a>
-</span><span id="L-579"><a href="#L-579"><span class="linenos">579</span></a><span class="sd">    #### :params:</span>
-</span><span id="L-580"><a href="#L-580"><span class="linenos">580</span></a>
-</span><span id="L-581"><a href="#L-581"><span class="linenos">581</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="L-582"><a href="#L-582"><span class="linenos">582</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-583"><a href="#L-583"><span class="linenos">583</span></a>
-</span><span id="L-584"><a href="#L-584"><span class="linenos">584</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
-</span><span id="L-585"><a href="#L-585"><span class="linenos">585</span></a>
-</span><span id="L-586"><a href="#L-586"><span class="linenos">586</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="L-587"><a href="#L-587"><span class="linenos">587</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="L-588"><a href="#L-588"><span class="linenos">588</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-589"><a href="#L-589"><span class="linenos">589</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-590"><a href="#L-590"><span class="linenos">590</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="L-591"><a href="#L-591"><span class="linenos">591</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="L-592"><a href="#L-592"><span class="linenos">592</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="L-593"><a href="#L-593"><span class="linenos">593</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="L-594"><a href="#L-594"><span class="linenos">594</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="L-595"><a href="#L-595"><span class="linenos">595</span></a>
-</span><span id="L-596"><a href="#L-596"><span class="linenos">596</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-597"><a href="#L-597"><span class="linenos">597</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-598"><a href="#L-598"><span class="linenos">598</span></a>        <span class="k">return</span> <span class="n">griddy</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="s2">&quot;keys&quot;</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
-</span><span id="L-599"><a href="#L-599"><span class="linenos">599</span></a>    <span class="k">except</span> <span class="ne">RuntimeError</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-600"><a href="#L-600"><span class="linenos">600</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-601"><a href="#L-601"><span class="linenos">601</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="L-573"><a href="#L-573"><span class="linenos">573</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="L-574"><a href="#L-574"><span class="linenos">574</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="L-575"><a href="#L-575"><span class="linenos">575</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="L-576"><a href="#L-576"><span class="linenos">576</span></a>
+</span><span id="L-577"><a href="#L-577"><span class="linenos">577</span></a>
+</span><span id="L-578"><a href="#L-578"><span class="linenos">578</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-579"><a href="#L-579"><span class="linenos">579</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-580"><a href="#L-580"><span class="linenos">580</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-581"><a href="#L-581"><span class="linenos">581</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="L-582"><a href="#L-582"><span class="linenos">582</span></a>
+</span><span id="L-583"><a href="#L-583"><span class="linenos">583</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-584"><a href="#L-584"><span class="linenos">584</span></a>
+</span><span id="L-585"><a href="#L-585"><span class="linenos">585</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="L-586"><a href="#L-586"><span class="linenos">586</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="L-587"><a href="#L-587"><span class="linenos">587</span></a>
+</span><span id="L-588"><a href="#L-588"><span class="linenos">588</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="L-589"><a href="#L-589"><span class="linenos">589</span></a>
+</span><span id="L-590"><a href="#L-590"><span class="linenos">590</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="L-591"><a href="#L-591"><span class="linenos">591</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="L-592"><a href="#L-592"><span class="linenos">592</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-593"><a href="#L-593"><span class="linenos">593</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-594"><a href="#L-594"><span class="linenos">594</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="L-595"><a href="#L-595"><span class="linenos">595</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="L-596"><a href="#L-596"><span class="linenos">596</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="L-597"><a href="#L-597"><span class="linenos">597</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="L-598"><a href="#L-598"><span class="linenos">598</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
+</span><span id="L-599"><a href="#L-599"><span class="linenos">599</span></a>
+</span><span id="L-600"><a href="#L-600"><span class="linenos">600</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-601"><a href="#L-601"><span class="linenos">601</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-602"><a href="#L-602"><span class="linenos">602</span></a>        <span class="k">return</span> <span class="n">griddy</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="s2">&quot;keys&quot;</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="L-603"><a href="#L-603"><span class="linenos">603</span></a>    <span class="k">except</span> <span class="ne">RuntimeError</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-604"><a href="#L-604"><span class="linenos">604</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-605"><a href="#L-605"><span class="linenos">605</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DataBased">
                             <input id="DataBased-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -873,397 +877,401 @@
 </span><span id="DataBased-183"><a href="#DataBased-183"><span class="linenos">183</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="DataBased-184"><a href="#DataBased-184"><span class="linenos">184</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot; and &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
 </span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
 </span><span id="DataBased-186"><a href="#DataBased-186"><span class="linenos">186</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
 </span><span id="DataBased-187"><a href="#DataBased-187"><span class="linenos">187</span></a>            <span class="p">)</span>
 </span><span id="DataBased-188"><a href="#DataBased-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
 </span><span id="DataBased-189"><a href="#DataBased-189"><span class="linenos">189</span></a>
-</span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.&quot;&quot;&quot;</span>
-</span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
-</span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a>
-</span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
-</span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased-199"><a href="#DataBased-199"><span class="linenos">199</span></a>
-</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-201"><a href="#DataBased-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="DataBased-202"><a href="#DataBased-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.</span>
+</span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>
+</span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a><span class="sd">        Returns space freed up in bytes.&quot;&quot;&quot;</span>
+</span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>        <span class="k">return</span> <span class="n">size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>
+</span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-199"><a href="#DataBased-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
+</span><span id="DataBased-201"><a href="#DataBased-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="DataBased-202"><a href="#DataBased-202"><span class="linenos">202</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span><span id="DataBased-203"><a href="#DataBased-203"><span class="linenos">203</span></a>
-</span><span id="DataBased-204"><a href="#DataBased-204"><span class="linenos">204</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
-</span><span id="DataBased-205"><a href="#DataBased-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased-206"><a href="#DataBased-206"><span class="linenos">206</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DataBased-207"><a href="#DataBased-207"><span class="linenos">207</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
-</span><span id="DataBased-208"><a href="#DataBased-208"><span class="linenos">208</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased-209"><a href="#DataBased-209"><span class="linenos">209</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
-</span><span id="DataBased-210"><a href="#DataBased-210"><span class="linenos">210</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-211"><a href="#DataBased-211"><span class="linenos">211</span></a>
-</span><span id="DataBased-212"><a href="#DataBased-212"><span class="linenos">212</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-213"><a href="#DataBased-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="DataBased-214"><a href="#DataBased-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
+</span><span id="DataBased-204"><a href="#DataBased-204"><span class="linenos">204</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-205"><a href="#DataBased-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="DataBased-206"><a href="#DataBased-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased-207"><a href="#DataBased-207"><span class="linenos">207</span></a>
+</span><span id="DataBased-208"><a href="#DataBased-208"><span class="linenos">208</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
+</span><span id="DataBased-209"><a href="#DataBased-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased-210"><a href="#DataBased-210"><span class="linenos">210</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DataBased-211"><a href="#DataBased-211"><span class="linenos">211</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
+</span><span id="DataBased-212"><a href="#DataBased-212"><span class="linenos">212</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="DataBased-213"><a href="#DataBased-213"><span class="linenos">213</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
+</span><span id="DataBased-214"><a href="#DataBased-214"><span class="linenos">214</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span><span id="DataBased-215"><a href="#DataBased-215"><span class="linenos">215</span></a>
-</span><span id="DataBased-216"><a href="#DataBased-216"><span class="linenos">216</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased-217"><a href="#DataBased-217"><span class="linenos">217</span></a>
-</span><span id="DataBased-218"><a href="#DataBased-218"><span class="linenos">218</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="DataBased-216"><a href="#DataBased-216"><span class="linenos">216</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-217"><a href="#DataBased-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="DataBased-218"><a href="#DataBased-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
 </span><span id="DataBased-219"><a href="#DataBased-219"><span class="linenos">219</span></a>
-</span><span id="DataBased-220"><a href="#DataBased-220"><span class="linenos">220</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
-</span><span id="DataBased-221"><a href="#DataBased-221"><span class="linenos">221</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
-</span><span id="DataBased-222"><a href="#DataBased-222"><span class="linenos">222</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
-</span><span id="DataBased-224"><a href="#DataBased-224"><span class="linenos">224</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased-225"><a href="#DataBased-225"><span class="linenos">225</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
-</span><span id="DataBased-226"><a href="#DataBased-226"><span class="linenos">226</span></a>
-</span><span id="DataBased-227"><a href="#DataBased-227"><span class="linenos">227</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-228"><a href="#DataBased-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased-229"><a href="#DataBased-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
-</span><span id="DataBased-230"><a href="#DataBased-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-231"><a href="#DataBased-231"><span class="linenos">231</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
-</span><span id="DataBased-232"><a href="#DataBased-232"><span class="linenos">232</span></a>        <span class="p">)</span>
-</span><span id="DataBased-233"><a href="#DataBased-233"><span class="linenos">233</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
-</span><span id="DataBased-234"><a href="#DataBased-234"><span class="linenos">234</span></a>
-</span><span id="DataBased-235"><a href="#DataBased-235"><span class="linenos">235</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-236"><a href="#DataBased-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased-237"><a href="#DataBased-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased-238"><a href="#DataBased-238"><span class="linenos">238</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
-</span><span id="DataBased-239"><a href="#DataBased-239"><span class="linenos">239</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
-</span><span id="DataBased-240"><a href="#DataBased-240"><span class="linenos">240</span></a>
-</span><span id="DataBased-241"><a href="#DataBased-241"><span class="linenos">241</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-242"><a href="#DataBased-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="DataBased-243"><a href="#DataBased-243"><span class="linenos">243</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-244"><a href="#DataBased-244"><span class="linenos">244</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-245"><a href="#DataBased-245"><span class="linenos">245</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-246"><a href="#DataBased-246"><span class="linenos">246</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased-247"><a href="#DataBased-247"><span class="linenos">247</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased-248"><a href="#DataBased-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
-</span><span id="DataBased-249"><a href="#DataBased-249"><span class="linenos">249</span></a>
-</span><span id="DataBased-250"><a href="#DataBased-250"><span class="linenos">250</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased-251"><a href="#DataBased-251"><span class="linenos">251</span></a>
-</span><span id="DataBased-252"><a href="#DataBased-252"><span class="linenos">252</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-253"><a href="#DataBased-253"><span class="linenos">253</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
-</span><span id="DataBased-254"><a href="#DataBased-254"><span class="linenos">254</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased-255"><a href="#DataBased-255"><span class="linenos">255</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
-</span><span id="DataBased-256"><a href="#DataBased-256"><span class="linenos">256</span></a>
-</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
-</span><span id="DataBased-258"><a href="#DataBased-258"><span class="linenos">258</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
-</span><span id="DataBased-259"><a href="#DataBased-259"><span class="linenos">259</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
-</span><span id="DataBased-260"><a href="#DataBased-260"><span class="linenos">260</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-261"><a href="#DataBased-261"><span class="linenos">261</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
-</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-263"><a href="#DataBased-263"><span class="linenos">263</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-264"><a href="#DataBased-264"><span class="linenos">264</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-265"><a href="#DataBased-265"><span class="linenos">265</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DataBased-266"><a href="#DataBased-266"><span class="linenos">266</span></a>                <span class="p">)</span>
-</span><span id="DataBased-267"><a href="#DataBased-267"><span class="linenos">267</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-268"><a href="#DataBased-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased-269"><a href="#DataBased-269"><span class="linenos">269</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DataBased-270"><a href="#DataBased-270"><span class="linenos">270</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="DataBased-271"><a href="#DataBased-271"><span class="linenos">271</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="DataBased-272"><a href="#DataBased-272"><span class="linenos">272</span></a>
-</span><span id="DataBased-273"><a href="#DataBased-273"><span class="linenos">273</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-274"><a href="#DataBased-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
-</span><span id="DataBased-275"><a href="#DataBased-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-276"><a href="#DataBased-276"><span class="linenos">276</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased-277"><a href="#DataBased-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
-</span><span id="DataBased-278"><a href="#DataBased-278"><span class="linenos">278</span></a>
-</span><span id="DataBased-279"><a href="#DataBased-279"><span class="linenos">279</span></a><span class="sd">        Returns whether the addition was successful or not.</span>
-</span><span id="DataBased-280"><a href="#DataBased-280"><span class="linenos">280</span></a>
-</span><span id="DataBased-281"><a href="#DataBased-281"><span class="linenos">281</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-220"><a href="#DataBased-220"><span class="linenos">220</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-221"><a href="#DataBased-221"><span class="linenos">221</span></a>
+</span><span id="DataBased-222"><a href="#DataBased-222"><span class="linenos">222</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a>
+</span><span id="DataBased-224"><a href="#DataBased-224"><span class="linenos">224</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
+</span><span id="DataBased-225"><a href="#DataBased-225"><span class="linenos">225</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
+</span><span id="DataBased-226"><a href="#DataBased-226"><span class="linenos">226</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="DataBased-227"><a href="#DataBased-227"><span class="linenos">227</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="DataBased-228"><a href="#DataBased-228"><span class="linenos">228</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased-229"><a href="#DataBased-229"><span class="linenos">229</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+</span><span id="DataBased-230"><a href="#DataBased-230"><span class="linenos">230</span></a>
+</span><span id="DataBased-231"><a href="#DataBased-231"><span class="linenos">231</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-232"><a href="#DataBased-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased-233"><a href="#DataBased-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
+</span><span id="DataBased-234"><a href="#DataBased-234"><span class="linenos">234</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-235"><a href="#DataBased-235"><span class="linenos">235</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
+</span><span id="DataBased-236"><a href="#DataBased-236"><span class="linenos">236</span></a>        <span class="p">)</span>
+</span><span id="DataBased-237"><a href="#DataBased-237"><span class="linenos">237</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+</span><span id="DataBased-238"><a href="#DataBased-238"><span class="linenos">238</span></a>
+</span><span id="DataBased-239"><a href="#DataBased-239"><span class="linenos">239</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-240"><a href="#DataBased-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased-241"><a href="#DataBased-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="DataBased-242"><a href="#DataBased-242"><span class="linenos">242</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-243"><a href="#DataBased-243"><span class="linenos">243</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+</span><span id="DataBased-244"><a href="#DataBased-244"><span class="linenos">244</span></a>
+</span><span id="DataBased-245"><a href="#DataBased-245"><span class="linenos">245</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-246"><a href="#DataBased-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="DataBased-247"><a href="#DataBased-247"><span class="linenos">247</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-248"><a href="#DataBased-248"><span class="linenos">248</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-249"><a href="#DataBased-249"><span class="linenos">249</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-250"><a href="#DataBased-250"><span class="linenos">250</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased-251"><a href="#DataBased-251"><span class="linenos">251</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-252"><a href="#DataBased-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
+</span><span id="DataBased-253"><a href="#DataBased-253"><span class="linenos">253</span></a>
+</span><span id="DataBased-254"><a href="#DataBased-254"><span class="linenos">254</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-255"><a href="#DataBased-255"><span class="linenos">255</span></a>
+</span><span id="DataBased-256"><a href="#DataBased-256"><span class="linenos">256</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased-258"><a href="#DataBased-258"><span class="linenos">258</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-259"><a href="#DataBased-259"><span class="linenos">259</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
+</span><span id="DataBased-260"><a href="#DataBased-260"><span class="linenos">260</span></a>
+</span><span id="DataBased-261"><a href="#DataBased-261"><span class="linenos">261</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
+</span><span id="DataBased-263"><a href="#DataBased-263"><span class="linenos">263</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
+</span><span id="DataBased-264"><a href="#DataBased-264"><span class="linenos">264</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-265"><a href="#DataBased-265"><span class="linenos">265</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
+</span><span id="DataBased-266"><a href="#DataBased-266"><span class="linenos">266</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-267"><a href="#DataBased-267"><span class="linenos">267</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-268"><a href="#DataBased-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-269"><a href="#DataBased-269"><span class="linenos">269</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased-270"><a href="#DataBased-270"><span class="linenos">270</span></a>                <span class="p">)</span>
+</span><span id="DataBased-271"><a href="#DataBased-271"><span class="linenos">271</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-272"><a href="#DataBased-272"><span class="linenos">272</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased-273"><a href="#DataBased-273"><span class="linenos">273</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DataBased-274"><a href="#DataBased-274"><span class="linenos">274</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="DataBased-275"><a href="#DataBased-275"><span class="linenos">275</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased-276"><a href="#DataBased-276"><span class="linenos">276</span></a>
+</span><span id="DataBased-277"><a href="#DataBased-277"><span class="linenos">277</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-278"><a href="#DataBased-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="DataBased-279"><a href="#DataBased-279"><span class="linenos">279</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-280"><a href="#DataBased-280"><span class="linenos">280</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased-281"><a href="#DataBased-281"><span class="linenos">281</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
 </span><span id="DataBased-282"><a href="#DataBased-282"><span class="linenos">282</span></a>
-</span><span id="DataBased-283"><a href="#DataBased-283"><span class="linenos">283</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased-283"><a href="#DataBased-283"><span class="linenos">283</span></a><span class="sd">        Returns whether the addition was successful or not.</span>
 </span><span id="DataBased-284"><a href="#DataBased-284"><span class="linenos">284</span></a>
-</span><span id="DataBased-285"><a href="#DataBased-285"><span class="linenos">285</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased-285"><a href="#DataBased-285"><span class="linenos">285</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased-286"><a href="#DataBased-286"><span class="linenos">286</span></a>
-</span><span id="DataBased-287"><a href="#DataBased-287"><span class="linenos">287</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
-</span><span id="DataBased-288"><a href="#DataBased-288"><span class="linenos">288</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
-</span><span id="DataBased-289"><a href="#DataBased-289"><span class="linenos">289</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-290"><a href="#DataBased-290"><span class="linenos">290</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased-291"><a href="#DataBased-291"><span class="linenos">291</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-292"><a href="#DataBased-292"><span class="linenos">292</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-293"><a href="#DataBased-293"><span class="linenos">293</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="DataBased-294"><a href="#DataBased-294"><span class="linenos">294</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-295"><a href="#DataBased-295"><span class="linenos">295</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
-</span><span id="DataBased-296"><a href="#DataBased-296"><span class="linenos">296</span></a>                    <span class="n">values</span><span class="p">,</span>
-</span><span id="DataBased-297"><a href="#DataBased-297"><span class="linenos">297</span></a>                <span class="p">)</span>
-</span><span id="DataBased-298"><a href="#DataBased-298"><span class="linenos">298</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-299"><a href="#DataBased-299"><span class="linenos">299</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-300"><a href="#DataBased-300"><span class="linenos">300</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased-287"><a href="#DataBased-287"><span class="linenos">287</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased-288"><a href="#DataBased-288"><span class="linenos">288</span></a>
+</span><span id="DataBased-289"><a href="#DataBased-289"><span class="linenos">289</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased-290"><a href="#DataBased-290"><span class="linenos">290</span></a>
+</span><span id="DataBased-291"><a href="#DataBased-291"><span class="linenos">291</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="DataBased-292"><a href="#DataBased-292"><span class="linenos">292</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="DataBased-293"><a href="#DataBased-293"><span class="linenos">293</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-294"><a href="#DataBased-294"><span class="linenos">294</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased-295"><a href="#DataBased-295"><span class="linenos">295</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-296"><a href="#DataBased-296"><span class="linenos">296</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-297"><a href="#DataBased-297"><span class="linenos">297</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="DataBased-298"><a href="#DataBased-298"><span class="linenos">298</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-299"><a href="#DataBased-299"><span class="linenos">299</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="DataBased-300"><a href="#DataBased-300"><span class="linenos">300</span></a>                    <span class="n">values</span><span class="p">,</span>
 </span><span id="DataBased-301"><a href="#DataBased-301"><span class="linenos">301</span></a>                <span class="p">)</span>
-</span><span id="DataBased-302"><a href="#DataBased-302"><span class="linenos">302</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-303"><a href="#DataBased-303"><span class="linenos">303</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased-304"><a href="#DataBased-304"><span class="linenos">304</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-305"><a href="#DataBased-305"><span class="linenos">305</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="DataBased-306"><a href="#DataBased-306"><span class="linenos">306</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="DataBased-307"><a href="#DataBased-307"><span class="linenos">307</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="DataBased-308"><a href="#DataBased-308"><span class="linenos">308</span></a>                <span class="p">)</span>
-</span><span id="DataBased-309"><a href="#DataBased-309"><span class="linenos">309</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-310"><a href="#DataBased-310"><span class="linenos">310</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
-</span><span id="DataBased-311"><a href="#DataBased-311"><span class="linenos">311</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-312"><a href="#DataBased-312"><span class="linenos">312</span></a>
-</span><span id="DataBased-313"><a href="#DataBased-313"><span class="linenos">313</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-314"><a href="#DataBased-314"><span class="linenos">314</span></a>    <span class="k">def</span> <span class="nf">add_rows</span><span class="p">(</span>
-</span><span id="DataBased-315"><a href="#DataBased-315"><span class="linenos">315</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">]],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-316"><a href="#DataBased-316"><span class="linenos">316</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
-</span><span id="DataBased-317"><a href="#DataBased-317"><span class="linenos">317</span></a>        <span class="sd">&quot;&quot;&quot;Add multiple rows of values to a table.</span>
-</span><span id="DataBased-318"><a href="#DataBased-318"><span class="linenos">318</span></a>
-</span><span id="DataBased-319"><a href="#DataBased-319"><span class="linenos">319</span></a><span class="sd">        Returns a tuple containing the number of successful additions and the number of failed additions.</span>
-</span><span id="DataBased-320"><a href="#DataBased-320"><span class="linenos">320</span></a>
-</span><span id="DataBased-321"><a href="#DataBased-321"><span class="linenos">321</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-302"><a href="#DataBased-302"><span class="linenos">302</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-303"><a href="#DataBased-303"><span class="linenos">303</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-304"><a href="#DataBased-304"><span class="linenos">304</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased-305"><a href="#DataBased-305"><span class="linenos">305</span></a>                <span class="p">)</span>
+</span><span id="DataBased-306"><a href="#DataBased-306"><span class="linenos">306</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-307"><a href="#DataBased-307"><span class="linenos">307</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased-308"><a href="#DataBased-308"><span class="linenos">308</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-309"><a href="#DataBased-309"><span class="linenos">309</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="DataBased-310"><a href="#DataBased-310"><span class="linenos">310</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="DataBased-311"><a href="#DataBased-311"><span class="linenos">311</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
+</span><span id="DataBased-312"><a href="#DataBased-312"><span class="linenos">312</span></a>                <span class="p">)</span>
+</span><span id="DataBased-313"><a href="#DataBased-313"><span class="linenos">313</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-314"><a href="#DataBased-314"><span class="linenos">314</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="DataBased-315"><a href="#DataBased-315"><span class="linenos">315</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-316"><a href="#DataBased-316"><span class="linenos">316</span></a>
+</span><span id="DataBased-317"><a href="#DataBased-317"><span class="linenos">317</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-318"><a href="#DataBased-318"><span class="linenos">318</span></a>    <span class="k">def</span> <span class="nf">add_rows</span><span class="p">(</span>
+</span><span id="DataBased-319"><a href="#DataBased-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">]],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-320"><a href="#DataBased-320"><span class="linenos">320</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
+</span><span id="DataBased-321"><a href="#DataBased-321"><span class="linenos">321</span></a>        <span class="sd">&quot;&quot;&quot;Add multiple rows of values to a table.</span>
 </span><span id="DataBased-322"><a href="#DataBased-322"><span class="linenos">322</span></a>
-</span><span id="DataBased-323"><a href="#DataBased-323"><span class="linenos">323</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased-323"><a href="#DataBased-323"><span class="linenos">323</span></a><span class="sd">        Returns a tuple containing the number of successful additions and the number of failed additions.</span>
 </span><span id="DataBased-324"><a href="#DataBased-324"><span class="linenos">324</span></a>
-</span><span id="DataBased-325"><a href="#DataBased-325"><span class="linenos">325</span></a><span class="sd">        `values`: A list of tuples of values to be inserted into the table.</span>
-</span><span id="DataBased-326"><a href="#DataBased-326"><span class="linenos">326</span></a><span class="sd">        Each tuple constitutes a single row to be inserted</span>
-</span><span id="DataBased-327"><a href="#DataBased-327"><span class="linenos">327</span></a>
-</span><span id="DataBased-328"><a href="#DataBased-328"><span class="linenos">328</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
-</span><span id="DataBased-329"><a href="#DataBased-329"><span class="linenos">329</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
-</span><span id="DataBased-330"><a href="#DataBased-330"><span class="linenos">330</span></a>        <span class="n">successes</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="DataBased-331"><a href="#DataBased-331"><span class="linenos">331</span></a>        <span class="n">failures</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="DataBased-332"><a href="#DataBased-332"><span class="linenos">332</span></a>        <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">values</span><span class="p">:</span>
-</span><span id="DataBased-333"><a href="#DataBased-333"><span class="linenos">333</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">row</span><span class="p">,</span> <span class="n">columns</span><span class="p">):</span>
-</span><span id="DataBased-334"><a href="#DataBased-334"><span class="linenos">334</span></a>                <span class="n">successes</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="DataBased-335"><a href="#DataBased-335"><span class="linenos">335</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-336"><a href="#DataBased-336"><span class="linenos">336</span></a>                <span class="n">failures</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="DataBased-337"><a href="#DataBased-337"><span class="linenos">337</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">successes</span><span class="p">,</span> <span class="n">failures</span><span class="p">)</span>
-</span><span id="DataBased-338"><a href="#DataBased-338"><span class="linenos">338</span></a>
-</span><span id="DataBased-339"><a href="#DataBased-339"><span class="linenos">339</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-340"><a href="#DataBased-340"><span class="linenos">340</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="DataBased-341"><a href="#DataBased-341"><span class="linenos">341</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-342"><a href="#DataBased-342"><span class="linenos">342</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-343"><a href="#DataBased-343"><span class="linenos">343</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-344"><a href="#DataBased-344"><span class="linenos">344</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased-345"><a href="#DataBased-345"><span class="linenos">345</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-347"><a href="#DataBased-347"><span class="linenos">347</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased-348"><a href="#DataBased-348"><span class="linenos">348</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased-349"><a href="#DataBased-349"><span class="linenos">349</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-350"><a href="#DataBased-350"><span class="linenos">350</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-351"><a href="#DataBased-351"><span class="linenos">351</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="DataBased-352"><a href="#DataBased-352"><span class="linenos">352</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
-</span><span id="DataBased-353"><a href="#DataBased-353"><span class="linenos">353</span></a>
-</span><span id="DataBased-354"><a href="#DataBased-354"><span class="linenos">354</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
-</span><span id="DataBased-355"><a href="#DataBased-355"><span class="linenos">355</span></a>
-</span><span id="DataBased-356"><a href="#DataBased-356"><span class="linenos">356</span></a>
-</span><span id="DataBased-357"><a href="#DataBased-357"><span class="linenos">357</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased-358"><a href="#DataBased-358"><span class="linenos">358</span></a>
-</span><span id="DataBased-359"><a href="#DataBased-359"><span class="linenos">359</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased-360"><a href="#DataBased-360"><span class="linenos">360</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
-</span><span id="DataBased-361"><a href="#DataBased-361"><span class="linenos">361</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-325"><a href="#DataBased-325"><span class="linenos">325</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-326"><a href="#DataBased-326"><span class="linenos">326</span></a>
+</span><span id="DataBased-327"><a href="#DataBased-327"><span class="linenos">327</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased-328"><a href="#DataBased-328"><span class="linenos">328</span></a>
+</span><span id="DataBased-329"><a href="#DataBased-329"><span class="linenos">329</span></a><span class="sd">        `values`: A list of tuples of values to be inserted into the table.</span>
+</span><span id="DataBased-330"><a href="#DataBased-330"><span class="linenos">330</span></a><span class="sd">        Each tuple constitutes a single row to be inserted</span>
+</span><span id="DataBased-331"><a href="#DataBased-331"><span class="linenos">331</span></a>
+</span><span id="DataBased-332"><a href="#DataBased-332"><span class="linenos">332</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="DataBased-333"><a href="#DataBased-333"><span class="linenos">333</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="DataBased-334"><a href="#DataBased-334"><span class="linenos">334</span></a>        <span class="n">successes</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="DataBased-335"><a href="#DataBased-335"><span class="linenos">335</span></a>        <span class="n">failures</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="DataBased-336"><a href="#DataBased-336"><span class="linenos">336</span></a>        <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">values</span><span class="p">:</span>
+</span><span id="DataBased-337"><a href="#DataBased-337"><span class="linenos">337</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">row</span><span class="p">,</span> <span class="n">columns</span><span class="p">):</span>
+</span><span id="DataBased-338"><a href="#DataBased-338"><span class="linenos">338</span></a>                <span class="n">successes</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="DataBased-339"><a href="#DataBased-339"><span class="linenos">339</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-340"><a href="#DataBased-340"><span class="linenos">340</span></a>                <span class="n">failures</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="DataBased-341"><a href="#DataBased-341"><span class="linenos">341</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">successes</span><span class="p">,</span> <span class="n">failures</span><span class="p">)</span>
+</span><span id="DataBased-342"><a href="#DataBased-342"><span class="linenos">342</span></a>
+</span><span id="DataBased-343"><a href="#DataBased-343"><span class="linenos">343</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-344"><a href="#DataBased-344"><span class="linenos">344</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="DataBased-345"><a href="#DataBased-345"><span class="linenos">345</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-347"><a href="#DataBased-347"><span class="linenos">347</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-348"><a href="#DataBased-348"><span class="linenos">348</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased-349"><a href="#DataBased-349"><span class="linenos">349</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-350"><a href="#DataBased-350"><span class="linenos">350</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-351"><a href="#DataBased-351"><span class="linenos">351</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased-352"><a href="#DataBased-352"><span class="linenos">352</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased-353"><a href="#DataBased-353"><span class="linenos">353</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-354"><a href="#DataBased-354"><span class="linenos">354</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-355"><a href="#DataBased-355"><span class="linenos">355</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="DataBased-356"><a href="#DataBased-356"><span class="linenos">356</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
+</span><span id="DataBased-357"><a href="#DataBased-357"><span class="linenos">357</span></a>
+</span><span id="DataBased-358"><a href="#DataBased-358"><span class="linenos">358</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
+</span><span id="DataBased-359"><a href="#DataBased-359"><span class="linenos">359</span></a>
+</span><span id="DataBased-360"><a href="#DataBased-360"><span class="linenos">360</span></a>
+</span><span id="DataBased-361"><a href="#DataBased-361"><span class="linenos">361</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased-362"><a href="#DataBased-362"><span class="linenos">362</span></a>
-</span><span id="DataBased-363"><a href="#DataBased-363"><span class="linenos">363</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
-</span><span id="DataBased-364"><a href="#DataBased-364"><span class="linenos">364</span></a>
-</span><span id="DataBased-365"><a href="#DataBased-365"><span class="linenos">365</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
-</span><span id="DataBased-366"><a href="#DataBased-366"><span class="linenos">366</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="DataBased-367"><a href="#DataBased-367"><span class="linenos">367</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="DataBased-363"><a href="#DataBased-363"><span class="linenos">363</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased-364"><a href="#DataBased-364"><span class="linenos">364</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased-365"><a href="#DataBased-365"><span class="linenos">365</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased-366"><a href="#DataBased-366"><span class="linenos">366</span></a>
+</span><span id="DataBased-367"><a href="#DataBased-367"><span class="linenos">367</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
 </span><span id="DataBased-368"><a href="#DataBased-368"><span class="linenos">368</span></a>
-</span><span id="DataBased-369"><a href="#DataBased-369"><span class="linenos">369</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
-</span><span id="DataBased-370"><a href="#DataBased-370"><span class="linenos">370</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
-</span><span id="DataBased-371"><a href="#DataBased-371"><span class="linenos">371</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
+</span><span id="DataBased-369"><a href="#DataBased-369"><span class="linenos">369</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
+</span><span id="DataBased-370"><a href="#DataBased-370"><span class="linenos">370</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="DataBased-371"><a href="#DataBased-371"><span class="linenos">371</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
 </span><span id="DataBased-372"><a href="#DataBased-372"><span class="linenos">372</span></a>
-</span><span id="DataBased-373"><a href="#DataBased-373"><span class="linenos">373</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
-</span><span id="DataBased-374"><a href="#DataBased-374"><span class="linenos">374</span></a>
-</span><span id="DataBased-375"><a href="#DataBased-375"><span class="linenos">375</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="DataBased-373"><a href="#DataBased-373"><span class="linenos">373</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
+</span><span id="DataBased-374"><a href="#DataBased-374"><span class="linenos">374</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
+</span><span id="DataBased-375"><a href="#DataBased-375"><span class="linenos">375</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
 </span><span id="DataBased-376"><a href="#DataBased-376"><span class="linenos">376</span></a>
-</span><span id="DataBased-377"><a href="#DataBased-377"><span class="linenos">377</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="DataBased-377"><a href="#DataBased-377"><span class="linenos">377</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
 </span><span id="DataBased-378"><a href="#DataBased-378"><span class="linenos">378</span></a>
-</span><span id="DataBased-379"><a href="#DataBased-379"><span class="linenos">379</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
-</span><span id="DataBased-380"><a href="#DataBased-380"><span class="linenos">380</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-381"><a href="#DataBased-381"><span class="linenos">381</span></a>
-</span><span id="DataBased-382"><a href="#DataBased-382"><span class="linenos">382</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-383"><a href="#DataBased-383"><span class="linenos">383</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased-384"><a href="#DataBased-384"><span class="linenos">384</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
-</span><span id="DataBased-385"><a href="#DataBased-385"><span class="linenos">385</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased-386"><a href="#DataBased-386"><span class="linenos">386</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-387"><a href="#DataBased-387"><span class="linenos">387</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-388"><a href="#DataBased-388"><span class="linenos">388</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="DataBased-389"><a href="#DataBased-389"><span class="linenos">389</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-390"><a href="#DataBased-390"><span class="linenos">390</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="DataBased-391"><a href="#DataBased-391"><span class="linenos">391</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-392"><a href="#DataBased-392"><span class="linenos">392</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased-393"><a href="#DataBased-393"><span class="linenos">393</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased-394"><a href="#DataBased-394"><span class="linenos">394</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased-395"><a href="#DataBased-395"><span class="linenos">395</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="DataBased-396"><a href="#DataBased-396"><span class="linenos">396</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="DataBased-397"><a href="#DataBased-397"><span class="linenos">397</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="DataBased-398"><a href="#DataBased-398"><span class="linenos">398</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="DataBased-399"><a href="#DataBased-399"><span class="linenos">399</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="DataBased-400"><a href="#DataBased-400"><span class="linenos">400</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="DataBased-401"><a href="#DataBased-401"><span class="linenos">401</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DataBased-402"><a href="#DataBased-402"><span class="linenos">402</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-403"><a href="#DataBased-403"><span class="linenos">403</span></a>            <span class="k">return</span> <span class="n">results</span>
-</span><span id="DataBased-404"><a href="#DataBased-404"><span class="linenos">404</span></a>
-</span><span id="DataBased-405"><a href="#DataBased-405"><span class="linenos">405</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-406"><a href="#DataBased-406"><span class="linenos">406</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="DataBased-407"><a href="#DataBased-407"><span class="linenos">407</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-408"><a href="#DataBased-408"><span class="linenos">408</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="DataBased-409"><a href="#DataBased-409"><span class="linenos">409</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
-</span><span id="DataBased-410"><a href="#DataBased-410"><span class="linenos">410</span></a>
-</span><span id="DataBased-411"><a href="#DataBased-411"><span class="linenos">411</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased-412"><a href="#DataBased-412"><span class="linenos">412</span></a>
-</span><span id="DataBased-413"><a href="#DataBased-413"><span class="linenos">413</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="DataBased-379"><a href="#DataBased-379"><span class="linenos">379</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="DataBased-380"><a href="#DataBased-380"><span class="linenos">380</span></a>
+</span><span id="DataBased-381"><a href="#DataBased-381"><span class="linenos">381</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="DataBased-382"><a href="#DataBased-382"><span class="linenos">382</span></a>
+</span><span id="DataBased-383"><a href="#DataBased-383"><span class="linenos">383</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
+</span><span id="DataBased-384"><a href="#DataBased-384"><span class="linenos">384</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-385"><a href="#DataBased-385"><span class="linenos">385</span></a>
+</span><span id="DataBased-386"><a href="#DataBased-386"><span class="linenos">386</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-387"><a href="#DataBased-387"><span class="linenos">387</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="DataBased-388"><a href="#DataBased-388"><span class="linenos">388</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
+</span><span id="DataBased-389"><a href="#DataBased-389"><span class="linenos">389</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased-390"><a href="#DataBased-390"><span class="linenos">390</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-391"><a href="#DataBased-391"><span class="linenos">391</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-392"><a href="#DataBased-392"><span class="linenos">392</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="DataBased-393"><a href="#DataBased-393"><span class="linenos">393</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-394"><a href="#DataBased-394"><span class="linenos">394</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="DataBased-395"><a href="#DataBased-395"><span class="linenos">395</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-396"><a href="#DataBased-396"><span class="linenos">396</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased-397"><a href="#DataBased-397"><span class="linenos">397</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased-398"><a href="#DataBased-398"><span class="linenos">398</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="DataBased-399"><a href="#DataBased-399"><span class="linenos">399</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="DataBased-400"><a href="#DataBased-400"><span class="linenos">400</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="DataBased-401"><a href="#DataBased-401"><span class="linenos">401</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="DataBased-402"><a href="#DataBased-402"><span class="linenos">402</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="DataBased-403"><a href="#DataBased-403"><span class="linenos">403</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="DataBased-404"><a href="#DataBased-404"><span class="linenos">404</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="DataBased-405"><a href="#DataBased-405"><span class="linenos">405</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DataBased-406"><a href="#DataBased-406"><span class="linenos">406</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-407"><a href="#DataBased-407"><span class="linenos">407</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased-408"><a href="#DataBased-408"><span class="linenos">408</span></a>
+</span><span id="DataBased-409"><a href="#DataBased-409"><span class="linenos">409</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-410"><a href="#DataBased-410"><span class="linenos">410</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="DataBased-411"><a href="#DataBased-411"><span class="linenos">411</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-412"><a href="#DataBased-412"><span class="linenos">412</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="DataBased-413"><a href="#DataBased-413"><span class="linenos">413</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
 </span><span id="DataBased-414"><a href="#DataBased-414"><span class="linenos">414</span></a>
-</span><span id="DataBased-415"><a href="#DataBased-415"><span class="linenos">415</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="DataBased-415"><a href="#DataBased-415"><span class="linenos">415</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased-416"><a href="#DataBased-416"><span class="linenos">416</span></a>
-</span><span id="DataBased-417"><a href="#DataBased-417"><span class="linenos">417</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
-</span><span id="DataBased-418"><a href="#DataBased-418"><span class="linenos">418</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="DataBased-419"><a href="#DataBased-419"><span class="linenos">419</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-420"><a href="#DataBased-420"><span class="linenos">420</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-421"><a href="#DataBased-421"><span class="linenos">421</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="DataBased-422"><a href="#DataBased-422"><span class="linenos">422</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased-423"><a href="#DataBased-423"><span class="linenos">423</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-424"><a href="#DataBased-424"><span class="linenos">424</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DataBased-425"><a href="#DataBased-425"><span class="linenos">425</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased-426"><a href="#DataBased-426"><span class="linenos">426</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="DataBased-427"><a href="#DataBased-427"><span class="linenos">427</span></a>                <span class="p">[</span>
-</span><span id="DataBased-428"><a href="#DataBased-428"><span class="linenos">428</span></a>                    <span class="n">row</span>
-</span><span id="DataBased-429"><a href="#DataBased-429"><span class="linenos">429</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DataBased-430"><a href="#DataBased-430"><span class="linenos">430</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="DataBased-431"><a href="#DataBased-431"><span class="linenos">431</span></a>                    <span class="p">)</span>
-</span><span id="DataBased-432"><a href="#DataBased-432"><span class="linenos">432</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="DataBased-433"><a href="#DataBased-433"><span class="linenos">433</span></a>                <span class="p">]</span>
-</span><span id="DataBased-434"><a href="#DataBased-434"><span class="linenos">434</span></a>            <span class="p">)</span>
-</span><span id="DataBased-435"><a href="#DataBased-435"><span class="linenos">435</span></a>        <span class="k">return</span> <span class="n">results</span>
-</span><span id="DataBased-436"><a href="#DataBased-436"><span class="linenos">436</span></a>
-</span><span id="DataBased-437"><a href="#DataBased-437"><span class="linenos">437</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-438"><a href="#DataBased-438"><span class="linenos">438</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="DataBased-439"><a href="#DataBased-439"><span class="linenos">439</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-440"><a href="#DataBased-440"><span class="linenos">440</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased-441"><a href="#DataBased-441"><span class="linenos">441</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
-</span><span id="DataBased-442"><a href="#DataBased-442"><span class="linenos">442</span></a>
-</span><span id="DataBased-443"><a href="#DataBased-443"><span class="linenos">443</span></a><span class="sd">        Returns the number of deleted records.</span>
-</span><span id="DataBased-444"><a href="#DataBased-444"><span class="linenos">444</span></a>
-</span><span id="DataBased-445"><a href="#DataBased-445"><span class="linenos">445</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-417"><a href="#DataBased-417"><span class="linenos">417</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="DataBased-418"><a href="#DataBased-418"><span class="linenos">418</span></a>
+</span><span id="DataBased-419"><a href="#DataBased-419"><span class="linenos">419</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="DataBased-420"><a href="#DataBased-420"><span class="linenos">420</span></a>
+</span><span id="DataBased-421"><a href="#DataBased-421"><span class="linenos">421</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
+</span><span id="DataBased-422"><a href="#DataBased-422"><span class="linenos">422</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="DataBased-423"><a href="#DataBased-423"><span class="linenos">423</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-424"><a href="#DataBased-424"><span class="linenos">424</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-425"><a href="#DataBased-425"><span class="linenos">425</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="DataBased-426"><a href="#DataBased-426"><span class="linenos">426</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased-427"><a href="#DataBased-427"><span class="linenos">427</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-428"><a href="#DataBased-428"><span class="linenos">428</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DataBased-429"><a href="#DataBased-429"><span class="linenos">429</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased-430"><a href="#DataBased-430"><span class="linenos">430</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="DataBased-431"><a href="#DataBased-431"><span class="linenos">431</span></a>                <span class="p">[</span>
+</span><span id="DataBased-432"><a href="#DataBased-432"><span class="linenos">432</span></a>                    <span class="n">row</span>
+</span><span id="DataBased-433"><a href="#DataBased-433"><span class="linenos">433</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DataBased-434"><a href="#DataBased-434"><span class="linenos">434</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="DataBased-435"><a href="#DataBased-435"><span class="linenos">435</span></a>                    <span class="p">)</span>
+</span><span id="DataBased-436"><a href="#DataBased-436"><span class="linenos">436</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="DataBased-437"><a href="#DataBased-437"><span class="linenos">437</span></a>                <span class="p">]</span>
+</span><span id="DataBased-438"><a href="#DataBased-438"><span class="linenos">438</span></a>            <span class="p">)</span>
+</span><span id="DataBased-439"><a href="#DataBased-439"><span class="linenos">439</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased-440"><a href="#DataBased-440"><span class="linenos">440</span></a>
+</span><span id="DataBased-441"><a href="#DataBased-441"><span class="linenos">441</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-442"><a href="#DataBased-442"><span class="linenos">442</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="DataBased-443"><a href="#DataBased-443"><span class="linenos">443</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-444"><a href="#DataBased-444"><span class="linenos">444</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-445"><a href="#DataBased-445"><span class="linenos">445</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
 </span><span id="DataBased-446"><a href="#DataBased-446"><span class="linenos">446</span></a>
-</span><span id="DataBased-447"><a href="#DataBased-447"><span class="linenos">447</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
-</span><span id="DataBased-448"><a href="#DataBased-448"><span class="linenos">448</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
-</span><span id="DataBased-449"><a href="#DataBased-449"><span class="linenos">449</span></a>
-</span><span id="DataBased-450"><a href="#DataBased-450"><span class="linenos">450</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
-</span><span id="DataBased-451"><a href="#DataBased-451"><span class="linenos">451</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-452"><a href="#DataBased-452"><span class="linenos">452</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased-453"><a href="#DataBased-453"><span class="linenos">453</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
-</span><span id="DataBased-455"><a href="#DataBased-455"><span class="linenos">455</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
-</span><span id="DataBased-456"><a href="#DataBased-456"><span class="linenos">456</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-457"><a href="#DataBased-457"><span class="linenos">457</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="DataBased-458"><a href="#DataBased-458"><span class="linenos">458</span></a>            <span class="p">)</span>
-</span><span id="DataBased-459"><a href="#DataBased-459"><span class="linenos">459</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
-</span><span id="DataBased-460"><a href="#DataBased-460"><span class="linenos">460</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-461"><a href="#DataBased-461"><span class="linenos">461</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
-</span><span id="DataBased-462"><a href="#DataBased-462"><span class="linenos">462</span></a>                <span class="sa">f</span><span class="s1">&#39;Error deleting rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased-463"><a href="#DataBased-463"><span class="linenos">463</span></a>            <span class="p">)</span>
-</span><span id="DataBased-464"><a href="#DataBased-464"><span class="linenos">464</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="DataBased-465"><a href="#DataBased-465"><span class="linenos">465</span></a>
-</span><span id="DataBased-466"><a href="#DataBased-466"><span class="linenos">466</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-467"><a href="#DataBased-467"><span class="linenos">467</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="DataBased-468"><a href="#DataBased-468"><span class="linenos">468</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased-469"><a href="#DataBased-469"><span class="linenos">469</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-470"><a href="#DataBased-470"><span class="linenos">470</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased-471"><a href="#DataBased-471"><span class="linenos">471</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="DataBased-472"><a href="#DataBased-472"><span class="linenos">472</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased-473"><a href="#DataBased-473"><span class="linenos">473</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased-474"><a href="#DataBased-474"><span class="linenos">474</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased-475"><a href="#DataBased-475"><span class="linenos">475</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
-</span><span id="DataBased-476"><a href="#DataBased-476"><span class="linenos">476</span></a>
-</span><span id="DataBased-477"><a href="#DataBased-477"><span class="linenos">477</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased-478"><a href="#DataBased-478"><span class="linenos">478</span></a>
-</span><span id="DataBased-479"><a href="#DataBased-479"><span class="linenos">479</span></a><span class="sd">        `table`: The table to update rows in.</span>
+</span><span id="DataBased-447"><a href="#DataBased-447"><span class="linenos">447</span></a><span class="sd">        Returns the number of deleted records.</span>
+</span><span id="DataBased-448"><a href="#DataBased-448"><span class="linenos">448</span></a>
+</span><span id="DataBased-449"><a href="#DataBased-449"><span class="linenos">449</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-450"><a href="#DataBased-450"><span class="linenos">450</span></a>
+</span><span id="DataBased-451"><a href="#DataBased-451"><span class="linenos">451</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
+</span><span id="DataBased-452"><a href="#DataBased-452"><span class="linenos">452</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased-453"><a href="#DataBased-453"><span class="linenos">453</span></a>
+</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
+</span><span id="DataBased-455"><a href="#DataBased-455"><span class="linenos">455</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased-456"><a href="#DataBased-456"><span class="linenos">456</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased-457"><a href="#DataBased-457"><span class="linenos">457</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-458"><a href="#DataBased-458"><span class="linenos">458</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-459"><a href="#DataBased-459"><span class="linenos">459</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
+</span><span id="DataBased-460"><a href="#DataBased-460"><span class="linenos">460</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-461"><a href="#DataBased-461"><span class="linenos">461</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="DataBased-462"><a href="#DataBased-462"><span class="linenos">462</span></a>            <span class="p">)</span>
+</span><span id="DataBased-463"><a href="#DataBased-463"><span class="linenos">463</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
+</span><span id="DataBased-464"><a href="#DataBased-464"><span class="linenos">464</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-465"><a href="#DataBased-465"><span class="linenos">465</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
+</span><span id="DataBased-466"><a href="#DataBased-466"><span class="linenos">466</span></a>                <span class="sa">f</span><span class="s1">&#39;Error deleting rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-467"><a href="#DataBased-467"><span class="linenos">467</span></a>            <span class="p">)</span>
+</span><span id="DataBased-468"><a href="#DataBased-468"><span class="linenos">468</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased-469"><a href="#DataBased-469"><span class="linenos">469</span></a>
+</span><span id="DataBased-470"><a href="#DataBased-470"><span class="linenos">470</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-471"><a href="#DataBased-471"><span class="linenos">471</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="DataBased-472"><a href="#DataBased-472"><span class="linenos">472</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased-473"><a href="#DataBased-473"><span class="linenos">473</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-474"><a href="#DataBased-474"><span class="linenos">474</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased-475"><a href="#DataBased-475"><span class="linenos">475</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="DataBased-476"><a href="#DataBased-476"><span class="linenos">476</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased-477"><a href="#DataBased-477"><span class="linenos">477</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased-478"><a href="#DataBased-478"><span class="linenos">478</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased-479"><a href="#DataBased-479"><span class="linenos">479</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
 </span><span id="DataBased-480"><a href="#DataBased-480"><span class="linenos">480</span></a>
-</span><span id="DataBased-481"><a href="#DataBased-481"><span class="linenos">481</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
+</span><span id="DataBased-481"><a href="#DataBased-481"><span class="linenos">481</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased-482"><a href="#DataBased-482"><span class="linenos">482</span></a>
-</span><span id="DataBased-483"><a href="#DataBased-483"><span class="linenos">483</span></a><span class="sd">        `new_value`: The new value to insert.</span>
+</span><span id="DataBased-483"><a href="#DataBased-483"><span class="linenos">483</span></a><span class="sd">        `table`: The table to update rows in.</span>
 </span><span id="DataBased-484"><a href="#DataBased-484"><span class="linenos">484</span></a>
-</span><span id="DataBased-485"><a href="#DataBased-485"><span class="linenos">485</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
-</span><span id="DataBased-486"><a href="#DataBased-486"><span class="linenos">486</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
-</span><span id="DataBased-487"><a href="#DataBased-487"><span class="linenos">487</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="DataBased-485"><a href="#DataBased-485"><span class="linenos">485</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
+</span><span id="DataBased-486"><a href="#DataBased-486"><span class="linenos">486</span></a>
+</span><span id="DataBased-487"><a href="#DataBased-487"><span class="linenos">487</span></a><span class="sd">        `new_value`: The new value to insert.</span>
 </span><span id="DataBased-488"><a href="#DataBased-488"><span class="linenos">488</span></a>
-</span><span id="DataBased-489"><a href="#DataBased-489"><span class="linenos">489</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
-</span><span id="DataBased-490"><a href="#DataBased-490"><span class="linenos">490</span></a>
-</span><span id="DataBased-491"><a href="#DataBased-491"><span class="linenos">491</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
-</span><span id="DataBased-492"><a href="#DataBased-492"><span class="linenos">492</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="DataBased-493"><a href="#DataBased-493"><span class="linenos">493</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="DataBased-494"><a href="#DataBased-494"><span class="linenos">494</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased-495"><a href="#DataBased-495"><span class="linenos">495</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased-496"><a href="#DataBased-496"><span class="linenos">496</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased-497"><a href="#DataBased-497"><span class="linenos">497</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-498"><a href="#DataBased-498"><span class="linenos">498</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-499"><a href="#DataBased-499"><span class="linenos">499</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased-500"><a href="#DataBased-500"><span class="linenos">500</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-501"><a href="#DataBased-501"><span class="linenos">501</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-502"><a href="#DataBased-502"><span class="linenos">502</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="DataBased-503"><a href="#DataBased-503"><span class="linenos">503</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="DataBased-504"><a href="#DataBased-504"><span class="linenos">504</span></a>            <span class="p">)</span>
-</span><span id="DataBased-505"><a href="#DataBased-505"><span class="linenos">505</span></a>            <span class="n">num_updates</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
-</span><span id="DataBased-506"><a href="#DataBased-506"><span class="linenos">506</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased-507"><a href="#DataBased-507"><span class="linenos">507</span></a>                <span class="sa">f</span><span class="s1">&#39;In </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s1"> rows, updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-489"><a href="#DataBased-489"><span class="linenos">489</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
+</span><span id="DataBased-490"><a href="#DataBased-490"><span class="linenos">490</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased-491"><a href="#DataBased-491"><span class="linenos">491</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="DataBased-492"><a href="#DataBased-492"><span class="linenos">492</span></a>
+</span><span id="DataBased-493"><a href="#DataBased-493"><span class="linenos">493</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
+</span><span id="DataBased-494"><a href="#DataBased-494"><span class="linenos">494</span></a>
+</span><span id="DataBased-495"><a href="#DataBased-495"><span class="linenos">495</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
+</span><span id="DataBased-496"><a href="#DataBased-496"><span class="linenos">496</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased-497"><a href="#DataBased-497"><span class="linenos">497</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="DataBased-498"><a href="#DataBased-498"><span class="linenos">498</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased-499"><a href="#DataBased-499"><span class="linenos">499</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased-500"><a href="#DataBased-500"><span class="linenos">500</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-501"><a href="#DataBased-501"><span class="linenos">501</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-502"><a href="#DataBased-502"><span class="linenos">502</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-503"><a href="#DataBased-503"><span class="linenos">503</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased-504"><a href="#DataBased-504"><span class="linenos">504</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-505"><a href="#DataBased-505"><span class="linenos">505</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-506"><a href="#DataBased-506"><span class="linenos">506</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="DataBased-507"><a href="#DataBased-507"><span class="linenos">507</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
 </span><span id="DataBased-508"><a href="#DataBased-508"><span class="linenos">508</span></a>            <span class="p">)</span>
-</span><span id="DataBased-509"><a href="#DataBased-509"><span class="linenos">509</span></a>            <span class="k">return</span> <span class="n">num_updates</span>
-</span><span id="DataBased-510"><a href="#DataBased-510"><span class="linenos">510</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-511"><a href="#DataBased-511"><span class="linenos">511</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased-512"><a href="#DataBased-512"><span class="linenos">512</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased-513"><a href="#DataBased-513"><span class="linenos">513</span></a>            <span class="p">)</span>
-</span><span id="DataBased-514"><a href="#DataBased-514"><span class="linenos">514</span></a>            <span class="k">return</span> <span class="mi">0</span>
-</span><span id="DataBased-515"><a href="#DataBased-515"><span class="linenos">515</span></a>
-</span><span id="DataBased-516"><a href="#DataBased-516"><span class="linenos">516</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-517"><a href="#DataBased-517"><span class="linenos">517</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased-518"><a href="#DataBased-518"><span class="linenos">518</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="DataBased-509"><a href="#DataBased-509"><span class="linenos">509</span></a>            <span class="n">num_updates</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
+</span><span id="DataBased-510"><a href="#DataBased-510"><span class="linenos">510</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased-511"><a href="#DataBased-511"><span class="linenos">511</span></a>                <span class="sa">f</span><span class="s1">&#39;In </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s1"> rows, updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-512"><a href="#DataBased-512"><span class="linenos">512</span></a>            <span class="p">)</span>
+</span><span id="DataBased-513"><a href="#DataBased-513"><span class="linenos">513</span></a>            <span class="k">return</span> <span class="n">num_updates</span>
+</span><span id="DataBased-514"><a href="#DataBased-514"><span class="linenos">514</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-515"><a href="#DataBased-515"><span class="linenos">515</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="DataBased-516"><a href="#DataBased-516"><span class="linenos">516</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased-517"><a href="#DataBased-517"><span class="linenos">517</span></a>            <span class="p">)</span>
+</span><span id="DataBased-518"><a href="#DataBased-518"><span class="linenos">518</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span><span id="DataBased-519"><a href="#DataBased-519"><span class="linenos">519</span></a>
-</span><span id="DataBased-520"><a href="#DataBased-520"><span class="linenos">520</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased-521"><a href="#DataBased-521"><span class="linenos">521</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-522"><a href="#DataBased-522"><span class="linenos">522</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
-</span><span id="DataBased-523"><a href="#DataBased-523"><span class="linenos">523</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased-524"><a href="#DataBased-524"><span class="linenos">524</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased-525"><a href="#DataBased-525"><span class="linenos">525</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-526"><a href="#DataBased-526"><span class="linenos">526</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="DataBased-527"><a href="#DataBased-527"><span class="linenos">527</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased-528"><a href="#DataBased-528"><span class="linenos">528</span></a>            <span class="k">return</span> <span class="kc">False</span>
-</span><span id="DataBased-529"><a href="#DataBased-529"><span class="linenos">529</span></a>
-</span><span id="DataBased-530"><a href="#DataBased-530"><span class="linenos">530</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased-531"><a href="#DataBased-531"><span class="linenos">531</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="DataBased-532"><a href="#DataBased-532"><span class="linenos">532</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased-533"><a href="#DataBased-533"><span class="linenos">533</span></a>    <span class="p">):</span>
-</span><span id="DataBased-534"><a href="#DataBased-534"><span class="linenos">534</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
-</span><span id="DataBased-535"><a href="#DataBased-535"><span class="linenos">535</span></a>
-</span><span id="DataBased-536"><a href="#DataBased-536"><span class="linenos">536</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased-537"><a href="#DataBased-537"><span class="linenos">537</span></a>
-</span><span id="DataBased-538"><a href="#DataBased-538"><span class="linenos">538</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="DataBased-520"><a href="#DataBased-520"><span class="linenos">520</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-521"><a href="#DataBased-521"><span class="linenos">521</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased-522"><a href="#DataBased-522"><span class="linenos">522</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="DataBased-523"><a href="#DataBased-523"><span class="linenos">523</span></a>
+</span><span id="DataBased-524"><a href="#DataBased-524"><span class="linenos">524</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased-525"><a href="#DataBased-525"><span class="linenos">525</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-526"><a href="#DataBased-526"><span class="linenos">526</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
+</span><span id="DataBased-527"><a href="#DataBased-527"><span class="linenos">527</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased-528"><a href="#DataBased-528"><span class="linenos">528</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased-529"><a href="#DataBased-529"><span class="linenos">529</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-530"><a href="#DataBased-530"><span class="linenos">530</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="DataBased-531"><a href="#DataBased-531"><span class="linenos">531</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased-532"><a href="#DataBased-532"><span class="linenos">532</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased-533"><a href="#DataBased-533"><span class="linenos">533</span></a>
+</span><span id="DataBased-534"><a href="#DataBased-534"><span class="linenos">534</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased-535"><a href="#DataBased-535"><span class="linenos">535</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="DataBased-536"><a href="#DataBased-536"><span class="linenos">536</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased-537"><a href="#DataBased-537"><span class="linenos">537</span></a>    <span class="p">):</span>
+</span><span id="DataBased-538"><a href="#DataBased-538"><span class="linenos">538</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
 </span><span id="DataBased-539"><a href="#DataBased-539"><span class="linenos">539</span></a>
-</span><span id="DataBased-540"><a href="#DataBased-540"><span class="linenos">540</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="DataBased-540"><a href="#DataBased-540"><span class="linenos">540</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased-541"><a href="#DataBased-541"><span class="linenos">541</span></a>
-</span><span id="DataBased-542"><a href="#DataBased-542"><span class="linenos">542</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="DataBased-543"><a href="#DataBased-543"><span class="linenos">543</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-544"><a href="#DataBased-544"><span class="linenos">544</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="DataBased-545"><a href="#DataBased-545"><span class="linenos">545</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-546"><a href="#DataBased-546"><span class="linenos">546</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DataBased-547"><a href="#DataBased-547"><span class="linenos">547</span></a>                <span class="p">)</span>
-</span><span id="DataBased-548"><a href="#DataBased-548"><span class="linenos">548</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
-</span><span id="DataBased-549"><a href="#DataBased-549"><span class="linenos">549</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-550"><a href="#DataBased-550"><span class="linenos">550</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-551"><a href="#DataBased-551"><span class="linenos">551</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DataBased-552"><a href="#DataBased-552"><span class="linenos">552</span></a>                <span class="p">)</span>
-</span><span id="DataBased-553"><a href="#DataBased-553"><span class="linenos">553</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-554"><a href="#DataBased-554"><span class="linenos">554</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-555"><a href="#DataBased-555"><span class="linenos">555</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-556"><a href="#DataBased-556"><span class="linenos">556</span></a>
-</span><span id="DataBased-557"><a href="#DataBased-557"><span class="linenos">557</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased-558"><a href="#DataBased-558"><span class="linenos">558</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased-559"><a href="#DataBased-559"><span class="linenos">559</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-560"><a href="#DataBased-560"><span class="linenos">560</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-561"><a href="#DataBased-561"><span class="linenos">561</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="DataBased-562"><a href="#DataBased-562"><span class="linenos">562</span></a>
-</span><span id="DataBased-563"><a href="#DataBased-563"><span class="linenos">563</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased-564"><a href="#DataBased-564"><span class="linenos">564</span></a>
-</span><span id="DataBased-565"><a href="#DataBased-565"><span class="linenos">565</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="DataBased-566"><a href="#DataBased-566"><span class="linenos">566</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased-567"><a href="#DataBased-567"><span class="linenos">567</span></a>
-</span><span id="DataBased-568"><a href="#DataBased-568"><span class="linenos">568</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
-</span><span id="DataBased-569"><a href="#DataBased-569"><span class="linenos">569</span></a>
-</span><span id="DataBased-570"><a href="#DataBased-570"><span class="linenos">570</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="DataBased-571"><a href="#DataBased-571"><span class="linenos">571</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="DataBased-572"><a href="#DataBased-572"><span class="linenos">572</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="DataBased-542"><a href="#DataBased-542"><span class="linenos">542</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="DataBased-543"><a href="#DataBased-543"><span class="linenos">543</span></a>
+</span><span id="DataBased-544"><a href="#DataBased-544"><span class="linenos">544</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="DataBased-545"><a href="#DataBased-545"><span class="linenos">545</span></a>
+</span><span id="DataBased-546"><a href="#DataBased-546"><span class="linenos">546</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="DataBased-547"><a href="#DataBased-547"><span class="linenos">547</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased-548"><a href="#DataBased-548"><span class="linenos">548</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="DataBased-549"><a href="#DataBased-549"><span class="linenos">549</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-550"><a href="#DataBased-550"><span class="linenos">550</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased-551"><a href="#DataBased-551"><span class="linenos">551</span></a>                <span class="p">)</span>
+</span><span id="DataBased-552"><a href="#DataBased-552"><span class="linenos">552</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
+</span><span id="DataBased-553"><a href="#DataBased-553"><span class="linenos">553</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased-554"><a href="#DataBased-554"><span class="linenos">554</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-555"><a href="#DataBased-555"><span class="linenos">555</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased-556"><a href="#DataBased-556"><span class="linenos">556</span></a>                <span class="p">)</span>
+</span><span id="DataBased-557"><a href="#DataBased-557"><span class="linenos">557</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-558"><a href="#DataBased-558"><span class="linenos">558</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-559"><a href="#DataBased-559"><span class="linenos">559</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-560"><a href="#DataBased-560"><span class="linenos">560</span></a>
+</span><span id="DataBased-561"><a href="#DataBased-561"><span class="linenos">561</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased-562"><a href="#DataBased-562"><span class="linenos">562</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased-563"><a href="#DataBased-563"><span class="linenos">563</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-564"><a href="#DataBased-564"><span class="linenos">564</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-565"><a href="#DataBased-565"><span class="linenos">565</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="DataBased-566"><a href="#DataBased-566"><span class="linenos">566</span></a>
+</span><span id="DataBased-567"><a href="#DataBased-567"><span class="linenos">567</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-568"><a href="#DataBased-568"><span class="linenos">568</span></a>
+</span><span id="DataBased-569"><a href="#DataBased-569"><span class="linenos">569</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="DataBased-570"><a href="#DataBased-570"><span class="linenos">570</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="DataBased-571"><a href="#DataBased-571"><span class="linenos">571</span></a>
+</span><span id="DataBased-572"><a href="#DataBased-572"><span class="linenos">572</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased-573"><a href="#DataBased-573"><span class="linenos">573</span></a>
+</span><span id="DataBased-574"><a href="#DataBased-574"><span class="linenos">574</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="DataBased-575"><a href="#DataBased-575"><span class="linenos">575</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="DataBased-576"><a href="#DataBased-576"><span class="linenos">576</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sqli wrapper so queries don't need to be written except table definitions.</p>
 
 <p>Supports saving and reading dates as datetime objects.</p>
 
@@ -1385,27 +1393,33 @@
 
                             </div>
                             <div id="DataBased.vacuum" class="classattr">
                                         <input id="DataBased.vacuum-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">vacuum</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
+        <span class="name">vacuum</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.vacuum-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.vacuum"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.vacuum-190"><a href="#DataBased.vacuum-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DataBased.vacuum-191"><a href="#DataBased.vacuum-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.&quot;&quot;&quot;</span>
-</span><span id="DataBased.vacuum-192"><a href="#DataBased.vacuum-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.vacuum-190"><a href="#DataBased.vacuum-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.vacuum-191"><a href="#DataBased.vacuum-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.</span>
+</span><span id="DataBased.vacuum-192"><a href="#DataBased.vacuum-192"><span class="linenos">192</span></a>
+</span><span id="DataBased.vacuum-193"><a href="#DataBased.vacuum-193"><span class="linenos">193</span></a><span class="sd">        Returns space freed up in bytes.&quot;&quot;&quot;</span>
+</span><span id="DataBased.vacuum-194"><a href="#DataBased.vacuum-194"><span class="linenos">194</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="DataBased.vacuum-195"><a href="#DataBased.vacuum-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.vacuum-196"><a href="#DataBased.vacuum-196"><span class="linenos">196</span></a>        <span class="k">return</span> <span class="n">size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Reduce disk size of the database with a <code>VACUUM</code> query.</p>
+
+<p>Returns space freed up in bytes.</p>
 </div>
 
 
                             </div>
                             <div id="DataBased.query" class="classattr">
                                         <input id="DataBased.query-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1413,19 +1427,19 @@
         <span class="def">def</span>
         <span class="name">query</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">query_</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.query-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.query"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.query-194"><a href="#DataBased.query-194"><span class="linenos">194</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.query-195"><a href="#DataBased.query-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="DataBased.query-196"><a href="#DataBased.query-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
-</span><span id="DataBased.query-197"><a href="#DataBased.query-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
-</span><span id="DataBased.query-198"><a href="#DataBased.query-198"><span class="linenos">198</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.query-198"><a href="#DataBased.query-198"><span class="linenos">198</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.query-199"><a href="#DataBased.query-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="DataBased.query-200"><a href="#DataBased.query-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
+</span><span id="DataBased.query-201"><a href="#DataBased.query-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
+</span><span id="DataBased.query-202"><a href="#DataBased.query-202"><span class="linenos">202</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute an arbitrary query and return the results.</p>
 </div>
 
 
@@ -1437,25 +1451,25 @@
         <span class="def">def</span>
         <span class="name">create_tables</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.create_tables-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.create_tables"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_tables-200"><a href="#DataBased.create_tables-200"><span class="linenos">200</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.create_tables-201"><a href="#DataBased.create_tables-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
-</span><span id="DataBased.create_tables-202"><a href="#DataBased.create_tables-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
-</span><span id="DataBased.create_tables-203"><a href="#DataBased.create_tables-203"><span class="linenos">203</span></a>
-</span><span id="DataBased.create_tables-204"><a href="#DataBased.create_tables-204"><span class="linenos">204</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
-</span><span id="DataBased.create_tables-205"><a href="#DataBased.create_tables-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-206"><a href="#DataBased.create_tables-206"><span class="linenos">206</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DataBased.create_tables-207"><a href="#DataBased.create_tables-207"><span class="linenos">207</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-208"><a href="#DataBased.create_tables-208"><span class="linenos">208</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-209"><a href="#DataBased.create_tables-209"><span class="linenos">209</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
-</span><span id="DataBased.create_tables-210"><a href="#DataBased.create_tables-210"><span class="linenos">210</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_tables-204"><a href="#DataBased.create_tables-204"><span class="linenos">204</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.create_tables-205"><a href="#DataBased.create_tables-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">create_tables</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]):</span>
+</span><span id="DataBased.create_tables-206"><a href="#DataBased.create_tables-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
+</span><span id="DataBased.create_tables-207"><a href="#DataBased.create_tables-207"><span class="linenos">207</span></a>
+</span><span id="DataBased.create_tables-208"><a href="#DataBased.create_tables-208"><span class="linenos">208</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
+</span><span id="DataBased.create_tables-209"><a href="#DataBased.create_tables-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-210"><a href="#DataBased.create_tables-210"><span class="linenos">210</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DataBased.create_tables-211"><a href="#DataBased.create_tables-211"><span class="linenos">211</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-212"><a href="#DataBased.create_tables-212"><span class="linenos">212</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
+</span><span id="DataBased.create_tables-213"><a href="#DataBased.create_tables-213"><span class="linenos">213</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
+</span><span id="DataBased.create_tables-214"><a href="#DataBased.create_tables-214"><span class="linenos">214</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create tables if they don't exist.</p>
 
 <h6 id="parameters">Parameters</h6>
 
@@ -1473,28 +1487,28 @@
         <span class="def">def</span>
         <span class="name">create_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.create_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.create_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_table-212"><a href="#DataBased.create_table-212"><span class="linenos">212</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.create_table-213"><a href="#DataBased.create_table-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="DataBased.create_table-214"><a href="#DataBased.create_table-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
-</span><span id="DataBased.create_table-215"><a href="#DataBased.create_table-215"><span class="linenos">215</span></a>
-</span><span id="DataBased.create_table-216"><a href="#DataBased.create_table-216"><span class="linenos">216</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased.create_table-217"><a href="#DataBased.create_table-217"><span class="linenos">217</span></a>
-</span><span id="DataBased.create_table-218"><a href="#DataBased.create_table-218"><span class="linenos">218</span></a><span class="sd">        `table`: Name of the table to create.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.create_table-216"><a href="#DataBased.create_table-216"><span class="linenos">216</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.create_table-217"><a href="#DataBased.create_table-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="DataBased.create_table-218"><a href="#DataBased.create_table-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
 </span><span id="DataBased.create_table-219"><a href="#DataBased.create_table-219"><span class="linenos">219</span></a>
-</span><span id="DataBased.create_table-220"><a href="#DataBased.create_table-220"><span class="linenos">220</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
-</span><span id="DataBased.create_table-221"><a href="#DataBased.create_table-221"><span class="linenos">221</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
-</span><span id="DataBased.create_table-222"><a href="#DataBased.create_table-222"><span class="linenos">222</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased.create_table-223"><a href="#DataBased.create_table-223"><span class="linenos">223</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
-</span><span id="DataBased.create_table-224"><a href="#DataBased.create_table-224"><span class="linenos">224</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased.create_table-225"><a href="#DataBased.create_table-225"><span class="linenos">225</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
+</span><span id="DataBased.create_table-220"><a href="#DataBased.create_table-220"><span class="linenos">220</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.create_table-221"><a href="#DataBased.create_table-221"><span class="linenos">221</span></a>
+</span><span id="DataBased.create_table-222"><a href="#DataBased.create_table-222"><span class="linenos">222</span></a><span class="sd">        `table`: Name of the table to create.</span>
+</span><span id="DataBased.create_table-223"><a href="#DataBased.create_table-223"><span class="linenos">223</span></a>
+</span><span id="DataBased.create_table-224"><a href="#DataBased.create_table-224"><span class="linenos">224</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
+</span><span id="DataBased.create_table-225"><a href="#DataBased.create_table-225"><span class="linenos">225</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
+</span><span id="DataBased.create_table-226"><a href="#DataBased.create_table-226"><span class="linenos">226</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
+</span><span id="DataBased.create_table-227"><a href="#DataBased.create_table-227"><span class="linenos">227</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="DataBased.create_table-228"><a href="#DataBased.create_table-228"><span class="linenos">228</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased.create_table-229"><a href="#DataBased.create_table-229"><span class="linenos">229</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a table if it doesn't exist.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1513,21 +1527,21 @@
         <span class="def">def</span>
         <span class="name">get_table_names</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_table_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_table_names"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_table_names-227"><a href="#DataBased.get_table_names-227"><span class="linenos">227</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_table_names-228"><a href="#DataBased.get_table_names-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased.get_table_names-229"><a href="#DataBased.get_table_names-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
-</span><span id="DataBased.get_table_names-230"><a href="#DataBased.get_table_names-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.get_table_names-231"><a href="#DataBased.get_table_names-231"><span class="linenos">231</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
-</span><span id="DataBased.get_table_names-232"><a href="#DataBased.get_table_names-232"><span class="linenos">232</span></a>        <span class="p">)</span>
-</span><span id="DataBased.get_table_names-233"><a href="#DataBased.get_table_names-233"><span class="linenos">233</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_table_names-231"><a href="#DataBased.get_table_names-231"><span class="linenos">231</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_table_names-232"><a href="#DataBased.get_table_names-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased.get_table_names-233"><a href="#DataBased.get_table_names-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
+</span><span id="DataBased.get_table_names-234"><a href="#DataBased.get_table_names-234"><span class="linenos">234</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.get_table_names-235"><a href="#DataBased.get_table_names-235"><span class="linenos">235</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
+</span><span id="DataBased.get_table_names-236"><a href="#DataBased.get_table_names-236"><span class="linenos">236</span></a>        <span class="p">)</span>
+</span><span id="DataBased.get_table_names-237"><a href="#DataBased.get_table_names-237"><span class="linenos">237</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns a list of table names from the database.</p>
 </div>
 
 
@@ -1539,19 +1553,19 @@
         <span class="def">def</span>
         <span class="name">get_column_names</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_column_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_column_names"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_column_names-235"><a href="#DataBased.get_column_names-235"><span class="linenos">235</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_column_names-236"><a href="#DataBased.get_column_names-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="DataBased.get_column_names-237"><a href="#DataBased.get_column_names-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased.get_column_names-238"><a href="#DataBased.get_column_names-238"><span class="linenos">238</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
-</span><span id="DataBased.get_column_names-239"><a href="#DataBased.get_column_names-239"><span class="linenos">239</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_column_names-239"><a href="#DataBased.get_column_names-239"><span class="linenos">239</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_column_names-240"><a href="#DataBased.get_column_names-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="DataBased.get_column_names-241"><a href="#DataBased.get_column_names-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
+</span><span id="DataBased.get_column_names-242"><a href="#DataBased.get_column_names-242"><span class="linenos">242</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.get_column_names-243"><a href="#DataBased.get_column_names-243"><span class="linenos">243</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a list of column names from a table.</p>
 </div>
 
 
@@ -1563,45 +1577,45 @@
         <span class="def">def</span>
         <span class="name">count</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.count-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.count"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.count-241"><a href="#DataBased.count-241"><span class="linenos">241</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.count-242"><a href="#DataBased.count-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
-</span><span id="DataBased.count-243"><a href="#DataBased.count-243"><span class="linenos">243</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.count-244"><a href="#DataBased.count-244"><span class="linenos">244</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.count-245"><a href="#DataBased.count-245"><span class="linenos">245</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.count-246"><a href="#DataBased.count-246"><span class="linenos">246</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased.count-247"><a href="#DataBased.count-247"><span class="linenos">247</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased.count-248"><a href="#DataBased.count-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
-</span><span id="DataBased.count-249"><a href="#DataBased.count-249"><span class="linenos">249</span></a>
-</span><span id="DataBased.count-250"><a href="#DataBased.count-250"><span class="linenos">250</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased.count-251"><a href="#DataBased.count-251"><span class="linenos">251</span></a>
-</span><span id="DataBased.count-252"><a href="#DataBased.count-252"><span class="linenos">252</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.count-253"><a href="#DataBased.count-253"><span class="linenos">253</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
-</span><span id="DataBased.count-254"><a href="#DataBased.count-254"><span class="linenos">254</span></a><span class="sd">        keys are column names and values are row values.</span>
-</span><span id="DataBased.count-255"><a href="#DataBased.count-255"><span class="linenos">255</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
-</span><span id="DataBased.count-256"><a href="#DataBased.count-256"><span class="linenos">256</span></a>
-</span><span id="DataBased.count-257"><a href="#DataBased.count-257"><span class="linenos">257</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
-</span><span id="DataBased.count-258"><a href="#DataBased.count-258"><span class="linenos">258</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
-</span><span id="DataBased.count-259"><a href="#DataBased.count-259"><span class="linenos">259</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
-</span><span id="DataBased.count-260"><a href="#DataBased.count-260"><span class="linenos">260</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.count-261"><a href="#DataBased.count-261"><span class="linenos">261</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
-</span><span id="DataBased.count-262"><a href="#DataBased.count-262"><span class="linenos">262</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.count-263"><a href="#DataBased.count-263"><span class="linenos">263</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.count-264"><a href="#DataBased.count-264"><span class="linenos">264</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.count-265"><a href="#DataBased.count-265"><span class="linenos">265</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DataBased.count-266"><a href="#DataBased.count-266"><span class="linenos">266</span></a>                <span class="p">)</span>
-</span><span id="DataBased.count-267"><a href="#DataBased.count-267"><span class="linenos">267</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.count-268"><a href="#DataBased.count-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DataBased.count-269"><a href="#DataBased.count-269"><span class="linenos">269</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DataBased.count-270"><a href="#DataBased.count-270"><span class="linenos">270</span></a>        <span class="k">except</span><span class="p">:</span>
-</span><span id="DataBased.count-271"><a href="#DataBased.count-271"><span class="linenos">271</span></a>            <span class="k">return</span> <span class="mi">0</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.count-245"><a href="#DataBased.count-245"><span class="linenos">245</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.count-246"><a href="#DataBased.count-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
+</span><span id="DataBased.count-247"><a href="#DataBased.count-247"><span class="linenos">247</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.count-248"><a href="#DataBased.count-248"><span class="linenos">248</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.count-249"><a href="#DataBased.count-249"><span class="linenos">249</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.count-250"><a href="#DataBased.count-250"><span class="linenos">250</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased.count-251"><a href="#DataBased.count-251"><span class="linenos">251</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.count-252"><a href="#DataBased.count-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Return number of items in `table`.</span>
+</span><span id="DataBased.count-253"><a href="#DataBased.count-253"><span class="linenos">253</span></a>
+</span><span id="DataBased.count-254"><a href="#DataBased.count-254"><span class="linenos">254</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.count-255"><a href="#DataBased.count-255"><span class="linenos">255</span></a>
+</span><span id="DataBased.count-256"><a href="#DataBased.count-256"><span class="linenos">256</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.count-257"><a href="#DataBased.count-257"><span class="linenos">257</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased.count-258"><a href="#DataBased.count-258"><span class="linenos">258</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased.count-259"><a href="#DataBased.count-259"><span class="linenos">259</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
+</span><span id="DataBased.count-260"><a href="#DataBased.count-260"><span class="linenos">260</span></a>
+</span><span id="DataBased.count-261"><a href="#DataBased.count-261"><span class="linenos">261</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
+</span><span id="DataBased.count-262"><a href="#DataBased.count-262"><span class="linenos">262</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
+</span><span id="DataBased.count-263"><a href="#DataBased.count-263"><span class="linenos">263</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
+</span><span id="DataBased.count-264"><a href="#DataBased.count-264"><span class="linenos">264</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.count-265"><a href="#DataBased.count-265"><span class="linenos">265</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
+</span><span id="DataBased.count-266"><a href="#DataBased.count-266"><span class="linenos">266</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.count-267"><a href="#DataBased.count-267"><span class="linenos">267</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.count-268"><a href="#DataBased.count-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.count-269"><a href="#DataBased.count-269"><span class="linenos">269</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased.count-270"><a href="#DataBased.count-270"><span class="linenos">270</span></a>                <span class="p">)</span>
+</span><span id="DataBased.count-271"><a href="#DataBased.count-271"><span class="linenos">271</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.count-272"><a href="#DataBased.count-272"><span class="linenos">272</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DataBased.count-273"><a href="#DataBased.count-273"><span class="linenos">273</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchone</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DataBased.count-274"><a href="#DataBased.count-274"><span class="linenos">274</span></a>        <span class="k">except</span><span class="p">:</span>
+</span><span id="DataBased.count-275"><a href="#DataBased.count-275"><span class="linenos">275</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return number of items in <code>table</code>.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1624,53 +1638,53 @@
         <span class="def">def</span>
         <span class="name">add_row</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.add_row-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.add_row"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_row-273"><a href="#DataBased.add_row-273"><span class="linenos">273</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.add_row-274"><a href="#DataBased.add_row-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
-</span><span id="DataBased.add_row-275"><a href="#DataBased.add_row-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.add_row-276"><a href="#DataBased.add_row-276"><span class="linenos">276</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased.add_row-277"><a href="#DataBased.add_row-277"><span class="linenos">277</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
-</span><span id="DataBased.add_row-278"><a href="#DataBased.add_row-278"><span class="linenos">278</span></a>
-</span><span id="DataBased.add_row-279"><a href="#DataBased.add_row-279"><span class="linenos">279</span></a><span class="sd">        Returns whether the addition was successful or not.</span>
-</span><span id="DataBased.add_row-280"><a href="#DataBased.add_row-280"><span class="linenos">280</span></a>
-</span><span id="DataBased.add_row-281"><a href="#DataBased.add_row-281"><span class="linenos">281</span></a><span class="sd">        #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_row-277"><a href="#DataBased.add_row-277"><span class="linenos">277</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.add_row-278"><a href="#DataBased.add_row-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">add_row</span><span class="p">(</span>
+</span><span id="DataBased.add_row-279"><a href="#DataBased.add_row-279"><span class="linenos">279</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.add_row-280"><a href="#DataBased.add_row-280"><span class="linenos">280</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased.add_row-281"><a href="#DataBased.add_row-281"><span class="linenos">281</span></a>        <span class="sd">&quot;&quot;&quot;Add a row of values to a table.</span>
 </span><span id="DataBased.add_row-282"><a href="#DataBased.add_row-282"><span class="linenos">282</span></a>
-</span><span id="DataBased.add_row-283"><a href="#DataBased.add_row-283"><span class="linenos">283</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased.add_row-283"><a href="#DataBased.add_row-283"><span class="linenos">283</span></a><span class="sd">        Returns whether the addition was successful or not.</span>
 </span><span id="DataBased.add_row-284"><a href="#DataBased.add_row-284"><span class="linenos">284</span></a>
-</span><span id="DataBased.add_row-285"><a href="#DataBased.add_row-285"><span class="linenos">285</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased.add_row-285"><a href="#DataBased.add_row-285"><span class="linenos">285</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased.add_row-286"><a href="#DataBased.add_row-286"><span class="linenos">286</span></a>
-</span><span id="DataBased.add_row-287"><a href="#DataBased.add_row-287"><span class="linenos">287</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
-</span><span id="DataBased.add_row-288"><a href="#DataBased.add_row-288"><span class="linenos">288</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
-</span><span id="DataBased.add_row-289"><a href="#DataBased.add_row-289"><span class="linenos">289</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased.add_row-290"><a href="#DataBased.add_row-290"><span class="linenos">290</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
-</span><span id="DataBased.add_row-291"><a href="#DataBased.add_row-291"><span class="linenos">291</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.add_row-292"><a href="#DataBased.add_row-292"><span class="linenos">292</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.add_row-293"><a href="#DataBased.add_row-293"><span class="linenos">293</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
-</span><span id="DataBased.add_row-294"><a href="#DataBased.add_row-294"><span class="linenos">294</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-295"><a href="#DataBased.add_row-295"><span class="linenos">295</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
-</span><span id="DataBased.add_row-296"><a href="#DataBased.add_row-296"><span class="linenos">296</span></a>                    <span class="n">values</span><span class="p">,</span>
-</span><span id="DataBased.add_row-297"><a href="#DataBased.add_row-297"><span class="linenos">297</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-298"><a href="#DataBased.add_row-298"><span class="linenos">298</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_row-299"><a href="#DataBased.add_row-299"><span class="linenos">299</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-300"><a href="#DataBased.add_row-300"><span class="linenos">300</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased.add_row-287"><a href="#DataBased.add_row-287"><span class="linenos">287</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased.add_row-288"><a href="#DataBased.add_row-288"><span class="linenos">288</span></a>
+</span><span id="DataBased.add_row-289"><a href="#DataBased.add_row-289"><span class="linenos">289</span></a><span class="sd">        `values`: A tuple of values to be inserted into the table.</span>
+</span><span id="DataBased.add_row-290"><a href="#DataBased.add_row-290"><span class="linenos">290</span></a>
+</span><span id="DataBased.add_row-291"><a href="#DataBased.add_row-291"><span class="linenos">291</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="DataBased.add_row-292"><a href="#DataBased.add_row-292"><span class="linenos">292</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="DataBased.add_row-293"><a href="#DataBased.add_row-293"><span class="linenos">293</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased.add_row-294"><a href="#DataBased.add_row-294"><span class="linenos">294</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
+</span><span id="DataBased.add_row-295"><a href="#DataBased.add_row-295"><span class="linenos">295</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.add_row-296"><a href="#DataBased.add_row-296"><span class="linenos">296</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.add_row-297"><a href="#DataBased.add_row-297"><span class="linenos">297</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
+</span><span id="DataBased.add_row-298"><a href="#DataBased.add_row-298"><span class="linenos">298</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_row-299"><a href="#DataBased.add_row-299"><span class="linenos">299</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="DataBased.add_row-300"><a href="#DataBased.add_row-300"><span class="linenos">300</span></a>                    <span class="n">values</span><span class="p">,</span>
 </span><span id="DataBased.add_row-301"><a href="#DataBased.add_row-301"><span class="linenos">301</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-302"><a href="#DataBased.add_row-302"><span class="linenos">302</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased.add_row-303"><a href="#DataBased.add_row-303"><span class="linenos">303</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased.add_row-304"><a href="#DataBased.add_row-304"><span class="linenos">304</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.add_row-305"><a href="#DataBased.add_row-305"><span class="linenos">305</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
-</span><span id="DataBased.add_row-306"><a href="#DataBased.add_row-306"><span class="linenos">306</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
-</span><span id="DataBased.add_row-307"><a href="#DataBased.add_row-307"><span class="linenos">307</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
-</span><span id="DataBased.add_row-308"><a href="#DataBased.add_row-308"><span class="linenos">308</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_row-309"><a href="#DataBased.add_row-309"><span class="linenos">309</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_row-310"><a href="#DataBased.add_row-310"><span class="linenos">310</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
-</span><span id="DataBased.add_row-311"><a href="#DataBased.add_row-311"><span class="linenos">311</span></a>            <span class="k">return</span> <span class="kc">False</span>
+</span><span id="DataBased.add_row-302"><a href="#DataBased.add_row-302"><span class="linenos">302</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_row-303"><a href="#DataBased.add_row-303"><span class="linenos">303</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_row-304"><a href="#DataBased.add_row-304"><span class="linenos">304</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased.add_row-305"><a href="#DataBased.add_row-305"><span class="linenos">305</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_row-306"><a href="#DataBased.add_row-306"><span class="linenos">306</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_row-307"><a href="#DataBased.add_row-307"><span class="linenos">307</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased.add_row-308"><a href="#DataBased.add_row-308"><span class="linenos">308</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.add_row-309"><a href="#DataBased.add_row-309"><span class="linenos">309</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
+</span><span id="DataBased.add_row-310"><a href="#DataBased.add_row-310"><span class="linenos">310</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
+</span><span id="DataBased.add_row-311"><a href="#DataBased.add_row-311"><span class="linenos">311</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
+</span><span id="DataBased.add_row-312"><a href="#DataBased.add_row-312"><span class="linenos">312</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_row-313"><a href="#DataBased.add_row-313"><span class="linenos">313</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_row-314"><a href="#DataBased.add_row-314"><span class="linenos">314</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">))</span>
+</span><span id="DataBased.add_row-315"><a href="#DataBased.add_row-315"><span class="linenos">315</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a row of values to a table.</p>
 
 <p>Returns whether the addition was successful or not.</p>
 
@@ -1693,39 +1707,39 @@
         <span class="def">def</span>
         <span class="name">add_rows</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]]</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.add_rows-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.add_rows"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_rows-313"><a href="#DataBased.add_rows-313"><span class="linenos">313</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.add_rows-314"><a href="#DataBased.add_rows-314"><span class="linenos">314</span></a>    <span class="k">def</span> <span class="nf">add_rows</span><span class="p">(</span>
-</span><span id="DataBased.add_rows-315"><a href="#DataBased.add_rows-315"><span class="linenos">315</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">]],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.add_rows-316"><a href="#DataBased.add_rows-316"><span class="linenos">316</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
-</span><span id="DataBased.add_rows-317"><a href="#DataBased.add_rows-317"><span class="linenos">317</span></a>        <span class="sd">&quot;&quot;&quot;Add multiple rows of values to a table.</span>
-</span><span id="DataBased.add_rows-318"><a href="#DataBased.add_rows-318"><span class="linenos">318</span></a>
-</span><span id="DataBased.add_rows-319"><a href="#DataBased.add_rows-319"><span class="linenos">319</span></a><span class="sd">        Returns a tuple containing the number of successful additions and the number of failed additions.</span>
-</span><span id="DataBased.add_rows-320"><a href="#DataBased.add_rows-320"><span class="linenos">320</span></a>
-</span><span id="DataBased.add_rows-321"><a href="#DataBased.add_rows-321"><span class="linenos">321</span></a><span class="sd">        #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_rows-317"><a href="#DataBased.add_rows-317"><span class="linenos">317</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.add_rows-318"><a href="#DataBased.add_rows-318"><span class="linenos">318</span></a>    <span class="k">def</span> <span class="nf">add_rows</span><span class="p">(</span>
+</span><span id="DataBased.add_rows-319"><a href="#DataBased.add_rows-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">values</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="n">Any</span><span class="p">]],</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.add_rows-320"><a href="#DataBased.add_rows-320"><span class="linenos">320</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">tuple</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">int</span><span class="p">]:</span>
+</span><span id="DataBased.add_rows-321"><a href="#DataBased.add_rows-321"><span class="linenos">321</span></a>        <span class="sd">&quot;&quot;&quot;Add multiple rows of values to a table.</span>
 </span><span id="DataBased.add_rows-322"><a href="#DataBased.add_rows-322"><span class="linenos">322</span></a>
-</span><span id="DataBased.add_rows-323"><a href="#DataBased.add_rows-323"><span class="linenos">323</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased.add_rows-323"><a href="#DataBased.add_rows-323"><span class="linenos">323</span></a><span class="sd">        Returns a tuple containing the number of successful additions and the number of failed additions.</span>
 </span><span id="DataBased.add_rows-324"><a href="#DataBased.add_rows-324"><span class="linenos">324</span></a>
-</span><span id="DataBased.add_rows-325"><a href="#DataBased.add_rows-325"><span class="linenos">325</span></a><span class="sd">        `values`: A list of tuples of values to be inserted into the table.</span>
-</span><span id="DataBased.add_rows-326"><a href="#DataBased.add_rows-326"><span class="linenos">326</span></a><span class="sd">        Each tuple constitutes a single row to be inserted</span>
-</span><span id="DataBased.add_rows-327"><a href="#DataBased.add_rows-327"><span class="linenos">327</span></a>
-</span><span id="DataBased.add_rows-328"><a href="#DataBased.add_rows-328"><span class="linenos">328</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
-</span><span id="DataBased.add_rows-329"><a href="#DataBased.add_rows-329"><span class="linenos">329</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
-</span><span id="DataBased.add_rows-330"><a href="#DataBased.add_rows-330"><span class="linenos">330</span></a>        <span class="n">successes</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="DataBased.add_rows-331"><a href="#DataBased.add_rows-331"><span class="linenos">331</span></a>        <span class="n">failures</span> <span class="o">=</span> <span class="mi">0</span>
-</span><span id="DataBased.add_rows-332"><a href="#DataBased.add_rows-332"><span class="linenos">332</span></a>        <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">values</span><span class="p">:</span>
-</span><span id="DataBased.add_rows-333"><a href="#DataBased.add_rows-333"><span class="linenos">333</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">row</span><span class="p">,</span> <span class="n">columns</span><span class="p">):</span>
-</span><span id="DataBased.add_rows-334"><a href="#DataBased.add_rows-334"><span class="linenos">334</span></a>                <span class="n">successes</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="DataBased.add_rows-335"><a href="#DataBased.add_rows-335"><span class="linenos">335</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_rows-336"><a href="#DataBased.add_rows-336"><span class="linenos">336</span></a>                <span class="n">failures</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="DataBased.add_rows-337"><a href="#DataBased.add_rows-337"><span class="linenos">337</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">successes</span><span class="p">,</span> <span class="n">failures</span><span class="p">)</span>
+</span><span id="DataBased.add_rows-325"><a href="#DataBased.add_rows-325"><span class="linenos">325</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.add_rows-326"><a href="#DataBased.add_rows-326"><span class="linenos">326</span></a>
+</span><span id="DataBased.add_rows-327"><a href="#DataBased.add_rows-327"><span class="linenos">327</span></a><span class="sd">        `table`: The table to insert values into.</span>
+</span><span id="DataBased.add_rows-328"><a href="#DataBased.add_rows-328"><span class="linenos">328</span></a>
+</span><span id="DataBased.add_rows-329"><a href="#DataBased.add_rows-329"><span class="linenos">329</span></a><span class="sd">        `values`: A list of tuples of values to be inserted into the table.</span>
+</span><span id="DataBased.add_rows-330"><a href="#DataBased.add_rows-330"><span class="linenos">330</span></a><span class="sd">        Each tuple constitutes a single row to be inserted</span>
+</span><span id="DataBased.add_rows-331"><a href="#DataBased.add_rows-331"><span class="linenos">331</span></a>
+</span><span id="DataBased.add_rows-332"><a href="#DataBased.add_rows-332"><span class="linenos">332</span></a><span class="sd">        `columns`: If `None`, `values` is expected to supply a value for every column in the table.</span>
+</span><span id="DataBased.add_rows-333"><a href="#DataBased.add_rows-333"><span class="linenos">333</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
+</span><span id="DataBased.add_rows-334"><a href="#DataBased.add_rows-334"><span class="linenos">334</span></a>        <span class="n">successes</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="DataBased.add_rows-335"><a href="#DataBased.add_rows-335"><span class="linenos">335</span></a>        <span class="n">failures</span> <span class="o">=</span> <span class="mi">0</span>
+</span><span id="DataBased.add_rows-336"><a href="#DataBased.add_rows-336"><span class="linenos">336</span></a>        <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">values</span><span class="p">:</span>
+</span><span id="DataBased.add_rows-337"><a href="#DataBased.add_rows-337"><span class="linenos">337</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_row</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">row</span><span class="p">,</span> <span class="n">columns</span><span class="p">):</span>
+</span><span id="DataBased.add_rows-338"><a href="#DataBased.add_rows-338"><span class="linenos">338</span></a>                <span class="n">successes</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="DataBased.add_rows-339"><a href="#DataBased.add_rows-339"><span class="linenos">339</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_rows-340"><a href="#DataBased.add_rows-340"><span class="linenos">340</span></a>                <span class="n">failures</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="DataBased.add_rows-341"><a href="#DataBased.add_rows-341"><span class="linenos">341</span></a>        <span class="k">return</span> <span class="p">(</span><span class="n">successes</span><span class="p">,</span> <span class="n">failures</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add multiple rows of values to a table.</p>
 
 <p>Returns a tuple containing the number of successful additions and the number of failed additions.</p>
 
@@ -1749,79 +1763,79 @@
         <span class="def">def</span>
         <span class="name">get_rows</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">core</span><span class="o">.</span><span class="n">frame</span><span class="o">.</span><span class="n">DataFrame</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.get_rows-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_rows"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_rows-339"><a href="#DataBased.get_rows-339"><span class="linenos">339</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.get_rows-340"><a href="#DataBased.get_rows-340"><span class="linenos">340</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
-</span><span id="DataBased.get_rows-341"><a href="#DataBased.get_rows-341"><span class="linenos">341</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-342"><a href="#DataBased.get_rows-342"><span class="linenos">342</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-343"><a href="#DataBased.get_rows-343"><span class="linenos">343</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-344"><a href="#DataBased.get_rows-344"><span class="linenos">344</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-345"><a href="#DataBased.get_rows-345"><span class="linenos">345</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-346"><a href="#DataBased.get_rows-346"><span class="linenos">346</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-347"><a href="#DataBased.get_rows-347"><span class="linenos">347</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-348"><a href="#DataBased.get_rows-348"><span class="linenos">348</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-349"><a href="#DataBased.get_rows-349"><span class="linenos">349</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-350"><a href="#DataBased.get_rows-350"><span class="linenos">350</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.get_rows-351"><a href="#DataBased.get_rows-351"><span class="linenos">351</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-352"><a href="#DataBased.get_rows-352"><span class="linenos">352</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
-</span><span id="DataBased.get_rows-353"><a href="#DataBased.get_rows-353"><span class="linenos">353</span></a>
-</span><span id="DataBased.get_rows-354"><a href="#DataBased.get_rows-354"><span class="linenos">354</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
-</span><span id="DataBased.get_rows-355"><a href="#DataBased.get_rows-355"><span class="linenos">355</span></a>
-</span><span id="DataBased.get_rows-356"><a href="#DataBased.get_rows-356"><span class="linenos">356</span></a>
-</span><span id="DataBased.get_rows-357"><a href="#DataBased.get_rows-357"><span class="linenos">357</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased.get_rows-358"><a href="#DataBased.get_rows-358"><span class="linenos">358</span></a>
-</span><span id="DataBased.get_rows-359"><a href="#DataBased.get_rows-359"><span class="linenos">359</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
-</span><span id="DataBased.get_rows-360"><a href="#DataBased.get_rows-360"><span class="linenos">360</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
-</span><span id="DataBased.get_rows-361"><a href="#DataBased.get_rows-361"><span class="linenos">361</span></a><span class="sd">        keys are column names and values are row values.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_rows-343"><a href="#DataBased.get_rows-343"><span class="linenos">343</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.get_rows-344"><a href="#DataBased.get_rows-344"><span class="linenos">344</span></a>    <span class="k">def</span> <span class="nf">get_rows</span><span class="p">(</span>
+</span><span id="DataBased.get_rows-345"><a href="#DataBased.get_rows-345"><span class="linenos">345</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-346"><a href="#DataBased.get_rows-346"><span class="linenos">346</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-347"><a href="#DataBased.get_rows-347"><span class="linenos">347</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-348"><a href="#DataBased.get_rows-348"><span class="linenos">348</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-349"><a href="#DataBased.get_rows-349"><span class="linenos">349</span></a>        <span class="n">sort_by_column</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-350"><a href="#DataBased.get_rows-350"><span class="linenos">350</span></a>        <span class="n">columns_to_return</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-351"><a href="#DataBased.get_rows-351"><span class="linenos">351</span></a>        <span class="n">return_as_dataframe</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-352"><a href="#DataBased.get_rows-352"><span class="linenos">352</span></a>        <span class="n">values_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-353"><a href="#DataBased.get_rows-353"><span class="linenos">353</span></a>        <span class="n">order_by</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-354"><a href="#DataBased.get_rows-354"><span class="linenos">354</span></a>        <span class="n">limit</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.get_rows-355"><a href="#DataBased.get_rows-355"><span class="linenos">355</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span> <span class="o">|</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-356"><a href="#DataBased.get_rows-356"><span class="linenos">356</span></a>        <span class="sd">&quot;&quot;&quot;Return matching rows from `table`.</span>
+</span><span id="DataBased.get_rows-357"><a href="#DataBased.get_rows-357"><span class="linenos">357</span></a>
+</span><span id="DataBased.get_rows-358"><a href="#DataBased.get_rows-358"><span class="linenos">358</span></a><span class="sd">        By default, rows will be returned as a list of dictionaries of the form `[{&quot;column_name&quot;: value, ...}, ...]`</span>
+</span><span id="DataBased.get_rows-359"><a href="#DataBased.get_rows-359"><span class="linenos">359</span></a>
+</span><span id="DataBased.get_rows-360"><a href="#DataBased.get_rows-360"><span class="linenos">360</span></a>
+</span><span id="DataBased.get_rows-361"><a href="#DataBased.get_rows-361"><span class="linenos">361</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased.get_rows-362"><a href="#DataBased.get_rows-362"><span class="linenos">362</span></a>
-</span><span id="DataBased.get_rows-363"><a href="#DataBased.get_rows-363"><span class="linenos">363</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
-</span><span id="DataBased.get_rows-364"><a href="#DataBased.get_rows-364"><span class="linenos">364</span></a>
-</span><span id="DataBased.get_rows-365"><a href="#DataBased.get_rows-365"><span class="linenos">365</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
-</span><span id="DataBased.get_rows-366"><a href="#DataBased.get_rows-366"><span class="linenos">366</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
-</span><span id="DataBased.get_rows-367"><a href="#DataBased.get_rows-367"><span class="linenos">367</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
+</span><span id="DataBased.get_rows-363"><a href="#DataBased.get_rows-363"><span class="linenos">363</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each</span>
+</span><span id="DataBased.get_rows-364"><a href="#DataBased.get_rows-364"><span class="linenos">364</span></a><span class="sd">        tuple is `(columnName, rowValue)` or a dictionary where</span>
+</span><span id="DataBased.get_rows-365"><a href="#DataBased.get_rows-365"><span class="linenos">365</span></a><span class="sd">        keys are column names and values are row values.</span>
+</span><span id="DataBased.get_rows-366"><a href="#DataBased.get_rows-366"><span class="linenos">366</span></a>
+</span><span id="DataBased.get_rows-367"><a href="#DataBased.get_rows-367"><span class="linenos">367</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column will be matched as a substring.</span>
 </span><span id="DataBased.get_rows-368"><a href="#DataBased.get_rows-368"><span class="linenos">368</span></a>
-</span><span id="DataBased.get_rows-369"><a href="#DataBased.get_rows-369"><span class="linenos">369</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
-</span><span id="DataBased.get_rows-370"><a href="#DataBased.get_rows-370"><span class="linenos">370</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
-</span><span id="DataBased.get_rows-371"><a href="#DataBased.get_rows-371"><span class="linenos">371</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
+</span><span id="DataBased.get_rows-369"><a href="#DataBased.get_rows-369"><span class="linenos">369</span></a><span class="sd">        `sort_by_column`: A column name to sort the results by.</span>
+</span><span id="DataBased.get_rows-370"><a href="#DataBased.get_rows-370"><span class="linenos">370</span></a><span class="sd">        This will sort results in Python after retrieving them from the db.</span>
+</span><span id="DataBased.get_rows-371"><a href="#DataBased.get_rows-371"><span class="linenos">371</span></a><span class="sd">        Use the &#39;order_by&#39; param to use SQLite engine for ordering.</span>
 </span><span id="DataBased.get_rows-372"><a href="#DataBased.get_rows-372"><span class="linenos">372</span></a>
-</span><span id="DataBased.get_rows-373"><a href="#DataBased.get_rows-373"><span class="linenos">373</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
-</span><span id="DataBased.get_rows-374"><a href="#DataBased.get_rows-374"><span class="linenos">374</span></a>
-</span><span id="DataBased.get_rows-375"><a href="#DataBased.get_rows-375"><span class="linenos">375</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="DataBased.get_rows-373"><a href="#DataBased.get_rows-373"><span class="linenos">373</span></a><span class="sd">        `columns_to_return`: Optional list of column names.</span>
+</span><span id="DataBased.get_rows-374"><a href="#DataBased.get_rows-374"><span class="linenos">374</span></a><span class="sd">        If provided, the elements returned by this function will only contain the provided columns.</span>
+</span><span id="DataBased.get_rows-375"><a href="#DataBased.get_rows-375"><span class="linenos">375</span></a><span class="sd">        Otherwise every column in the row is returned.</span>
 </span><span id="DataBased.get_rows-376"><a href="#DataBased.get_rows-376"><span class="linenos">376</span></a>
-</span><span id="DataBased.get_rows-377"><a href="#DataBased.get_rows-377"><span class="linenos">377</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="DataBased.get_rows-377"><a href="#DataBased.get_rows-377"><span class="linenos">377</span></a><span class="sd">        `return_as_dataframe`: Return the results as a `pandas.DataFrame` object.</span>
 </span><span id="DataBased.get_rows-378"><a href="#DataBased.get_rows-378"><span class="linenos">378</span></a>
-</span><span id="DataBased.get_rows-379"><a href="#DataBased.get_rows-379"><span class="linenos">379</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
-</span><span id="DataBased.get_rows-380"><a href="#DataBased.get_rows-380"><span class="linenos">380</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.get_rows-381"><a href="#DataBased.get_rows-381"><span class="linenos">381</span></a>
-</span><span id="DataBased.get_rows-382"><a href="#DataBased.get_rows-382"><span class="linenos">382</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-383"><a href="#DataBased.get_rows-383"><span class="linenos">383</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-384"><a href="#DataBased.get_rows-384"><span class="linenos">384</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
-</span><span id="DataBased.get_rows-385"><a href="#DataBased.get_rows-385"><span class="linenos">385</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased.get_rows-386"><a href="#DataBased.get_rows-386"><span class="linenos">386</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-387"><a href="#DataBased.get_rows-387"><span class="linenos">387</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-388"><a href="#DataBased.get_rows-388"><span class="linenos">388</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-389"><a href="#DataBased.get_rows-389"><span class="linenos">389</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-390"><a href="#DataBased.get_rows-390"><span class="linenos">390</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-391"><a href="#DataBased.get_rows-391"><span class="linenos">391</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.get_rows-392"><a href="#DataBased.get_rows-392"><span class="linenos">392</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased.get_rows-393"><a href="#DataBased.get_rows-393"><span class="linenos">393</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DataBased.get_rows-394"><a href="#DataBased.get_rows-394"><span class="linenos">394</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
-</span><span id="DataBased.get_rows-395"><a href="#DataBased.get_rows-395"><span class="linenos">395</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-396"><a href="#DataBased.get_rows-396"><span class="linenos">396</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-397"><a href="#DataBased.get_rows-397"><span class="linenos">397</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
-</span><span id="DataBased.get_rows-398"><a href="#DataBased.get_rows-398"><span class="linenos">398</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-399"><a href="#DataBased.get_rows-399"><span class="linenos">399</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
-</span><span id="DataBased.get_rows-400"><a href="#DataBased.get_rows-400"><span class="linenos">400</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-401"><a href="#DataBased.get_rows-401"><span class="linenos">401</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-402"><a href="#DataBased.get_rows-402"><span class="linenos">402</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.get_rows-403"><a href="#DataBased.get_rows-403"><span class="linenos">403</span></a>            <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased.get_rows-379"><a href="#DataBased.get_rows-379"><span class="linenos">379</span></a><span class="sd">        `values_only`: Return the results as a list of tuples.</span>
+</span><span id="DataBased.get_rows-380"><a href="#DataBased.get_rows-380"><span class="linenos">380</span></a>
+</span><span id="DataBased.get_rows-381"><a href="#DataBased.get_rows-381"><span class="linenos">381</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
+</span><span id="DataBased.get_rows-382"><a href="#DataBased.get_rows-382"><span class="linenos">382</span></a>
+</span><span id="DataBased.get_rows-383"><a href="#DataBased.get_rows-383"><span class="linenos">383</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
+</span><span id="DataBased.get_rows-384"><a href="#DataBased.get_rows-384"><span class="linenos">384</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.get_rows-385"><a href="#DataBased.get_rows-385"><span class="linenos">385</span></a>
+</span><span id="DataBased.get_rows-386"><a href="#DataBased.get_rows-386"><span class="linenos">386</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-387"><a href="#DataBased.get_rows-387"><span class="linenos">387</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-388"><a href="#DataBased.get_rows-388"><span class="linenos">388</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
+</span><span id="DataBased.get_rows-389"><a href="#DataBased.get_rows-389"><span class="linenos">389</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased.get_rows-390"><a href="#DataBased.get_rows-390"><span class="linenos">390</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-391"><a href="#DataBased.get_rows-391"><span class="linenos">391</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-392"><a href="#DataBased.get_rows-392"><span class="linenos">392</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-393"><a href="#DataBased.get_rows-393"><span class="linenos">393</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-394"><a href="#DataBased.get_rows-394"><span class="linenos">394</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-395"><a href="#DataBased.get_rows-395"><span class="linenos">395</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-396"><a href="#DataBased.get_rows-396"><span class="linenos">396</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased.get_rows-397"><a href="#DataBased.get_rows-397"><span class="linenos">397</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DataBased.get_rows-398"><a href="#DataBased.get_rows-398"><span class="linenos">398</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
+</span><span id="DataBased.get_rows-399"><a href="#DataBased.get_rows-399"><span class="linenos">399</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">match</span><span class="p">,</span> <span class="n">columns_to_return</span><span class="p">)</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-400"><a href="#DataBased.get_rows-400"><span class="linenos">400</span></a>        <span class="k">if</span> <span class="n">sort_by_column</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-401"><a href="#DataBased.get_rows-401"><span class="linenos">401</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">results</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span><span class="p">[</span><span class="n">sort_by_column</span><span class="p">])</span>
+</span><span id="DataBased.get_rows-402"><a href="#DataBased.get_rows-402"><span class="linenos">402</span></a>        <span class="k">if</span> <span class="n">return_as_dataframe</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-403"><a href="#DataBased.get_rows-403"><span class="linenos">403</span></a>            <span class="k">return</span> <span class="n">pandas</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">results</span><span class="p">)</span>
+</span><span id="DataBased.get_rows-404"><a href="#DataBased.get_rows-404"><span class="linenos">404</span></a>        <span class="k">if</span> <span class="n">values_only</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-405"><a href="#DataBased.get_rows-405"><span class="linenos">405</span></a>            <span class="k">return</span> <span class="p">[</span><span class="nb">tuple</span><span class="p">(</span><span class="n">row</span><span class="o">.</span><span class="n">values</span><span class="p">())</span> <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DataBased.get_rows-406"><a href="#DataBased.get_rows-406"><span class="linenos">406</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.get_rows-407"><a href="#DataBased.get_rows-407"><span class="linenos">407</span></a>            <span class="k">return</span> <span class="n">results</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return matching rows from <code>table</code>.</p>
 
 <p>By default, rows will be returned as a list of dictionaries of the form <code>[{"column_name": value, ...}, ...]</code></p>
 
@@ -1859,45 +1873,45 @@
         <span class="def">def</span>
         <span class="name">find</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.find-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.find"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.find-405"><a href="#DataBased.find-405"><span class="linenos">405</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.find-406"><a href="#DataBased.find-406"><span class="linenos">406</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
-</span><span id="DataBased.find-407"><a href="#DataBased.find-407"><span class="linenos">407</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.find-408"><a href="#DataBased.find-408"><span class="linenos">408</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
-</span><span id="DataBased.find-409"><a href="#DataBased.find-409"><span class="linenos">409</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
-</span><span id="DataBased.find-410"><a href="#DataBased.find-410"><span class="linenos">410</span></a>
-</span><span id="DataBased.find-411"><a href="#DataBased.find-411"><span class="linenos">411</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased.find-412"><a href="#DataBased.find-412"><span class="linenos">412</span></a>
-</span><span id="DataBased.find-413"><a href="#DataBased.find-413"><span class="linenos">413</span></a><span class="sd">        `table`: The table to search.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.find-409"><a href="#DataBased.find-409"><span class="linenos">409</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.find-410"><a href="#DataBased.find-410"><span class="linenos">410</span></a>    <span class="k">def</span> <span class="nf">find</span><span class="p">(</span>
+</span><span id="DataBased.find-411"><a href="#DataBased.find-411"><span class="linenos">411</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">query_string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">columns</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.find-412"><a href="#DataBased.find-412"><span class="linenos">412</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]:</span>
+</span><span id="DataBased.find-413"><a href="#DataBased.find-413"><span class="linenos">413</span></a>        <span class="sd">&quot;&quot;&quot;Search for rows that contain `query_string` as a substring of any column.</span>
 </span><span id="DataBased.find-414"><a href="#DataBased.find-414"><span class="linenos">414</span></a>
-</span><span id="DataBased.find-415"><a href="#DataBased.find-415"><span class="linenos">415</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="DataBased.find-415"><a href="#DataBased.find-415"><span class="linenos">415</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased.find-416"><a href="#DataBased.find-416"><span class="linenos">416</span></a>
-</span><span id="DataBased.find-417"><a href="#DataBased.find-417"><span class="linenos">417</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
-</span><span id="DataBased.find-418"><a href="#DataBased.find-418"><span class="linenos">418</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
-</span><span id="DataBased.find-419"><a href="#DataBased.find-419"><span class="linenos">419</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.find-420"><a href="#DataBased.find-420"><span class="linenos">420</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.find-421"><a href="#DataBased.find-421"><span class="linenos">421</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
-</span><span id="DataBased.find-422"><a href="#DataBased.find-422"><span class="linenos">422</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="DataBased.find-423"><a href="#DataBased.find-423"><span class="linenos">423</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.find-424"><a href="#DataBased.find-424"><span class="linenos">424</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DataBased.find-425"><a href="#DataBased.find-425"><span class="linenos">425</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
-</span><span id="DataBased.find-426"><a href="#DataBased.find-426"><span class="linenos">426</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="DataBased.find-427"><a href="#DataBased.find-427"><span class="linenos">427</span></a>                <span class="p">[</span>
-</span><span id="DataBased.find-428"><a href="#DataBased.find-428"><span class="linenos">428</span></a>                    <span class="n">row</span>
-</span><span id="DataBased.find-429"><a href="#DataBased.find-429"><span class="linenos">429</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
-</span><span id="DataBased.find-430"><a href="#DataBased.find-430"><span class="linenos">430</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
-</span><span id="DataBased.find-431"><a href="#DataBased.find-431"><span class="linenos">431</span></a>                    <span class="p">)</span>
-</span><span id="DataBased.find-432"><a href="#DataBased.find-432"><span class="linenos">432</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
-</span><span id="DataBased.find-433"><a href="#DataBased.find-433"><span class="linenos">433</span></a>                <span class="p">]</span>
-</span><span id="DataBased.find-434"><a href="#DataBased.find-434"><span class="linenos">434</span></a>            <span class="p">)</span>
-</span><span id="DataBased.find-435"><a href="#DataBased.find-435"><span class="linenos">435</span></a>        <span class="k">return</span> <span class="n">results</span>
+</span><span id="DataBased.find-417"><a href="#DataBased.find-417"><span class="linenos">417</span></a><span class="sd">        `table`: The table to search.</span>
+</span><span id="DataBased.find-418"><a href="#DataBased.find-418"><span class="linenos">418</span></a>
+</span><span id="DataBased.find-419"><a href="#DataBased.find-419"><span class="linenos">419</span></a><span class="sd">        `query_string`: The substring to search for in all columns.</span>
+</span><span id="DataBased.find-420"><a href="#DataBased.find-420"><span class="linenos">420</span></a>
+</span><span id="DataBased.find-421"><a href="#DataBased.find-421"><span class="linenos">421</span></a><span class="sd">        `columns`: A list of columns to search for query_string.</span>
+</span><span id="DataBased.find-422"><a href="#DataBased.find-422"><span class="linenos">422</span></a><span class="sd">        If None, all columns in the table will be searched.</span>
+</span><span id="DataBased.find-423"><a href="#DataBased.find-423"><span class="linenos">423</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.find-424"><a href="#DataBased.find-424"><span class="linenos">424</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.find-425"><a href="#DataBased.find-425"><span class="linenos">425</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns</span><span class="p">]</span>
+</span><span id="DataBased.find-426"><a href="#DataBased.find-426"><span class="linenos">426</span></a>        <span class="n">results</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="DataBased.find-427"><a href="#DataBased.find-427"><span class="linenos">427</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.find-428"><a href="#DataBased.find-428"><span class="linenos">428</span></a>            <span class="n">columns</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DataBased.find-429"><a href="#DataBased.find-429"><span class="linenos">429</span></a>        <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">:</span>
+</span><span id="DataBased.find-430"><a href="#DataBased.find-430"><span class="linenos">430</span></a>            <span class="n">results</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="DataBased.find-431"><a href="#DataBased.find-431"><span class="linenos">431</span></a>                <span class="p">[</span>
+</span><span id="DataBased.find-432"><a href="#DataBased.find-432"><span class="linenos">432</span></a>                    <span class="n">row</span>
+</span><span id="DataBased.find-433"><a href="#DataBased.find-433"><span class="linenos">433</span></a>                    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_rows</span><span class="p">(</span>
+</span><span id="DataBased.find-434"><a href="#DataBased.find-434"><span class="linenos">434</span></a>                        <span class="n">table</span><span class="p">,</span> <span class="p">[(</span><span class="n">column</span><span class="p">,</span> <span class="n">query_string</span><span class="p">)],</span> <span class="n">exact_match</span><span class="o">=</span><span class="kc">False</span>
+</span><span id="DataBased.find-435"><a href="#DataBased.find-435"><span class="linenos">435</span></a>                    <span class="p">)</span>
+</span><span id="DataBased.find-436"><a href="#DataBased.find-436"><span class="linenos">436</span></a>                    <span class="k">if</span> <span class="n">row</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">results</span>
+</span><span id="DataBased.find-437"><a href="#DataBased.find-437"><span class="linenos">437</span></a>                <span class="p">]</span>
+</span><span id="DataBased.find-438"><a href="#DataBased.find-438"><span class="linenos">438</span></a>            <span class="p">)</span>
+</span><span id="DataBased.find-439"><a href="#DataBased.find-439"><span class="linenos">439</span></a>        <span class="k">return</span> <span class="n">results</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Search for rows that contain <code>query_string</code> as a substring of any column.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1918,42 +1932,42 @@
         <span class="def">def</span>
         <span class="name">delete</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.delete-437"><a href="#DataBased.delete-437"><span class="linenos">437</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.delete-438"><a href="#DataBased.delete-438"><span class="linenos">438</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
-</span><span id="DataBased.delete-439"><a href="#DataBased.delete-439"><span class="linenos">439</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased.delete-440"><a href="#DataBased.delete-440"><span class="linenos">440</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased.delete-441"><a href="#DataBased.delete-441"><span class="linenos">441</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
-</span><span id="DataBased.delete-442"><a href="#DataBased.delete-442"><span class="linenos">442</span></a>
-</span><span id="DataBased.delete-443"><a href="#DataBased.delete-443"><span class="linenos">443</span></a><span class="sd">        Returns the number of deleted records.</span>
-</span><span id="DataBased.delete-444"><a href="#DataBased.delete-444"><span class="linenos">444</span></a>
-</span><span id="DataBased.delete-445"><a href="#DataBased.delete-445"><span class="linenos">445</span></a><span class="sd">        #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.delete-441"><a href="#DataBased.delete-441"><span class="linenos">441</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.delete-442"><a href="#DataBased.delete-442"><span class="linenos">442</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span>
+</span><span id="DataBased.delete-443"><a href="#DataBased.delete-443"><span class="linenos">443</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased.delete-444"><a href="#DataBased.delete-444"><span class="linenos">444</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.delete-445"><a href="#DataBased.delete-445"><span class="linenos">445</span></a>        <span class="sd">&quot;&quot;&quot;Delete records from `table`.</span>
 </span><span id="DataBased.delete-446"><a href="#DataBased.delete-446"><span class="linenos">446</span></a>
-</span><span id="DataBased.delete-447"><a href="#DataBased.delete-447"><span class="linenos">447</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
-</span><span id="DataBased.delete-448"><a href="#DataBased.delete-448"><span class="linenos">448</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
-</span><span id="DataBased.delete-449"><a href="#DataBased.delete-449"><span class="linenos">449</span></a>
-</span><span id="DataBased.delete-450"><a href="#DataBased.delete-450"><span class="linenos">450</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
-</span><span id="DataBased.delete-451"><a href="#DataBased.delete-451"><span class="linenos">451</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.delete-452"><a href="#DataBased.delete-452"><span class="linenos">452</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased.delete-453"><a href="#DataBased.delete-453"><span class="linenos">453</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.delete-454"><a href="#DataBased.delete-454"><span class="linenos">454</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
-</span><span id="DataBased.delete-455"><a href="#DataBased.delete-455"><span class="linenos">455</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
-</span><span id="DataBased.delete-456"><a href="#DataBased.delete-456"><span class="linenos">456</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.delete-457"><a href="#DataBased.delete-457"><span class="linenos">457</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
-</span><span id="DataBased.delete-458"><a href="#DataBased.delete-458"><span class="linenos">458</span></a>            <span class="p">)</span>
-</span><span id="DataBased.delete-459"><a href="#DataBased.delete-459"><span class="linenos">459</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
-</span><span id="DataBased.delete-460"><a href="#DataBased.delete-460"><span class="linenos">460</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.delete-461"><a href="#DataBased.delete-461"><span class="linenos">461</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
-</span><span id="DataBased.delete-462"><a href="#DataBased.delete-462"><span class="linenos">462</span></a>                <span class="sa">f</span><span class="s1">&#39;Error deleting rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased.delete-463"><a href="#DataBased.delete-463"><span class="linenos">463</span></a>            <span class="p">)</span>
-</span><span id="DataBased.delete-464"><a href="#DataBased.delete-464"><span class="linenos">464</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased.delete-447"><a href="#DataBased.delete-447"><span class="linenos">447</span></a><span class="sd">        Returns the number of deleted records.</span>
+</span><span id="DataBased.delete-448"><a href="#DataBased.delete-448"><span class="linenos">448</span></a>
+</span><span id="DataBased.delete-449"><a href="#DataBased.delete-449"><span class="linenos">449</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.delete-450"><a href="#DataBased.delete-450"><span class="linenos">450</span></a>
+</span><span id="DataBased.delete-451"><a href="#DataBased.delete-451"><span class="linenos">451</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
+</span><span id="DataBased.delete-452"><a href="#DataBased.delete-452"><span class="linenos">452</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased.delete-453"><a href="#DataBased.delete-453"><span class="linenos">453</span></a>
+</span><span id="DataBased.delete-454"><a href="#DataBased.delete-454"><span class="linenos">454</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
+</span><span id="DataBased.delete-455"><a href="#DataBased.delete-455"><span class="linenos">455</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="DataBased.delete-456"><a href="#DataBased.delete-456"><span class="linenos">456</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased.delete-457"><a href="#DataBased.delete-457"><span class="linenos">457</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.delete-458"><a href="#DataBased.delete-458"><span class="linenos">458</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.delete-459"><a href="#DataBased.delete-459"><span class="linenos">459</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
+</span><span id="DataBased.delete-460"><a href="#DataBased.delete-460"><span class="linenos">460</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.delete-461"><a href="#DataBased.delete-461"><span class="linenos">461</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
+</span><span id="DataBased.delete-462"><a href="#DataBased.delete-462"><span class="linenos">462</span></a>            <span class="p">)</span>
+</span><span id="DataBased.delete-463"><a href="#DataBased.delete-463"><span class="linenos">463</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
+</span><span id="DataBased.delete-464"><a href="#DataBased.delete-464"><span class="linenos">464</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.delete-465"><a href="#DataBased.delete-465"><span class="linenos">465</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
+</span><span id="DataBased.delete-466"><a href="#DataBased.delete-466"><span class="linenos">466</span></a>                <span class="sa">f</span><span class="s1">&#39;Error deleting rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">.</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased.delete-467"><a href="#DataBased.delete-467"><span class="linenos">467</span></a>            <span class="p">)</span>
+</span><span id="DataBased.delete-468"><a href="#DataBased.delete-468"><span class="linenos">468</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete records from <code>table</code>.</p>
 
 <p>Returns the number of deleted records.</p>
 
@@ -1974,63 +1988,63 @@
         <span class="def">def</span>
         <span class="name">update</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.update-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.update"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.update-466"><a href="#DataBased.update-466"><span class="linenos">466</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.update-467"><a href="#DataBased.update-467"><span class="linenos">467</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
-</span><span id="DataBased.update-468"><a href="#DataBased.update-468"><span class="linenos">468</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="DataBased.update-469"><a href="#DataBased.update-469"><span class="linenos">469</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.update-470"><a href="#DataBased.update-470"><span class="linenos">470</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
-</span><span id="DataBased.update-471"><a href="#DataBased.update-471"><span class="linenos">471</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="DataBased.update-472"><a href="#DataBased.update-472"><span class="linenos">472</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="DataBased.update-473"><a href="#DataBased.update-473"><span class="linenos">473</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="DataBased.update-474"><a href="#DataBased.update-474"><span class="linenos">474</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="DataBased.update-475"><a href="#DataBased.update-475"><span class="linenos">475</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
-</span><span id="DataBased.update-476"><a href="#DataBased.update-476"><span class="linenos">476</span></a>
-</span><span id="DataBased.update-477"><a href="#DataBased.update-477"><span class="linenos">477</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased.update-478"><a href="#DataBased.update-478"><span class="linenos">478</span></a>
-</span><span id="DataBased.update-479"><a href="#DataBased.update-479"><span class="linenos">479</span></a><span class="sd">        `table`: The table to update rows in.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.update-470"><a href="#DataBased.update-470"><span class="linenos">470</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.update-471"><a href="#DataBased.update-471"><span class="linenos">471</span></a>    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span>
+</span><span id="DataBased.update-472"><a href="#DataBased.update-472"><span class="linenos">472</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="DataBased.update-473"><a href="#DataBased.update-473"><span class="linenos">473</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.update-474"><a href="#DataBased.update-474"><span class="linenos">474</span></a>        <span class="n">column_to_update</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
+</span><span id="DataBased.update-475"><a href="#DataBased.update-475"><span class="linenos">475</span></a>        <span class="n">new_value</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="DataBased.update-476"><a href="#DataBased.update-476"><span class="linenos">476</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="DataBased.update-477"><a href="#DataBased.update-477"><span class="linenos">477</span></a>        <span class="n">exact_match</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="DataBased.update-478"><a href="#DataBased.update-478"><span class="linenos">478</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="DataBased.update-479"><a href="#DataBased.update-479"><span class="linenos">479</span></a>        <span class="sd">&quot;&quot;&quot;Update the value in `column_to_update` to `new_value` for rows matched with `match_criteria`.</span>
 </span><span id="DataBased.update-480"><a href="#DataBased.update-480"><span class="linenos">480</span></a>
-</span><span id="DataBased.update-481"><a href="#DataBased.update-481"><span class="linenos">481</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
+</span><span id="DataBased.update-481"><a href="#DataBased.update-481"><span class="linenos">481</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased.update-482"><a href="#DataBased.update-482"><span class="linenos">482</span></a>
-</span><span id="DataBased.update-483"><a href="#DataBased.update-483"><span class="linenos">483</span></a><span class="sd">        `new_value`: The new value to insert.</span>
+</span><span id="DataBased.update-483"><a href="#DataBased.update-483"><span class="linenos">483</span></a><span class="sd">        `table`: The table to update rows in.</span>
 </span><span id="DataBased.update-484"><a href="#DataBased.update-484"><span class="linenos">484</span></a>
-</span><span id="DataBased.update-485"><a href="#DataBased.update-485"><span class="linenos">485</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
-</span><span id="DataBased.update-486"><a href="#DataBased.update-486"><span class="linenos">486</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
-</span><span id="DataBased.update-487"><a href="#DataBased.update-487"><span class="linenos">487</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="DataBased.update-485"><a href="#DataBased.update-485"><span class="linenos">485</span></a><span class="sd">        `column_to_update`: The column to be updated in the matched rows.</span>
+</span><span id="DataBased.update-486"><a href="#DataBased.update-486"><span class="linenos">486</span></a>
+</span><span id="DataBased.update-487"><a href="#DataBased.update-487"><span class="linenos">487</span></a><span class="sd">        `new_value`: The new value to insert.</span>
 </span><span id="DataBased.update-488"><a href="#DataBased.update-488"><span class="linenos">488</span></a>
-</span><span id="DataBased.update-489"><a href="#DataBased.update-489"><span class="linenos">489</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
-</span><span id="DataBased.update-490"><a href="#DataBased.update-490"><span class="linenos">490</span></a>
-</span><span id="DataBased.update-491"><a href="#DataBased.update-491"><span class="linenos">491</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
-</span><span id="DataBased.update-492"><a href="#DataBased.update-492"><span class="linenos">492</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
-</span><span id="DataBased.update-493"><a href="#DataBased.update-493"><span class="linenos">493</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="DataBased.update-494"><a href="#DataBased.update-494"><span class="linenos">494</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
-</span><span id="DataBased.update-495"><a href="#DataBased.update-495"><span class="linenos">495</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
-</span><span id="DataBased.update-496"><a href="#DataBased.update-496"><span class="linenos">496</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DataBased.update-497"><a href="#DataBased.update-497"><span class="linenos">497</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.update-498"><a href="#DataBased.update-498"><span class="linenos">498</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.update-499"><a href="#DataBased.update-499"><span class="linenos">499</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
-</span><span id="DataBased.update-500"><a href="#DataBased.update-500"><span class="linenos">500</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.update-501"><a href="#DataBased.update-501"><span class="linenos">501</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.update-502"><a href="#DataBased.update-502"><span class="linenos">502</span></a>                <span class="n">query</span><span class="p">,</span>
-</span><span id="DataBased.update-503"><a href="#DataBased.update-503"><span class="linenos">503</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
-</span><span id="DataBased.update-504"><a href="#DataBased.update-504"><span class="linenos">504</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-505"><a href="#DataBased.update-505"><span class="linenos">505</span></a>            <span class="n">num_updates</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
-</span><span id="DataBased.update-506"><a href="#DataBased.update-506"><span class="linenos">506</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
-</span><span id="DataBased.update-507"><a href="#DataBased.update-507"><span class="linenos">507</span></a>                <span class="sa">f</span><span class="s1">&#39;In </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s1"> rows, updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased.update-489"><a href="#DataBased.update-489"><span class="linenos">489</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
+</span><span id="DataBased.update-490"><a href="#DataBased.update-490"><span class="linenos">490</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
+</span><span id="DataBased.update-491"><a href="#DataBased.update-491"><span class="linenos">491</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
+</span><span id="DataBased.update-492"><a href="#DataBased.update-492"><span class="linenos">492</span></a>
+</span><span id="DataBased.update-493"><a href="#DataBased.update-493"><span class="linenos">493</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
+</span><span id="DataBased.update-494"><a href="#DataBased.update-494"><span class="linenos">494</span></a>
+</span><span id="DataBased.update-495"><a href="#DataBased.update-495"><span class="linenos">495</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
+</span><span id="DataBased.update-496"><a href="#DataBased.update-496"><span class="linenos">496</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased.update-497"><a href="#DataBased.update-497"><span class="linenos">497</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="DataBased.update-498"><a href="#DataBased.update-498"><span class="linenos">498</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
+</span><span id="DataBased.update-499"><a href="#DataBased.update-499"><span class="linenos">499</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
+</span><span id="DataBased.update-500"><a href="#DataBased.update-500"><span class="linenos">500</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.update-501"><a href="#DataBased.update-501"><span class="linenos">501</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.update-502"><a href="#DataBased.update-502"><span class="linenos">502</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.update-503"><a href="#DataBased.update-503"><span class="linenos">503</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
+</span><span id="DataBased.update-504"><a href="#DataBased.update-504"><span class="linenos">504</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.update-505"><a href="#DataBased.update-505"><span class="linenos">505</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.update-506"><a href="#DataBased.update-506"><span class="linenos">506</span></a>                <span class="n">query</span><span class="p">,</span>
+</span><span id="DataBased.update-507"><a href="#DataBased.update-507"><span class="linenos">507</span></a>                <span class="p">(</span><span class="n">new_value</span><span class="p">,),</span>
 </span><span id="DataBased.update-508"><a href="#DataBased.update-508"><span class="linenos">508</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-509"><a href="#DataBased.update-509"><span class="linenos">509</span></a>            <span class="k">return</span> <span class="n">num_updates</span>
-</span><span id="DataBased.update-510"><a href="#DataBased.update-510"><span class="linenos">510</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.update-511"><a href="#DataBased.update-511"><span class="linenos">511</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
-</span><span id="DataBased.update-512"><a href="#DataBased.update-512"><span class="linenos">512</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
-</span><span id="DataBased.update-513"><a href="#DataBased.update-513"><span class="linenos">513</span></a>            <span class="p">)</span>
-</span><span id="DataBased.update-514"><a href="#DataBased.update-514"><span class="linenos">514</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="DataBased.update-509"><a href="#DataBased.update-509"><span class="linenos">509</span></a>            <span class="n">num_updates</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
+</span><span id="DataBased.update-510"><a href="#DataBased.update-510"><span class="linenos">510</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
+</span><span id="DataBased.update-511"><a href="#DataBased.update-511"><span class="linenos">511</span></a>                <span class="sa">f</span><span class="s1">&#39;In </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s1"> rows, updated &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased.update-512"><a href="#DataBased.update-512"><span class="linenos">512</span></a>            <span class="p">)</span>
+</span><span id="DataBased.update-513"><a href="#DataBased.update-513"><span class="linenos">513</span></a>            <span class="k">return</span> <span class="n">num_updates</span>
+</span><span id="DataBased.update-514"><a href="#DataBased.update-514"><span class="linenos">514</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.update-515"><a href="#DataBased.update-515"><span class="linenos">515</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span>
+</span><span id="DataBased.update-516"><a href="#DataBased.update-516"><span class="linenos">516</span></a>                <span class="sa">f</span><span class="s1">&#39;Failed to update &quot;</span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s1">&quot; in &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table to &quot;</span><span class="si">{</span><span class="n">new_value</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;</span><span class="se">\n</span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s1">&#39;</span>
+</span><span id="DataBased.update-517"><a href="#DataBased.update-517"><span class="linenos">517</span></a>            <span class="p">)</span>
+</span><span id="DataBased.update-518"><a href="#DataBased.update-518"><span class="linenos">518</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update the value in <code>column_to_update</code> to <code>new_value</code> for rows matched with <code>match_criteria</code>.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -2058,27 +2072,27 @@
         <span class="def">def</span>
         <span class="name">drop_table</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">table</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.drop_table-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.drop_table"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.drop_table-516"><a href="#DataBased.drop_table-516"><span class="linenos">516</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.drop_table-517"><a href="#DataBased.drop_table-517"><span class="linenos">517</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-518"><a href="#DataBased.drop_table-518"><span class="linenos">518</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
-</span><span id="DataBased.drop_table-519"><a href="#DataBased.drop_table-519"><span class="linenos">519</span></a>
-</span><span id="DataBased.drop_table-520"><a href="#DataBased.drop_table-520"><span class="linenos">520</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
-</span><span id="DataBased.drop_table-521"><a href="#DataBased.drop_table-521"><span class="linenos">521</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-522"><a href="#DataBased.drop_table-522"><span class="linenos">522</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-523"><a href="#DataBased.drop_table-523"><span class="linenos">523</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-524"><a href="#DataBased.drop_table-524"><span class="linenos">524</span></a>            <span class="k">return</span> <span class="kc">True</span>
-</span><span id="DataBased.drop_table-525"><a href="#DataBased.drop_table-525"><span class="linenos">525</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-526"><a href="#DataBased.drop_table-526"><span class="linenos">526</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-527"><a href="#DataBased.drop_table-527"><span class="linenos">527</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="DataBased.drop_table-528"><a href="#DataBased.drop_table-528"><span class="linenos">528</span></a>            <span class="k">return</span> <span class="kc">False</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.drop_table-520"><a href="#DataBased.drop_table-520"><span class="linenos">520</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.drop_table-521"><a href="#DataBased.drop_table-521"><span class="linenos">521</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-522"><a href="#DataBased.drop_table-522"><span class="linenos">522</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
+</span><span id="DataBased.drop_table-523"><a href="#DataBased.drop_table-523"><span class="linenos">523</span></a>
+</span><span id="DataBased.drop_table-524"><a href="#DataBased.drop_table-524"><span class="linenos">524</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
+</span><span id="DataBased.drop_table-525"><a href="#DataBased.drop_table-525"><span class="linenos">525</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-526"><a href="#DataBased.drop_table-526"><span class="linenos">526</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-527"><a href="#DataBased.drop_table-527"><span class="linenos">527</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-528"><a href="#DataBased.drop_table-528"><span class="linenos">528</span></a>            <span class="k">return</span> <span class="kc">True</span>
+</span><span id="DataBased.drop_table-529"><a href="#DataBased.drop_table-529"><span class="linenos">529</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.drop_table-530"><a href="#DataBased.drop_table-530"><span class="linenos">530</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-531"><a href="#DataBased.drop_table-531"><span class="linenos">531</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-532"><a href="#DataBased.drop_table-532"><span class="linenos">532</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Drop <code>table</code> from the database.</p>
 
 <p>Returns <code>True</code> if successful, <code>False</code> if not.</p>
 </div>
@@ -2092,40 +2106,40 @@
         <span class="def">def</span>
         <span class="name">add_column</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">table</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">column</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">_type</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DataBased.add_column-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.add_column"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_column-530"><a href="#DataBased.add_column-530"><span class="linenos">530</span></a>    <span class="nd">@_connect</span>
-</span><span id="DataBased.add_column-531"><a href="#DataBased.add_column-531"><span class="linenos">531</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
-</span><span id="DataBased.add_column-532"><a href="#DataBased.add_column-532"><span class="linenos">532</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="DataBased.add_column-533"><a href="#DataBased.add_column-533"><span class="linenos">533</span></a>    <span class="p">):</span>
-</span><span id="DataBased.add_column-534"><a href="#DataBased.add_column-534"><span class="linenos">534</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
-</span><span id="DataBased.add_column-535"><a href="#DataBased.add_column-535"><span class="linenos">535</span></a>
-</span><span id="DataBased.add_column-536"><a href="#DataBased.add_column-536"><span class="linenos">536</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased.add_column-537"><a href="#DataBased.add_column-537"><span class="linenos">537</span></a>
-</span><span id="DataBased.add_column-538"><a href="#DataBased.add_column-538"><span class="linenos">538</span></a><span class="sd">        `column`: Name of the column to add.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.add_column-534"><a href="#DataBased.add_column-534"><span class="linenos">534</span></a>    <span class="nd">@_connect</span>
+</span><span id="DataBased.add_column-535"><a href="#DataBased.add_column-535"><span class="linenos">535</span></a>    <span class="k">def</span> <span class="nf">add_column</span><span class="p">(</span>
+</span><span id="DataBased.add_column-536"><a href="#DataBased.add_column-536"><span class="linenos">536</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">_type</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">default_value</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="DataBased.add_column-537"><a href="#DataBased.add_column-537"><span class="linenos">537</span></a>    <span class="p">):</span>
+</span><span id="DataBased.add_column-538"><a href="#DataBased.add_column-538"><span class="linenos">538</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to `table`.</span>
 </span><span id="DataBased.add_column-539"><a href="#DataBased.add_column-539"><span class="linenos">539</span></a>
-</span><span id="DataBased.add_column-540"><a href="#DataBased.add_column-540"><span class="linenos">540</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="DataBased.add_column-540"><a href="#DataBased.add_column-540"><span class="linenos">540</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased.add_column-541"><a href="#DataBased.add_column-541"><span class="linenos">541</span></a>
-</span><span id="DataBased.add_column-542"><a href="#DataBased.add_column-542"><span class="linenos">542</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
-</span><span id="DataBased.add_column-543"><a href="#DataBased.add_column-543"><span class="linenos">543</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.add_column-544"><a href="#DataBased.add_column-544"><span class="linenos">544</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
-</span><span id="DataBased.add_column-545"><a href="#DataBased.add_column-545"><span class="linenos">545</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_column-546"><a href="#DataBased.add_column-546"><span class="linenos">546</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DataBased.add_column-547"><a href="#DataBased.add_column-547"><span class="linenos">547</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_column-548"><a href="#DataBased.add_column-548"><span class="linenos">548</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
-</span><span id="DataBased.add_column-549"><a href="#DataBased.add_column-549"><span class="linenos">549</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_column-550"><a href="#DataBased.add_column-550"><span class="linenos">550</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_column-551"><a href="#DataBased.add_column-551"><span class="linenos">551</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DataBased.add_column-552"><a href="#DataBased.add_column-552"><span class="linenos">552</span></a>                <span class="p">)</span>
-</span><span id="DataBased.add_column-553"><a href="#DataBased.add_column-553"><span class="linenos">553</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased.add_column-554"><a href="#DataBased.add_column-554"><span class="linenos">554</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.add_column-555"><a href="#DataBased.add_column-555"><span class="linenos">555</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-542"><a href="#DataBased.add_column-542"><span class="linenos">542</span></a><span class="sd">        `column`: Name of the column to add.</span>
+</span><span id="DataBased.add_column-543"><a href="#DataBased.add_column-543"><span class="linenos">543</span></a>
+</span><span id="DataBased.add_column-544"><a href="#DataBased.add_column-544"><span class="linenos">544</span></a><span class="sd">        `_type`: The data type of the new column.</span>
+</span><span id="DataBased.add_column-545"><a href="#DataBased.add_column-545"><span class="linenos">545</span></a>
+</span><span id="DataBased.add_column-546"><a href="#DataBased.add_column-546"><span class="linenos">546</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
+</span><span id="DataBased.add_column-547"><a href="#DataBased.add_column-547"><span class="linenos">547</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DataBased.add_column-548"><a href="#DataBased.add_column-548"><span class="linenos">548</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
+</span><span id="DataBased.add_column-549"><a href="#DataBased.add_column-549"><span class="linenos">549</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_column-550"><a href="#DataBased.add_column-550"><span class="linenos">550</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased.add_column-551"><a href="#DataBased.add_column-551"><span class="linenos">551</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_column-552"><a href="#DataBased.add_column-552"><span class="linenos">552</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
+</span><span id="DataBased.add_column-553"><a href="#DataBased.add_column-553"><span class="linenos">553</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DataBased.add_column-554"><a href="#DataBased.add_column-554"><span class="linenos">554</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_column-555"><a href="#DataBased.add_column-555"><span class="linenos">555</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased.add_column-556"><a href="#DataBased.add_column-556"><span class="linenos">556</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_column-557"><a href="#DataBased.add_column-557"><span class="linenos">557</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-558"><a href="#DataBased.add_column-558"><span class="linenos">558</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.add_column-559"><a href="#DataBased.add_column-559"><span class="linenos">559</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a new column to <code>table</code>.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -2146,30 +2160,30 @@
         <span class="def">def</span>
         <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-557"><a href="#DataBased.data_to_string-557"><span class="linenos">557</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased.data_to_string-558"><a href="#DataBased.data_to_string-558"><span class="linenos">558</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased.data_to_string-559"><a href="#DataBased.data_to_string-559"><span class="linenos">559</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased.data_to_string-560"><a href="#DataBased.data_to_string-560"><span class="linenos">560</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.data_to_string-561"><a href="#DataBased.data_to_string-561"><span class="linenos">561</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="DataBased.data_to_string-562"><a href="#DataBased.data_to_string-562"><span class="linenos">562</span></a>
-</span><span id="DataBased.data_to_string-563"><a href="#DataBased.data_to_string-563"><span class="linenos">563</span></a><span class="sd">        #### :params:</span>
-</span><span id="DataBased.data_to_string-564"><a href="#DataBased.data_to_string-564"><span class="linenos">564</span></a>
-</span><span id="DataBased.data_to_string-565"><a href="#DataBased.data_to_string-565"><span class="linenos">565</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="DataBased.data_to_string-566"><a href="#DataBased.data_to_string-566"><span class="linenos">566</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased.data_to_string-567"><a href="#DataBased.data_to_string-567"><span class="linenos">567</span></a>
-</span><span id="DataBased.data_to_string-568"><a href="#DataBased.data_to_string-568"><span class="linenos">568</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
-</span><span id="DataBased.data_to_string-569"><a href="#DataBased.data_to_string-569"><span class="linenos">569</span></a>
-</span><span id="DataBased.data_to_string-570"><a href="#DataBased.data_to_string-570"><span class="linenos">570</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="DataBased.data_to_string-571"><a href="#DataBased.data_to_string-571"><span class="linenos">571</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="DataBased.data_to_string-572"><a href="#DataBased.data_to_string-572"><span class="linenos">572</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-561"><a href="#DataBased.data_to_string-561"><span class="linenos">561</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased.data_to_string-562"><a href="#DataBased.data_to_string-562"><span class="linenos">562</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased.data_to_string-563"><a href="#DataBased.data_to_string-563"><span class="linenos">563</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased.data_to_string-564"><a href="#DataBased.data_to_string-564"><span class="linenos">564</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.data_to_string-565"><a href="#DataBased.data_to_string-565"><span class="linenos">565</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="DataBased.data_to_string-566"><a href="#DataBased.data_to_string-566"><span class="linenos">566</span></a>
+</span><span id="DataBased.data_to_string-567"><a href="#DataBased.data_to_string-567"><span class="linenos">567</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.data_to_string-568"><a href="#DataBased.data_to_string-568"><span class="linenos">568</span></a>
+</span><span id="DataBased.data_to_string-569"><a href="#DataBased.data_to_string-569"><span class="linenos">569</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="DataBased.data_to_string-570"><a href="#DataBased.data_to_string-570"><span class="linenos">570</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="DataBased.data_to_string-571"><a href="#DataBased.data_to_string-571"><span class="linenos">571</span></a>
+</span><span id="DataBased.data_to_string-572"><a href="#DataBased.data_to_string-572"><span class="linenos">572</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased.data_to_string-573"><a href="#DataBased.data_to_string-573"><span class="linenos">573</span></a>
+</span><span id="DataBased.data_to_string-574"><a href="#DataBased.data_to_string-574"><span class="linenos">574</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="DataBased.data_to_string-575"><a href="#DataBased.data_to_string-575"><span class="linenos">575</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="DataBased.data_to_string-576"><a href="#DataBased.data_to_string-576"><span class="linenos">576</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -2192,42 +2206,42 @@
         <span class="def">def</span>
         <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-575"><a href="#data_to_string-575"><span class="linenos">575</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="data_to_string-576"><a href="#data_to_string-576"><span class="linenos">576</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="data_to_string-577"><a href="#data_to_string-577"><span class="linenos">577</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="data_to_string-578"><a href="#data_to_string-578"><span class="linenos">578</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="data_to_string-579"><a href="#data_to_string-579"><span class="linenos">579</span></a>
-</span><span id="data_to_string-580"><a href="#data_to_string-580"><span class="linenos">580</span></a><span class="sd">    #### :params:</span>
-</span><span id="data_to_string-581"><a href="#data_to_string-581"><span class="linenos">581</span></a>
-</span><span id="data_to_string-582"><a href="#data_to_string-582"><span class="linenos">582</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="data_to_string-583"><a href="#data_to_string-583"><span class="linenos">583</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="data_to_string-584"><a href="#data_to_string-584"><span class="linenos">584</span></a>
-</span><span id="data_to_string-585"><a href="#data_to_string-585"><span class="linenos">585</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
-</span><span id="data_to_string-586"><a href="#data_to_string-586"><span class="linenos">586</span></a>
-</span><span id="data_to_string-587"><a href="#data_to_string-587"><span class="linenos">587</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="data_to_string-588"><a href="#data_to_string-588"><span class="linenos">588</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="data_to_string-589"><a href="#data_to_string-589"><span class="linenos">589</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="data_to_string-590"><a href="#data_to_string-590"><span class="linenos">590</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="data_to_string-591"><a href="#data_to_string-591"><span class="linenos">591</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="data_to_string-592"><a href="#data_to_string-592"><span class="linenos">592</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="data_to_string-593"><a href="#data_to_string-593"><span class="linenos">593</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="data_to_string-594"><a href="#data_to_string-594"><span class="linenos">594</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="data_to_string-595"><a href="#data_to_string-595"><span class="linenos">595</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="data_to_string-596"><a href="#data_to_string-596"><span class="linenos">596</span></a>
-</span><span id="data_to_string-597"><a href="#data_to_string-597"><span class="linenos">597</span></a>    <span class="k">try</span><span class="p">:</span>
-</span><span id="data_to_string-598"><a href="#data_to_string-598"><span class="linenos">598</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-599"><a href="#data_to_string-599"><span class="linenos">599</span></a>        <span class="k">return</span> <span class="n">griddy</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="s2">&quot;keys&quot;</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
-</span><span id="data_to_string-600"><a href="#data_to_string-600"><span class="linenos">600</span></a>    <span class="k">except</span> <span class="ne">RuntimeError</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="data_to_string-601"><a href="#data_to_string-601"><span class="linenos">601</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="data_to_string-602"><a href="#data_to_string-602"><span class="linenos">602</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-579"><a href="#data_to_string-579"><span class="linenos">579</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="data_to_string-580"><a href="#data_to_string-580"><span class="linenos">580</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="data_to_string-581"><a href="#data_to_string-581"><span class="linenos">581</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="data_to_string-582"><a href="#data_to_string-582"><span class="linenos">582</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
+</span><span id="data_to_string-583"><a href="#data_to_string-583"><span class="linenos">583</span></a>
+</span><span id="data_to_string-584"><a href="#data_to_string-584"><span class="linenos">584</span></a><span class="sd">    #### :params:</span>
+</span><span id="data_to_string-585"><a href="#data_to_string-585"><span class="linenos">585</span></a>
+</span><span id="data_to_string-586"><a href="#data_to_string-586"><span class="linenos">586</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="data_to_string-587"><a href="#data_to_string-587"><span class="linenos">587</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
+</span><span id="data_to_string-588"><a href="#data_to_string-588"><span class="linenos">588</span></a>
+</span><span id="data_to_string-589"><a href="#data_to_string-589"><span class="linenos">589</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="data_to_string-590"><a href="#data_to_string-590"><span class="linenos">590</span></a>
+</span><span id="data_to_string-591"><a href="#data_to_string-591"><span class="linenos">591</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="data_to_string-592"><a href="#data_to_string-592"><span class="linenos">592</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="data_to_string-593"><a href="#data_to_string-593"><span class="linenos">593</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="data_to_string-594"><a href="#data_to_string-594"><span class="linenos">594</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="data_to_string-595"><a href="#data_to_string-595"><span class="linenos">595</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="data_to_string-596"><a href="#data_to_string-596"><span class="linenos">596</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="data_to_string-597"><a href="#data_to_string-597"><span class="linenos">597</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="data_to_string-598"><a href="#data_to_string-598"><span class="linenos">598</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="data_to_string-599"><a href="#data_to_string-599"><span class="linenos">599</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
+</span><span id="data_to_string-600"><a href="#data_to_string-600"><span class="linenos">600</span></a>
+</span><span id="data_to_string-601"><a href="#data_to_string-601"><span class="linenos">601</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="data_to_string-602"><a href="#data_to_string-602"><span class="linenos">602</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-603"><a href="#data_to_string-603"><span class="linenos">603</span></a>        <span class="k">return</span> <span class="n">griddy</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="s2">&quot;keys&quot;</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="data_to_string-604"><a href="#data_to_string-604"><span class="linenos">604</span></a>    <span class="k">except</span> <span class="ne">RuntimeError</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="data_to_string-605"><a href="#data_to_string-605"><span class="linenos">605</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="data_to_string-606"><a href="#data_to_string-606"><span class="linenos">606</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -225,475 +225,479 @@
 182        else:
 183            conditions = " and ".join(
 184                f'"{column_row[0]}" like "%{column_row[1]}%"'
 185                for column_row in match_criteria
 186            )
 187        return f"({conditions})"
 188
-189    def vacuum(self):
-190        """Reduce disk size of the database with a `VACUUM` query."""
-191        self.query("VACUUM;")
-192
-193    @_connect
-194    def query(self, query_) -> list[Any]:
-195        """Execute an arbitrary query and return the results."""
-196        self.cursor.execute(query_)
-197        return self.cursor.fetchall()
-198
-199    @_connect
-200    def create_tables(self, table_defs: list[str] = []):
-201        """Create tables if they don't exist.
+189    def vacuum(self) -> int:
+190        """Reduce disk size of the database with a `VACUUM` query.
+191
+192        Returns space freed up in bytes."""
+193        size = self.dbpath.size
+194        self.query("VACUUM;")
+195        return size - self.dbpath.size
+196
+197    @_connect
+198    def query(self, query_) -> list[Any]:
+199        """Execute an arbitrary query and return the results."""
+200        self.cursor.execute(query_)
+201        return self.cursor.fetchall()
 202
-203        :param `table_defs`: Each definition should be in the form
+203    @_connect
+204    def create_tables(self, table_defs: list[str] = []):
+205        """Create tables if they don't exist.
+206
+207        :param `table_defs`: Each definition should be in the form
 `table_name(column_definitions)`"""
-204        if len(table_defs) > 0:
-205            table_names = self.get_table_names()
-206            for table in table_defs:
-207                if table.split("(")[0].strip() not in table_names:
-208                    self.cursor.execute(f"create table [{table}];")
-209                    self.logger.info(f'{table.split("(")[0]} table
+208        if len(table_defs) > 0:
+209            table_names = self.get_table_names()
+210            for table in table_defs:
+211                if table.split("(")[0].strip() not in table_names:
+212                    self.cursor.execute(f"create table [{table}];")
+213                    self.logger.info(f'{table.split("(")[0]} table
 created.')
-210
-211    @_connect
-212    def create_table(self, table: str, column_defs: list[str]):
-213        """Create a table if it doesn't exist.
 214
-215        #### :params:
-216
-217        `table`: Name of the table to create.
+215    @_connect
+216    def create_table(self, table: str, column_defs: list[str]):
+217        """Create a table if it doesn't exist.
 218
-219        `column_defs`: List of column definitions in proper Sqlite3 sytax.
-220        i.e. `"column_name text unique"` or `"column_name int primary key"`
+219        #### :params:
+220
+221        `table`: Name of the table to create.
+222
+223        `column_defs`: List of column definitions in proper Sqlite3 sytax.
+224        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
-221        if table not in self.get_table_names():
-222            query = f"create table [{table}]({', '.join(column_defs)});"
-223            self.cursor.execute(query)
-224            self.logger.info(f"'{table}' table created.")
-225
-226    @_connect
-227    def get_table_names(self) -> list[str]:
-228        """Returns a list of table names from the database."""
-229        self.cursor.execute(
-230            'select name from sqlite_Schema where type = "table" and name
+225        if table not in self.get_table_names():
+226            query = f"create table [{table}]({', '.join(column_defs)});"
+227            self.cursor.execute(query)
+228            self.logger.info(f"'{table}' table created.")
+229
+230    @_connect
+231    def get_table_names(self) -> list[str]:
+232        """Returns a list of table names from the database."""
+233        self.cursor.execute(
+234            'select name from sqlite_Schema where type = "table" and name
 not like "sqlite_%";'
-231        )
-232        return [result[0] for result in self.cursor.fetchall()]
-233
-234    @_connect
-235    def get_column_names(self, table: str) -> list[str]:
-236        """Return a list of column names from a table."""
-237        self.cursor.execute(f"select * from [{table}] where 1=0;")
-238        return [description[0] for description in self.cursor.description]
-239
-240    @_connect
-241    def count(
-242        self,
-243        table: str,
-244        match_criteria: list[tuple] | dict | None = None,
-245        exact_match: bool = True,
-246    ) -> int:
-247        """Return number of items in `table`.
-248
-249        #### :params:
-250
-251        `match_criteria`: Can be a list of 2-tuples where each
-252        tuple is `(columnName, rowValue)` or a dictionary where
-253        keys are column names and values are row values.
-254        If `None`, all rows from the table will be counted.
-255
-256        `exact_match`: If `False`, the row value for a given column
-257        in `match_criteria` will be matched as a substring.
-258        Has no effect if `match_criteria` is `None`.
-259        """
-260        query = f"select count(_rowid_) from [{table}]"
-261        try:
-262            if match_criteria:
-263                self.cursor.execute(
-264                    f"{query} where {self._get_conditions(match_criteria,
+235        )
+236        return [result[0] for result in self.cursor.fetchall()]
+237
+238    @_connect
+239    def get_column_names(self, table: str) -> list[str]:
+240        """Return a list of column names from a table."""
+241        self.cursor.execute(f"select * from [{table}] where 1=0;")
+242        return [description[0] for description in self.cursor.description]
+243
+244    @_connect
+245    def count(
+246        self,
+247        table: str,
+248        match_criteria: list[tuple] | dict | None = None,
+249        exact_match: bool = True,
+250    ) -> int:
+251        """Return number of items in `table`.
+252
+253        #### :params:
+254
+255        `match_criteria`: Can be a list of 2-tuples where each
+256        tuple is `(columnName, rowValue)` or a dictionary where
+257        keys are column names and values are row values.
+258        If `None`, all rows from the table will be counted.
+259
+260        `exact_match`: If `False`, the row value for a given column
+261        in `match_criteria` will be matched as a substring.
+262        Has no effect if `match_criteria` is `None`.
+263        """
+264        query = f"select count(_rowid_) from [{table}]"
+265        try:
+266            if match_criteria:
+267                self.cursor.execute(
+268                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)};"
-265                )
-266            else:
-267                self.cursor.execute(f"{query}")
-268            return self.cursor.fetchone()[0]
-269        except:
-270            return 0
-271
-272    @_connect
-273    def add_row(
-274        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+269                )
+270            else:
+271                self.cursor.execute(f"{query}")
+272            return self.cursor.fetchone()[0]
+273        except:
+274            return 0
+275
+276    @_connect
+277    def add_row(
+278        self, table: str, values: tuple[Any], columns: tuple[str] | None =
 None
-275    ) -> bool:
-276        """Add a row of values to a table.
-277
-278        Returns whether the addition was successful or not.
-279
-280        #### :params:
+279    ) -> bool:
+280        """Add a row of values to a table.
 281
-282        `table`: The table to insert values into.
+282        Returns whether the addition was successful or not.
 283
-284        `values`: A tuple of values to be inserted into the table.
+284        #### :params:
 285
-286        `columns`: If `None`, `values` is expected to supply a value for
+286        `table`: The table to insert values into.
+287
+288        `values`: A tuple of values to be inserted into the table.
+289
+290        `columns`: If `None`, `values` is expected to supply a value for
 every column in the table.
-287        If `columns` is provided, it should contain the same number of
+291        If `columns` is provided, it should contain the same number of
 elements as `values`."""
-288        parameterizer = ", ".join("?" for _ in values)
-289        logger_values = ", ".join(str(value) for value in values)
-290        try:
-291            if columns:
-292                columns_query = ", ".join(column for column in columns)
-293                self.cursor.execute(
-294                    f"insert into [{table}] ({columns_query}) values(
+292        parameterizer = ", ".join("?" for _ in values)
+293        logger_values = ", ".join(str(value) for value in values)
+294        try:
+295            if columns:
+296                columns_query = ", ".join(column for column in columns)
+297                self.cursor.execute(
+298                    f"insert into [{table}] ({columns_query}) values(
 {parameterizer});",
-295                    values,
-296                )
-297            else:
-298                self.cursor.execute(
-299                    f"insert into [{table}] values({parameterizer});",
-values
+299                    values,
 300                )
-301            self.logger.info(f'Added "{logger_values}" to {table} table.')
-302            return True
-303        except Exception as e:
-304            if "constraint" not in str(e).lower():
-305                self.logger.exception(
-306                    f'Error adding "{logger_values}" to {table} table.'
-307                )
-308            else:
-309                self.logger.debug(str(e))
-310            return False
-311
-312    @_connect
-313    def add_rows(
-314        self, table: str, values: list[tuple[Any]], columns: tuple[str] |
+301            else:
+302                self.cursor.execute(
+303                    f"insert into [{table}] values({parameterizer});",
+values
+304                )
+305            self.logger.info(f'Added "{logger_values}" to {table} table.')
+306            return True
+307        except Exception as e:
+308            if "constraint" not in str(e).lower():
+309                self.logger.exception(
+310                    f'Error adding "{logger_values}" to {table} table.'
+311                )
+312            else:
+313                self.logger.debug(str(e))
+314            return False
+315
+316    @_connect
+317    def add_rows(
+318        self, table: str, values: list[tuple[Any]], columns: tuple[str] |
 None = None
-315    ) -> tuple[int, int]:
-316        """Add multiple rows of values to a table.
-317
-318        Returns a tuple containing the number of successful additions and
-the number of failed additions.
-319
-320        #### :params:
+319    ) -> tuple[int, int]:
+320        """Add multiple rows of values to a table.
 321
-322        `table`: The table to insert values into.
+322        Returns a tuple containing the number of successful additions and
+the number of failed additions.
 323
-324        `values`: A list of tuples of values to be inserted into the table.
-325        Each tuple constitutes a single row to be inserted
-326
-327        `columns`: If `None`, `values` is expected to supply a value for
+324        #### :params:
+325
+326        `table`: The table to insert values into.
+327
+328        `values`: A list of tuples of values to be inserted into the table.
+329        Each tuple constitutes a single row to be inserted
+330
+331        `columns`: If `None`, `values` is expected to supply a value for
 every column in the table.
-328        If `columns` is provided, it should contain the same number of
+332        If `columns` is provided, it should contain the same number of
 elements as `values`."""
-329        successes = 0
-330        failures = 0
-331        for row in values:
-332            if self.add_row(table, row, columns):
-333                successes += 1
-334            else:
-335                failures += 1
-336        return (successes, failures)
-337
-338    @_connect
-339    def get_rows(
-340        self,
-341        table: str,
-342        match_criteria: list[tuple] | dict | None = None,
-343        exact_match: bool = True,
-344        sort_by_column: str | None = None,
-345        columns_to_return: list[str] | None = None,
-346        return_as_dataframe: bool = False,
-347        values_only: bool = False,
-348        order_by: str | None = None,
-349        limit: str | int | None = None,
-350    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-351        """Return matching rows from `table`.
-352
-353        By default, rows will be returned as a list of dictionaries of the
+333        successes = 0
+334        failures = 0
+335        for row in values:
+336            if self.add_row(table, row, columns):
+337                successes += 1
+338            else:
+339                failures += 1
+340        return (successes, failures)
+341
+342    @_connect
+343    def get_rows(
+344        self,
+345        table: str,
+346        match_criteria: list[tuple] | dict | None = None,
+347        exact_match: bool = True,
+348        sort_by_column: str | None = None,
+349        columns_to_return: list[str] | None = None,
+350        return_as_dataframe: bool = False,
+351        values_only: bool = False,
+352        order_by: str | None = None,
+353        limit: str | int | None = None,
+354    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+355        """Return matching rows from `table`.
+356
+357        By default, rows will be returned as a list of dictionaries of the
 form `[{"column_name": value, ...}, ...]`
-354
-355
-356        #### :params:
-357
-358        `match_criteria`: Can be a list of 2-tuples where each
-359        tuple is `(columnName, rowValue)` or a dictionary where
-360        keys are column names and values are row values.
+358
+359
+360        #### :params:
 361
-362        `exact_match`: If `False`, the row value for a given column will be
+362        `match_criteria`: Can be a list of 2-tuples where each
+363        tuple is `(columnName, rowValue)` or a dictionary where
+364        keys are column names and values are row values.
+365
+366        `exact_match`: If `False`, the row value for a given column will be
 matched as a substring.
-363
-364        `sort_by_column`: A column name to sort the results by.
-365        This will sort results in Python after retrieving them from the db.
-366        Use the 'order_by' param to use SQLite engine for ordering.
 367
-368        `columns_to_return`: Optional list of column names.
-369        If provided, the elements returned by this function will only
-contain the provided columns.
-370        Otherwise every column in the row is returned.
+368        `sort_by_column`: A column name to sort the results by.
+369        This will sort results in Python after retrieving them from the db.
+370        Use the 'order_by' param to use SQLite engine for ordering.
 371
-372        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
-object.
-373
-374        `values_only`: Return the results as a list of tuples.
+372        `columns_to_return`: Optional list of column names.
+373        If provided, the elements returned by this function will only
+contain the provided columns.
+374        Otherwise every column in the row is returned.
 375
-376        `order_by`: If given, a `order by {order_by}` clause will be added
-to the select query.
+376        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
+object.
 377
-378        `limit`: If given, a `limit {limit}` clause will be added to the
+378        `values_only`: Return the results as a list of tuples.
+379
+380        `order_by`: If given, a `order by {order_by}` clause will be added
+to the select query.
+381
+382        `limit`: If given, a `limit {limit}` clause will be added to the
 select query.
-379        """
-380
-381        if type(columns_to_return) is str:
-382            columns_to_return = [columns_to_return]
-383        query = f"select * from [{table}]"
-384        matches = []
-385        if match_criteria:
-386            query += f" where {self._get_conditions(match_criteria,
+383        """
+384
+385        if type(columns_to_return) is str:
+386            columns_to_return = [columns_to_return]
+387        query = f"select * from [{table}]"
+388        matches = []
+389        if match_criteria:
+390            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-387        if order_by:
-388            query += f" order by {order_by}"
-389        if limit:
-390            query += f" limit {limit}"
-391        query += ";"
-392        self.cursor.execute(query)
-393        matches = self.cursor.fetchall()
-394        results = [self._get_dict(table, match, columns_to_return) for match
+391        if order_by:
+392            query += f" order by {order_by}"
+393        if limit:
+394            query += f" limit {limit}"
+395        query += ";"
+396        self.cursor.execute(query)
+397        matches = self.cursor.fetchall()
+398        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-395        if sort_by_column:
-396            results = sorted(results, key=lambda x: x[sort_by_column])
-397        if return_as_dataframe:
-398            return pandas.DataFrame(results)
-399        if values_only:
-400            return [tuple(row.values()) for row in results]
-401        else:
-402            return results
-403
-404    @_connect
-405    def find(
-406        self, table: str, query_string: str, columns: list[str] | None =
+399        if sort_by_column:
+400            results = sorted(results, key=lambda x: x[sort_by_column])
+401        if return_as_dataframe:
+402            return pandas.DataFrame(results)
+403        if values_only:
+404            return [tuple(row.values()) for row in results]
+405        else:
+406            return results
+407
+408    @_connect
+409    def find(
+410        self, table: str, query_string: str, columns: list[str] | None =
 None
-407    ) -> list[dict]:
-408        """Search for rows that contain `query_string` as a substring of any
+411    ) -> list[dict]:
+412        """Search for rows that contain `query_string` as a substring of any
 column.
-409
-410        #### :params:
-411
-412        `table`: The table to search.
 413
-414        `query_string`: The substring to search for in all columns.
+414        #### :params:
 415
-416        `columns`: A list of columns to search for query_string.
-417        If None, all columns in the table will be searched.
-418        """
-419        if type(columns) is str:
-420            columns = [columns]
-421        results = []
-422        if not columns:
-423            columns = self.get_column_names(table)
-424        for column in columns:
-425            results.extend(
-426                [
-427                    row
-428                    for row in self.get_rows(
-429                        table, [(column, query_string)], exact_match=False
-430                    )
-431                    if row not in results
-432                ]
-433            )
-434        return results
-435
-436    @_connect
-437    def delete(
-438        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+416        `table`: The table to search.
+417
+418        `query_string`: The substring to search for in all columns.
+419
+420        `columns`: A list of columns to search for query_string.
+421        If None, all columns in the table will be searched.
+422        """
+423        if type(columns) is str:
+424            columns = [columns]
+425        results = []
+426        if not columns:
+427            columns = self.get_column_names(table)
+428        for column in columns:
+429            results.extend(
+430                [
+431                    row
+432                    for row in self.get_rows(
+433                        table, [(column, query_string)], exact_match=False
+434                    )
+435                    if row not in results
+436                ]
+437            )
+438        return results
+439
+440    @_connect
+441    def delete(
+442        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-439    ) -> int:
-440        """Delete records from `table`.
-441
-442        Returns the number of deleted records.
-443
-444        #### :params:
+443    ) -> int:
+444        """Delete records from `table`.
 445
-446        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+446        Returns the number of deleted records.
+447
+448        #### :params:
+449
+450        `match_criteria`: Can be a list of 2-tuples where each tuple is `
 (column_name, value)`
-447        or a dictionary where keys are column names and values are
+451        or a dictionary where keys are column names and values are
 corresponding values.
-448
-449        `exact_match`: If `False`, the value for a given column will be
+452
+453        `exact_match`: If `False`, the value for a given column will be
 matched as a substring.
-450        """
-451        conditions = self._get_conditions(match_criteria, exact_match)
-452        try:
-453            self.cursor.execute(f"delete from [{table}] where
+454        """
+455        conditions = self._get_conditions(match_criteria, exact_match)
+456        try:
+457            self.cursor.execute(f"delete from [{table}] where
 {conditions};")
-454            num_deletions = self.cursor.rowcount
-455            self.logger.info(
-456                f'Deleted {num_deletions} rows from "{table}" where
+458            num_deletions = self.cursor.rowcount
+459            self.logger.info(
+460                f'Deleted {num_deletions} rows from "{table}" where
 {conditions}".'
-457            )
-458            return num_deletions
-459        except Exception as e:
-460            self.logger.debug(
-461                f'Error deleting rows from "{table}" where {conditions}.\n
+461            )
+462            return num_deletions
+463        except Exception as e:
+464            self.logger.debug(
+465                f'Error deleting rows from "{table}" where {conditions}.\n
 {e}'
-462            )
-463            return 0
-464
-465    @_connect
-466    def update(
-467        self,
-468        table: str,
-469        column_to_update: str,
-470        new_value: Any,
-471        match_criteria: list[tuple] | dict | None = None,
-472        exact_match: bool = True,
-473    ) -> int:
-474        """Update the value in `column_to_update` to `new_value` for rows
+466            )
+467            return 0
+468
+469    @_connect
+470    def update(
+471        self,
+472        table: str,
+473        column_to_update: str,
+474        new_value: Any,
+475        match_criteria: list[tuple] | dict | None = None,
+476        exact_match: bool = True,
+477    ) -> int:
+478        """Update the value in `column_to_update` to `new_value` for rows
 matched with `match_criteria`.
-475
-476        #### :params:
-477
-478        `table`: The table to update rows in.
 479
-480        `column_to_update`: The column to be updated in the matched rows.
+480        #### :params:
 481
-482        `new_value`: The new value to insert.
+482        `table`: The table to update rows in.
 483
-484        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+484        `column_to_update`: The column to be updated in the matched rows.
+485
+486        `new_value`: The new value to insert.
+487
+488        `match_criteria`: Can be a list of 2-tuples where each tuple is `
 (columnName, rowValue)`
-485        or a dictionary where keys are column names and values are
+489        or a dictionary where keys are column names and values are
 corresponding values.
-486        If `None`, every row in `table` will be updated.
-487
-488        `exact_match`: If `False`, `match_criteria` values will be treated
+490        If `None`, every row in `table` will be updated.
+491
+492        `exact_match`: If `False`, `match_criteria` values will be treated
 as substrings.
-489
-490        Returns the number of updated rows."""
-491        query = f"update [{table}] set {column_to_update} = ?"
-492        conditions = ""
-493        if match_criteria:
-494            conditions = self._get_conditions(match_criteria, exact_match)
-495            query += f" where {conditions}"
-496        else:
-497            conditions = None
-498        query += ";"
-499        try:
-500            self.cursor.execute(
-501                query,
-502                (new_value,),
-503            )
-504            num_updates = self.cursor.rowcount
-505            self.logger.info(
-506                f'In {num_updates} rows, updated "{column_to_update}" in "
-{table}" table to "{new_value}" where {conditions}'
+493
+494        Returns the number of updated rows."""
+495        query = f"update [{table}] set {column_to_update} = ?"
+496        conditions = ""
+497        if match_criteria:
+498            conditions = self._get_conditions(match_criteria, exact_match)
+499            query += f" where {conditions}"
+500        else:
+501            conditions = None
+502        query += ";"
+503        try:
+504            self.cursor.execute(
+505                query,
+506                (new_value,),
 507            )
-508            return num_updates
-509        except Exception as e:
-510            self.logger.error(
-511                f'Failed to update "{column_to_update}" in "{table}" table
+508            num_updates = self.cursor.rowcount
+509            self.logger.info(
+510                f'In {num_updates} rows, updated "{column_to_update}" in "
+{table}" table to "{new_value}" where {conditions}'
+511            )
+512            return num_updates
+513        except Exception as e:
+514            self.logger.error(
+515                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-512            )
-513            return 0
-514
-515    @_connect
-516    def drop_table(self, table: str) -> bool:
-517        """Drop `table` from the database.
+516            )
+517            return 0
 518
-519        Returns `True` if successful, `False` if not."""
-520        try:
-521            self.cursor.execute(f"drop Table [{table}];")
-522            self.logger.info(f'Dropped table "{table}"')
-523            return True
-524        except Exception as e:
-525            print(e)
-526            self.logger.error(f'Failed to drop table "{table}"')
-527            return False
-528
-529    @_connect
-530    def add_column(
-531        self, table: str, column: str, _type: str, default_value: str | None
+519    @_connect
+520    def drop_table(self, table: str) -> bool:
+521        """Drop `table` from the database.
+522
+523        Returns `True` if successful, `False` if not."""
+524        try:
+525            self.cursor.execute(f"drop Table [{table}];")
+526            self.logger.info(f'Dropped table "{table}"')
+527            return True
+528        except Exception as e:
+529            print(e)
+530            self.logger.error(f'Failed to drop table "{table}"')
+531            return False
+532
+533    @_connect
+534    def add_column(
+535        self, table: str, column: str, _type: str, default_value: str | None
 = None
-532    ):
-533        """Add a new column to `table`.
-534
-535        #### :params:
-536
-537        `column`: Name of the column to add.
+536    ):
+537        """Add a new column to `table`.
 538
-539        `_type`: The data type of the new column.
+539        #### :params:
 540
-541        `default_value`: Optional default value for the column."""
-542        try:
-543            if default_value:
-544                self.cursor.execute(
-545                    f"alter table [{table}] add column {column} {_type}
+541        `column`: Name of the column to add.
+542
+543        `_type`: The data type of the new column.
+544
+545        `default_value`: Optional default value for the column."""
+546        try:
+547            if default_value:
+548                self.cursor.execute(
+549                    f"alter table [{table}] add column {column} {_type}
 default {default_value};"
-546                )
-547                self.update(table, column, default_value)
-548            else:
-549                self.cursor.execute(
-550                    f"alter table [{table}] add column {column} {_type};"
-551                )
-552            self.logger.info(f'Added column "{column}" to "{table}" table.')
-553        except Exception as e:
-554            self.logger.error(f'Failed to add column "{column}" to "{table}"
+550                )
+551                self.update(table, column, default_value)
+552            else:
+553                self.cursor.execute(
+554                    f"alter table [{table}] add column {column} {_type};"
+555                )
+556            self.logger.info(f'Added column "{column}" to "{table}" table.')
+557        except Exception as e:
+558            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
-555
-556    @staticmethod
-557    def data_to_string(
-558        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+559
+560    @staticmethod
+561    def data_to_string(
+562        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-559    ) -> str:
-560        """Uses tabulate to produce pretty string output from a list of
+563    ) -> str:
+564        """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-561
-562        #### :params:
-563
-564        `data`: The list of dictionaries to create a grid from.
-565        Assumes all dictionaries in list have the same set of keys.
-566
-567        `sort_key`: Optional dictionary key to sort data with.
-568
-569        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+565
+566        #### :params:
+567
+568        `data`: The list of dictionaries to create a grid from.
+569        Assumes all dictionaries in list have the same set of keys.
+570
+571        `sort_key`: Optional dictionary key to sort data with.
+572
+573        `wrap_to_terminal`: If `True`, the table width will be wrapped to
 fit within the current terminal window.
-570        Pass as `False` if the output is going into something like a `.txt`
+574        Pass as `False` if the output is going into something like a `.txt`
 file."""
-571        return data_to_string(data, sort_key, wrap_to_terminal)
-572
-573
-574def data_to_string(
-575    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
+575        return data_to_string(data, sort_key, wrap_to_terminal)
+576
+577
+578def data_to_string(
+579    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
 True
-576) -> str:
-577    """Uses tabulate to produce pretty string output from a list of
+580) -> str:
+581    """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-578
-579    #### :params:
-580
-581    `data`: The list of dictionaries to create a grid from.
-582    Assumes all dictionaries in list have the same set of keys.
-583
-584    `sort_key`: Optional dictionary key to sort data with.
-585
-586    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
+582
+583    #### :params:
+584
+585    `data`: The list of dictionaries to create a grid from.
+586    Assumes all dictionaries in list have the same set of keys.
+587
+588    `sort_key`: Optional dictionary key to sort data with.
+589
+590    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
 within the current terminal window.
-587    Pass as `False` if the output is going into something like a `.txt`
+591    Pass as `False` if the output is going into something like a `.txt`
 file."""
-588    if len(data) == 0:
-589        return ""
-590    if sort_key:
-591        data = sorted(data, key=lambda d: d[sort_key])
-592    for i, d in enumerate(data):
-593        for k in d:
-594            data[i][k] = str(data[i][k])
-595
-596    try:
-597        print("Resizing grid to fit within the terminal...\n")
-598        return griddy(data, "keys", wrap_to_terminal)
-599    except RuntimeError as e:
-600        print(e)
-601        return str(data)
+592    if len(data) == 0:
+593        return ""
+594    if sort_key:
+595        data = sorted(data, key=lambda d: d[sort_key])
+596    for i, d in enumerate(data):
+597        for k in d:
+598            data[i][k] = str(data[i][k])
+599
+600    try:
+601        print("Resizing grid to fit within the terminal...\n")
+602        return griddy(data, "keys", wrap_to_terminal)
+603    except RuntimeError as e:
+604        print(e)
+605        return str(data)
   ⁰
 class DataBased: View Source
 _46class DataBased:
 _47    """Sqli wrapper so queries don't need to be written except table
 definitions.
 _48
 _49    Supports saving and reading dates as datetime objects.
@@ -842,441 +846,445 @@
 183        else:
 184            conditions = " and ".join(
 185                f'"{column_row[0]}" like "%{column_row[1]}%"'
 186                for column_row in match_criteria
 187            )
 188        return f"({conditions})"
 189
-190    def vacuum(self):
-191        """Reduce disk size of the database with a `VACUUM` query."""
-192        self.query("VACUUM;")
-193
-194    @_connect
-195    def query(self, query_) -> list[Any]:
-196        """Execute an arbitrary query and return the results."""
-197        self.cursor.execute(query_)
-198        return self.cursor.fetchall()
-199
-200    @_connect
-201    def create_tables(self, table_defs: list[str] = []):
-202        """Create tables if they don't exist.
+190    def vacuum(self) -> int:
+191        """Reduce disk size of the database with a `VACUUM` query.
+192
+193        Returns space freed up in bytes."""
+194        size = self.dbpath.size
+195        self.query("VACUUM;")
+196        return size - self.dbpath.size
+197
+198    @_connect
+199    def query(self, query_) -> list[Any]:
+200        """Execute an arbitrary query and return the results."""
+201        self.cursor.execute(query_)
+202        return self.cursor.fetchall()
 203
-204        :param `table_defs`: Each definition should be in the form
+204    @_connect
+205    def create_tables(self, table_defs: list[str] = []):
+206        """Create tables if they don't exist.
+207
+208        :param `table_defs`: Each definition should be in the form
 `table_name(column_definitions)`"""
-205        if len(table_defs) > 0:
-206            table_names = self.get_table_names()
-207            for table in table_defs:
-208                if table.split("(")[0].strip() not in table_names:
-209                    self.cursor.execute(f"create table [{table}];")
-210                    self.logger.info(f'{table.split("(")[0]} table
+209        if len(table_defs) > 0:
+210            table_names = self.get_table_names()
+211            for table in table_defs:
+212                if table.split("(")[0].strip() not in table_names:
+213                    self.cursor.execute(f"create table [{table}];")
+214                    self.logger.info(f'{table.split("(")[0]} table
 created.')
-211
-212    @_connect
-213    def create_table(self, table: str, column_defs: list[str]):
-214        """Create a table if it doesn't exist.
 215
-216        #### :params:
-217
-218        `table`: Name of the table to create.
+216    @_connect
+217    def create_table(self, table: str, column_defs: list[str]):
+218        """Create a table if it doesn't exist.
 219
-220        `column_defs`: List of column definitions in proper Sqlite3 sytax.
-221        i.e. `"column_name text unique"` or `"column_name int primary key"`
+220        #### :params:
+221
+222        `table`: Name of the table to create.
+223
+224        `column_defs`: List of column definitions in proper Sqlite3 sytax.
+225        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
-222        if table not in self.get_table_names():
-223            query = f"create table [{table}]({', '.join(column_defs)});"
-224            self.cursor.execute(query)
-225            self.logger.info(f"'{table}' table created.")
-226
-227    @_connect
-228    def get_table_names(self) -> list[str]:
-229        """Returns a list of table names from the database."""
-230        self.cursor.execute(
-231            'select name from sqlite_Schema where type = "table" and name
+226        if table not in self.get_table_names():
+227            query = f"create table [{table}]({', '.join(column_defs)});"
+228            self.cursor.execute(query)
+229            self.logger.info(f"'{table}' table created.")
+230
+231    @_connect
+232    def get_table_names(self) -> list[str]:
+233        """Returns a list of table names from the database."""
+234        self.cursor.execute(
+235            'select name from sqlite_Schema where type = "table" and name
 not like "sqlite_%";'
-232        )
-233        return [result[0] for result in self.cursor.fetchall()]
-234
-235    @_connect
-236    def get_column_names(self, table: str) -> list[str]:
-237        """Return a list of column names from a table."""
-238        self.cursor.execute(f"select * from [{table}] where 1=0;")
-239        return [description[0] for description in self.cursor.description]
-240
-241    @_connect
-242    def count(
-243        self,
-244        table: str,
-245        match_criteria: list[tuple] | dict | None = None,
-246        exact_match: bool = True,
-247    ) -> int:
-248        """Return number of items in `table`.
-249
-250        #### :params:
-251
-252        `match_criteria`: Can be a list of 2-tuples where each
-253        tuple is `(columnName, rowValue)` or a dictionary where
-254        keys are column names and values are row values.
-255        If `None`, all rows from the table will be counted.
-256
-257        `exact_match`: If `False`, the row value for a given column
-258        in `match_criteria` will be matched as a substring.
-259        Has no effect if `match_criteria` is `None`.
-260        """
-261        query = f"select count(_rowid_) from [{table}]"
-262        try:
-263            if match_criteria:
-264                self.cursor.execute(
-265                    f"{query} where {self._get_conditions(match_criteria,
+236        )
+237        return [result[0] for result in self.cursor.fetchall()]
+238
+239    @_connect
+240    def get_column_names(self, table: str) -> list[str]:
+241        """Return a list of column names from a table."""
+242        self.cursor.execute(f"select * from [{table}] where 1=0;")
+243        return [description[0] for description in self.cursor.description]
+244
+245    @_connect
+246    def count(
+247        self,
+248        table: str,
+249        match_criteria: list[tuple] | dict | None = None,
+250        exact_match: bool = True,
+251    ) -> int:
+252        """Return number of items in `table`.
+253
+254        #### :params:
+255
+256        `match_criteria`: Can be a list of 2-tuples where each
+257        tuple is `(columnName, rowValue)` or a dictionary where
+258        keys are column names and values are row values.
+259        If `None`, all rows from the table will be counted.
+260
+261        `exact_match`: If `False`, the row value for a given column
+262        in `match_criteria` will be matched as a substring.
+263        Has no effect if `match_criteria` is `None`.
+264        """
+265        query = f"select count(_rowid_) from [{table}]"
+266        try:
+267            if match_criteria:
+268                self.cursor.execute(
+269                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)};"
-266                )
-267            else:
-268                self.cursor.execute(f"{query}")
-269            return self.cursor.fetchone()[0]
-270        except:
-271            return 0
-272
-273    @_connect
-274    def add_row(
-275        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+270                )
+271            else:
+272                self.cursor.execute(f"{query}")
+273            return self.cursor.fetchone()[0]
+274        except:
+275            return 0
+276
+277    @_connect
+278    def add_row(
+279        self, table: str, values: tuple[Any], columns: tuple[str] | None =
 None
-276    ) -> bool:
-277        """Add a row of values to a table.
-278
-279        Returns whether the addition was successful or not.
-280
-281        #### :params:
+280    ) -> bool:
+281        """Add a row of values to a table.
 282
-283        `table`: The table to insert values into.
+283        Returns whether the addition was successful or not.
 284
-285        `values`: A tuple of values to be inserted into the table.
+285        #### :params:
 286
-287        `columns`: If `None`, `values` is expected to supply a value for
+287        `table`: The table to insert values into.
+288
+289        `values`: A tuple of values to be inserted into the table.
+290
+291        `columns`: If `None`, `values` is expected to supply a value for
 every column in the table.
-288        If `columns` is provided, it should contain the same number of
+292        If `columns` is provided, it should contain the same number of
 elements as `values`."""
-289        parameterizer = ", ".join("?" for _ in values)
-290        logger_values = ", ".join(str(value) for value in values)
-291        try:
-292            if columns:
-293                columns_query = ", ".join(column for column in columns)
-294                self.cursor.execute(
-295                    f"insert into [{table}] ({columns_query}) values(
+293        parameterizer = ", ".join("?" for _ in values)
+294        logger_values = ", ".join(str(value) for value in values)
+295        try:
+296            if columns:
+297                columns_query = ", ".join(column for column in columns)
+298                self.cursor.execute(
+299                    f"insert into [{table}] ({columns_query}) values(
 {parameterizer});",
-296                    values,
-297                )
-298            else:
-299                self.cursor.execute(
-300                    f"insert into [{table}] values({parameterizer});",
-values
+300                    values,
 301                )
-302            self.logger.info(f'Added "{logger_values}" to {table} table.')
-303            return True
-304        except Exception as e:
-305            if "constraint" not in str(e).lower():
-306                self.logger.exception(
-307                    f'Error adding "{logger_values}" to {table} table.'
-308                )
-309            else:
-310                self.logger.debug(str(e))
-311            return False
-312
-313    @_connect
-314    def add_rows(
-315        self, table: str, values: list[tuple[Any]], columns: tuple[str] |
+302            else:
+303                self.cursor.execute(
+304                    f"insert into [{table}] values({parameterizer});",
+values
+305                )
+306            self.logger.info(f'Added "{logger_values}" to {table} table.')
+307            return True
+308        except Exception as e:
+309            if "constraint" not in str(e).lower():
+310                self.logger.exception(
+311                    f'Error adding "{logger_values}" to {table} table.'
+312                )
+313            else:
+314                self.logger.debug(str(e))
+315            return False
+316
+317    @_connect
+318    def add_rows(
+319        self, table: str, values: list[tuple[Any]], columns: tuple[str] |
 None = None
-316    ) -> tuple[int, int]:
-317        """Add multiple rows of values to a table.
-318
-319        Returns a tuple containing the number of successful additions and
-the number of failed additions.
-320
-321        #### :params:
+320    ) -> tuple[int, int]:
+321        """Add multiple rows of values to a table.
 322
-323        `table`: The table to insert values into.
+323        Returns a tuple containing the number of successful additions and
+the number of failed additions.
 324
-325        `values`: A list of tuples of values to be inserted into the table.
-326        Each tuple constitutes a single row to be inserted
-327
-328        `columns`: If `None`, `values` is expected to supply a value for
+325        #### :params:
+326
+327        `table`: The table to insert values into.
+328
+329        `values`: A list of tuples of values to be inserted into the table.
+330        Each tuple constitutes a single row to be inserted
+331
+332        `columns`: If `None`, `values` is expected to supply a value for
 every column in the table.
-329        If `columns` is provided, it should contain the same number of
+333        If `columns` is provided, it should contain the same number of
 elements as `values`."""
-330        successes = 0
-331        failures = 0
-332        for row in values:
-333            if self.add_row(table, row, columns):
-334                successes += 1
-335            else:
-336                failures += 1
-337        return (successes, failures)
-338
-339    @_connect
-340    def get_rows(
-341        self,
-342        table: str,
-343        match_criteria: list[tuple] | dict | None = None,
-344        exact_match: bool = True,
-345        sort_by_column: str | None = None,
-346        columns_to_return: list[str] | None = None,
-347        return_as_dataframe: bool = False,
-348        values_only: bool = False,
-349        order_by: str | None = None,
-350        limit: str | int | None = None,
-351    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-352        """Return matching rows from `table`.
-353
-354        By default, rows will be returned as a list of dictionaries of the
+334        successes = 0
+335        failures = 0
+336        for row in values:
+337            if self.add_row(table, row, columns):
+338                successes += 1
+339            else:
+340                failures += 1
+341        return (successes, failures)
+342
+343    @_connect
+344    def get_rows(
+345        self,
+346        table: str,
+347        match_criteria: list[tuple] | dict | None = None,
+348        exact_match: bool = True,
+349        sort_by_column: str | None = None,
+350        columns_to_return: list[str] | None = None,
+351        return_as_dataframe: bool = False,
+352        values_only: bool = False,
+353        order_by: str | None = None,
+354        limit: str | int | None = None,
+355    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+356        """Return matching rows from `table`.
+357
+358        By default, rows will be returned as a list of dictionaries of the
 form `[{"column_name": value, ...}, ...]`
-355
-356
-357        #### :params:
-358
-359        `match_criteria`: Can be a list of 2-tuples where each
-360        tuple is `(columnName, rowValue)` or a dictionary where
-361        keys are column names and values are row values.
+359
+360
+361        #### :params:
 362
-363        `exact_match`: If `False`, the row value for a given column will be
+363        `match_criteria`: Can be a list of 2-tuples where each
+364        tuple is `(columnName, rowValue)` or a dictionary where
+365        keys are column names and values are row values.
+366
+367        `exact_match`: If `False`, the row value for a given column will be
 matched as a substring.
-364
-365        `sort_by_column`: A column name to sort the results by.
-366        This will sort results in Python after retrieving them from the db.
-367        Use the 'order_by' param to use SQLite engine for ordering.
 368
-369        `columns_to_return`: Optional list of column names.
-370        If provided, the elements returned by this function will only
-contain the provided columns.
-371        Otherwise every column in the row is returned.
+369        `sort_by_column`: A column name to sort the results by.
+370        This will sort results in Python after retrieving them from the db.
+371        Use the 'order_by' param to use SQLite engine for ordering.
 372
-373        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
-object.
-374
-375        `values_only`: Return the results as a list of tuples.
+373        `columns_to_return`: Optional list of column names.
+374        If provided, the elements returned by this function will only
+contain the provided columns.
+375        Otherwise every column in the row is returned.
 376
-377        `order_by`: If given, a `order by {order_by}` clause will be added
-to the select query.
+377        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
+object.
 378
-379        `limit`: If given, a `limit {limit}` clause will be added to the
+379        `values_only`: Return the results as a list of tuples.
+380
+381        `order_by`: If given, a `order by {order_by}` clause will be added
+to the select query.
+382
+383        `limit`: If given, a `limit {limit}` clause will be added to the
 select query.
-380        """
-381
-382        if type(columns_to_return) is str:
-383            columns_to_return = [columns_to_return]
-384        query = f"select * from [{table}]"
-385        matches = []
-386        if match_criteria:
-387            query += f" where {self._get_conditions(match_criteria,
+384        """
+385
+386        if type(columns_to_return) is str:
+387            columns_to_return = [columns_to_return]
+388        query = f"select * from [{table}]"
+389        matches = []
+390        if match_criteria:
+391            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-388        if order_by:
-389            query += f" order by {order_by}"
-390        if limit:
-391            query += f" limit {limit}"
-392        query += ";"
-393        self.cursor.execute(query)
-394        matches = self.cursor.fetchall()
-395        results = [self._get_dict(table, match, columns_to_return) for match
+392        if order_by:
+393            query += f" order by {order_by}"
+394        if limit:
+395            query += f" limit {limit}"
+396        query += ";"
+397        self.cursor.execute(query)
+398        matches = self.cursor.fetchall()
+399        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-396        if sort_by_column:
-397            results = sorted(results, key=lambda x: x[sort_by_column])
-398        if return_as_dataframe:
-399            return pandas.DataFrame(results)
-400        if values_only:
-401            return [tuple(row.values()) for row in results]
-402        else:
-403            return results
-404
-405    @_connect
-406    def find(
-407        self, table: str, query_string: str, columns: list[str] | None =
+400        if sort_by_column:
+401            results = sorted(results, key=lambda x: x[sort_by_column])
+402        if return_as_dataframe:
+403            return pandas.DataFrame(results)
+404        if values_only:
+405            return [tuple(row.values()) for row in results]
+406        else:
+407            return results
+408
+409    @_connect
+410    def find(
+411        self, table: str, query_string: str, columns: list[str] | None =
 None
-408    ) -> list[dict]:
-409        """Search for rows that contain `query_string` as a substring of any
+412    ) -> list[dict]:
+413        """Search for rows that contain `query_string` as a substring of any
 column.
-410
-411        #### :params:
-412
-413        `table`: The table to search.
 414
-415        `query_string`: The substring to search for in all columns.
+415        #### :params:
 416
-417        `columns`: A list of columns to search for query_string.
-418        If None, all columns in the table will be searched.
-419        """
-420        if type(columns) is str:
-421            columns = [columns]
-422        results = []
-423        if not columns:
-424            columns = self.get_column_names(table)
-425        for column in columns:
-426            results.extend(
-427                [
-428                    row
-429                    for row in self.get_rows(
-430                        table, [(column, query_string)], exact_match=False
-431                    )
-432                    if row not in results
-433                ]
-434            )
-435        return results
-436
-437    @_connect
-438    def delete(
-439        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+417        `table`: The table to search.
+418
+419        `query_string`: The substring to search for in all columns.
+420
+421        `columns`: A list of columns to search for query_string.
+422        If None, all columns in the table will be searched.
+423        """
+424        if type(columns) is str:
+425            columns = [columns]
+426        results = []
+427        if not columns:
+428            columns = self.get_column_names(table)
+429        for column in columns:
+430            results.extend(
+431                [
+432                    row
+433                    for row in self.get_rows(
+434                        table, [(column, query_string)], exact_match=False
+435                    )
+436                    if row not in results
+437                ]
+438            )
+439        return results
+440
+441    @_connect
+442    def delete(
+443        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-440    ) -> int:
-441        """Delete records from `table`.
-442
-443        Returns the number of deleted records.
-444
-445        #### :params:
+444    ) -> int:
+445        """Delete records from `table`.
 446
-447        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+447        Returns the number of deleted records.
+448
+449        #### :params:
+450
+451        `match_criteria`: Can be a list of 2-tuples where each tuple is `
 (column_name, value)`
-448        or a dictionary where keys are column names and values are
+452        or a dictionary where keys are column names and values are
 corresponding values.
-449
-450        `exact_match`: If `False`, the value for a given column will be
+453
+454        `exact_match`: If `False`, the value for a given column will be
 matched as a substring.
-451        """
-452        conditions = self._get_conditions(match_criteria, exact_match)
-453        try:
-454            self.cursor.execute(f"delete from [{table}] where
+455        """
+456        conditions = self._get_conditions(match_criteria, exact_match)
+457        try:
+458            self.cursor.execute(f"delete from [{table}] where
 {conditions};")
-455            num_deletions = self.cursor.rowcount
-456            self.logger.info(
-457                f'Deleted {num_deletions} rows from "{table}" where
+459            num_deletions = self.cursor.rowcount
+460            self.logger.info(
+461                f'Deleted {num_deletions} rows from "{table}" where
 {conditions}".'
-458            )
-459            return num_deletions
-460        except Exception as e:
-461            self.logger.debug(
-462                f'Error deleting rows from "{table}" where {conditions}.\n
+462            )
+463            return num_deletions
+464        except Exception as e:
+465            self.logger.debug(
+466                f'Error deleting rows from "{table}" where {conditions}.\n
 {e}'
-463            )
-464            return 0
-465
-466    @_connect
-467    def update(
-468        self,
-469        table: str,
-470        column_to_update: str,
-471        new_value: Any,
-472        match_criteria: list[tuple] | dict | None = None,
-473        exact_match: bool = True,
-474    ) -> int:
-475        """Update the value in `column_to_update` to `new_value` for rows
+467            )
+468            return 0
+469
+470    @_connect
+471    def update(
+472        self,
+473        table: str,
+474        column_to_update: str,
+475        new_value: Any,
+476        match_criteria: list[tuple] | dict | None = None,
+477        exact_match: bool = True,
+478    ) -> int:
+479        """Update the value in `column_to_update` to `new_value` for rows
 matched with `match_criteria`.
-476
-477        #### :params:
-478
-479        `table`: The table to update rows in.
 480
-481        `column_to_update`: The column to be updated in the matched rows.
+481        #### :params:
 482
-483        `new_value`: The new value to insert.
+483        `table`: The table to update rows in.
 484
-485        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+485        `column_to_update`: The column to be updated in the matched rows.
+486
+487        `new_value`: The new value to insert.
+488
+489        `match_criteria`: Can be a list of 2-tuples where each tuple is `
 (columnName, rowValue)`
-486        or a dictionary where keys are column names and values are
+490        or a dictionary where keys are column names and values are
 corresponding values.
-487        If `None`, every row in `table` will be updated.
-488
-489        `exact_match`: If `False`, `match_criteria` values will be treated
+491        If `None`, every row in `table` will be updated.
+492
+493        `exact_match`: If `False`, `match_criteria` values will be treated
 as substrings.
-490
-491        Returns the number of updated rows."""
-492        query = f"update [{table}] set {column_to_update} = ?"
-493        conditions = ""
-494        if match_criteria:
-495            conditions = self._get_conditions(match_criteria, exact_match)
-496            query += f" where {conditions}"
-497        else:
-498            conditions = None
-499        query += ";"
-500        try:
-501            self.cursor.execute(
-502                query,
-503                (new_value,),
-504            )
-505            num_updates = self.cursor.rowcount
-506            self.logger.info(
-507                f'In {num_updates} rows, updated "{column_to_update}" in "
-{table}" table to "{new_value}" where {conditions}'
+494
+495        Returns the number of updated rows."""
+496        query = f"update [{table}] set {column_to_update} = ?"
+497        conditions = ""
+498        if match_criteria:
+499            conditions = self._get_conditions(match_criteria, exact_match)
+500            query += f" where {conditions}"
+501        else:
+502            conditions = None
+503        query += ";"
+504        try:
+505            self.cursor.execute(
+506                query,
+507                (new_value,),
 508            )
-509            return num_updates
-510        except Exception as e:
-511            self.logger.error(
-512                f'Failed to update "{column_to_update}" in "{table}" table
+509            num_updates = self.cursor.rowcount
+510            self.logger.info(
+511                f'In {num_updates} rows, updated "{column_to_update}" in "
+{table}" table to "{new_value}" where {conditions}'
+512            )
+513            return num_updates
+514        except Exception as e:
+515            self.logger.error(
+516                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-513            )
-514            return 0
-515
-516    @_connect
-517    def drop_table(self, table: str) -> bool:
-518        """Drop `table` from the database.
+517            )
+518            return 0
 519
-520        Returns `True` if successful, `False` if not."""
-521        try:
-522            self.cursor.execute(f"drop Table [{table}];")
-523            self.logger.info(f'Dropped table "{table}"')
-524            return True
-525        except Exception as e:
-526            print(e)
-527            self.logger.error(f'Failed to drop table "{table}"')
-528            return False
-529
-530    @_connect
-531    def add_column(
-532        self, table: str, column: str, _type: str, default_value: str | None
+520    @_connect
+521    def drop_table(self, table: str) -> bool:
+522        """Drop `table` from the database.
+523
+524        Returns `True` if successful, `False` if not."""
+525        try:
+526            self.cursor.execute(f"drop Table [{table}];")
+527            self.logger.info(f'Dropped table "{table}"')
+528            return True
+529        except Exception as e:
+530            print(e)
+531            self.logger.error(f'Failed to drop table "{table}"')
+532            return False
+533
+534    @_connect
+535    def add_column(
+536        self, table: str, column: str, _type: str, default_value: str | None
 = None
-533    ):
-534        """Add a new column to `table`.
-535
-536        #### :params:
-537
-538        `column`: Name of the column to add.
+537    ):
+538        """Add a new column to `table`.
 539
-540        `_type`: The data type of the new column.
+540        #### :params:
 541
-542        `default_value`: Optional default value for the column."""
-543        try:
-544            if default_value:
-545                self.cursor.execute(
-546                    f"alter table [{table}] add column {column} {_type}
+542        `column`: Name of the column to add.
+543
+544        `_type`: The data type of the new column.
+545
+546        `default_value`: Optional default value for the column."""
+547        try:
+548            if default_value:
+549                self.cursor.execute(
+550                    f"alter table [{table}] add column {column} {_type}
 default {default_value};"
-547                )
-548                self.update(table, column, default_value)
-549            else:
-550                self.cursor.execute(
-551                    f"alter table [{table}] add column {column} {_type};"
-552                )
-553            self.logger.info(f'Added column "{column}" to "{table}" table.')
-554        except Exception as e:
-555            self.logger.error(f'Failed to add column "{column}" to "{table}"
+551                )
+552                self.update(table, column, default_value)
+553            else:
+554                self.cursor.execute(
+555                    f"alter table [{table}] add column {column} {_type};"
+556                )
+557            self.logger.info(f'Added column "{column}" to "{table}" table.')
+558        except Exception as e:
+559            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
-556
-557    @staticmethod
-558    def data_to_string(
-559        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+560
+561    @staticmethod
+562    def data_to_string(
+563        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-560    ) -> str:
-561        """Uses tabulate to produce pretty string output from a list of
+564    ) -> str:
+565        """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-562
-563        #### :params:
-564
-565        `data`: The list of dictionaries to create a grid from.
-566        Assumes all dictionaries in list have the same set of keys.
-567
-568        `sort_key`: Optional dictionary key to sort data with.
-569
-570        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+566
+567        #### :params:
+568
+569        `data`: The list of dictionaries to create a grid from.
+570        Assumes all dictionaries in list have the same set of keys.
+571
+572        `sort_key`: Optional dictionary key to sort data with.
+573
+574        `wrap_to_terminal`: If `True`, the table width will be wrapped to
 fit within the current terminal window.
-571        Pass as `False` if the output is going into something like a `.txt`
+575        Pass as `False` if the output is going into something like a `.txt`
 file."""
-572        return data_to_string(data, sort_key, wrap_to_terminal)
+576        return data_to_string(data, sort_key, wrap_to_terminal)
 Sqli wrapper so queries don't need to be written except table definitions.
 Supports saving and reading dates as datetime objects.
 Supports using a context manager.
 ⁰
 DataBased(
 dbpath: str | pathier.pathier.Pathier,
 logger_encoding: str = 'utf-8',
@@ -1341,225 +1349,230 @@
 115            self.connection.commit()
 116            self.connection.close()
 117            self.connection_open = False
 Save and close connection to db.
 Call this as soon as you are done using the database if you have multiple
 threads or processes using the same database.
 ⁰
-def vacuum(self): View Source
-190    def vacuum(self):
-191        """Reduce disk size of the database with a `VACUUM` query."""
-192        self.query("VACUUM;")
+def vacuum(self) -> int: View Source
+190    def vacuum(self) -> int:
+191        """Reduce disk size of the database with a `VACUUM` query.
+192
+193        Returns space freed up in bytes."""
+194        size = self.dbpath.size
+195        self.query("VACUUM;")
+196        return size - self.dbpath.size
 Reduce disk size of the database with a VACUUM query.
+Returns space freed up in bytes.
 ⁰
 def query(self, query_) -> list[typing.Any]: View Source
-194    @_connect
-195    def query(self, query_) -> list[Any]:
-196        """Execute an arbitrary query and return the results."""
-197        self.cursor.execute(query_)
-198        return self.cursor.fetchall()
+198    @_connect
+199    def query(self, query_) -> list[Any]:
+200        """Execute an arbitrary query and return the results."""
+201        self.cursor.execute(query_)
+202        return self.cursor.fetchall()
 Execute an arbitrary query and return the results.
 ⁰
 def create_tables(self, table_defs: list[str] = []): View Source
-200    @_connect
-201    def create_tables(self, table_defs: list[str] = []):
-202        """Create tables if they don't exist.
-203
-204        :param `table_defs`: Each definition should be in the form
+204    @_connect
+205    def create_tables(self, table_defs: list[str] = []):
+206        """Create tables if they don't exist.
+207
+208        :param `table_defs`: Each definition should be in the form
 `table_name(column_definitions)`"""
-205        if len(table_defs) > 0:
-206            table_names = self.get_table_names()
-207            for table in table_defs:
-208                if table.split("(")[0].strip() not in table_names:
-209                    self.cursor.execute(f"create table [{table}];")
-210                    self.logger.info(f'{table.split("(")[0]} table
+209        if len(table_defs) > 0:
+210            table_names = self.get_table_names()
+211            for table in table_defs:
+212                if table.split("(")[0].strip() not in table_names:
+213                    self.cursor.execute(f"create table [{table}];")
+214                    self.logger.info(f'{table.split("(")[0]} table
 created.')
 Create tables if they don't exist.
 * Parameters *
     * table_defs: Each definition should be in the form table_name
       (column_definitions)
 ⁰
 def create_table(self, table: str, column_defs: list[str]): View Source
-212    @_connect
-213    def create_table(self, table: str, column_defs: list[str]):
-214        """Create a table if it doesn't exist.
-215
-216        #### :params:
-217
-218        `table`: Name of the table to create.
+216    @_connect
+217    def create_table(self, table: str, column_defs: list[str]):
+218        """Create a table if it doesn't exist.
 219
-220        `column_defs`: List of column definitions in proper Sqlite3 sytax.
-221        i.e. `"column_name text unique"` or `"column_name int primary key"`
+220        #### :params:
+221
+222        `table`: Name of the table to create.
+223
+224        `column_defs`: List of column definitions in proper Sqlite3 sytax.
+225        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
-222        if table not in self.get_table_names():
-223            query = f"create table [{table}]({', '.join(column_defs)});"
-224            self.cursor.execute(query)
-225            self.logger.info(f"'{table}' table created.")
+226        if table not in self.get_table_names():
+227            query = f"create table [{table}]({', '.join(column_defs)});"
+228            self.cursor.execute(query)
+229            self.logger.info(f"'{table}' table created.")
 Create a table if it doesn't exist.
 *** :params: ***
 table: Name of the table to create.
 column_defs: List of column definitions in proper Sqlite3 sytax. i.e.
 "column_name text unique" or "column_name int primary key" etc.
 ⁰
 def get_table_names(self) -> list[str]: View Source
-227    @_connect
-228    def get_table_names(self) -> list[str]:
-229        """Returns a list of table names from the database."""
-230        self.cursor.execute(
-231            'select name from sqlite_Schema where type = "table" and name
+231    @_connect
+232    def get_table_names(self) -> list[str]:
+233        """Returns a list of table names from the database."""
+234        self.cursor.execute(
+235            'select name from sqlite_Schema where type = "table" and name
 not like "sqlite_%";'
-232        )
-233        return [result[0] for result in self.cursor.fetchall()]
+236        )
+237        return [result[0] for result in self.cursor.fetchall()]
 Returns a list of table names from the database.
 ⁰
 def get_column_names(self, table: str) -> list[str]: View Source
-235    @_connect
-236    def get_column_names(self, table: str) -> list[str]:
-237        """Return a list of column names from a table."""
-238        self.cursor.execute(f"select * from [{table}] where 1=0;")
-239        return [description[0] for description in self.cursor.description]
+239    @_connect
+240    def get_column_names(self, table: str) -> list[str]:
+241        """Return a list of column names from a table."""
+242        self.cursor.execute(f"select * from [{table}] where 1=0;")
+243        return [description[0] for description in self.cursor.description]
 Return a list of column names from a table.
 ⁰
 def count(
 self,
 table: str,
 match_criteria: list[tuple] | dict | None = None,
 exact_match: bool = True) -> int: View Source
-241    @_connect
-242    def count(
-243        self,
-244        table: str,
-245        match_criteria: list[tuple] | dict | None = None,
-246        exact_match: bool = True,
-247    ) -> int:
-248        """Return number of items in `table`.
-249
-250        #### :params:
-251
-252        `match_criteria`: Can be a list of 2-tuples where each
-253        tuple is `(columnName, rowValue)` or a dictionary where
-254        keys are column names and values are row values.
-255        If `None`, all rows from the table will be counted.
-256
-257        `exact_match`: If `False`, the row value for a given column
-258        in `match_criteria` will be matched as a substring.
-259        Has no effect if `match_criteria` is `None`.
-260        """
-261        query = f"select count(_rowid_) from [{table}]"
-262        try:
-263            if match_criteria:
-264                self.cursor.execute(
-265                    f"{query} where {self._get_conditions(match_criteria,
+245    @_connect
+246    def count(
+247        self,
+248        table: str,
+249        match_criteria: list[tuple] | dict | None = None,
+250        exact_match: bool = True,
+251    ) -> int:
+252        """Return number of items in `table`.
+253
+254        #### :params:
+255
+256        `match_criteria`: Can be a list of 2-tuples where each
+257        tuple is `(columnName, rowValue)` or a dictionary where
+258        keys are column names and values are row values.
+259        If `None`, all rows from the table will be counted.
+260
+261        `exact_match`: If `False`, the row value for a given column
+262        in `match_criteria` will be matched as a substring.
+263        Has no effect if `match_criteria` is `None`.
+264        """
+265        query = f"select count(_rowid_) from [{table}]"
+266        try:
+267            if match_criteria:
+268                self.cursor.execute(
+269                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)};"
-266                )
-267            else:
-268                self.cursor.execute(f"{query}")
-269            return self.cursor.fetchone()[0]
-270        except:
-271            return 0
+270                )
+271            else:
+272                self.cursor.execute(f"{query}")
+273            return self.cursor.fetchone()[0]
+274        except:
+275            return 0
 Return number of items in table.
 *** :params: ***
 match_criteria: Can be a list of 2-tuples where each tuple is (columnName,
 rowValue) or a dictionary where keys are column names and values are row
 values. If None, all rows from the table will be counted.
 exact_match: If False, the row value for a given column in match_criteria will
 be matched as a substring. Has no effect if match_criteria is None.
 ⁰
 def add_row(
 self,
 table: str,
 values: tuple[typing.Any],
 columns: tuple[str] | None = None) -> bool: View Source
-273    @_connect
-274    def add_row(
-275        self, table: str, values: tuple[Any], columns: tuple[str] | None =
+277    @_connect
+278    def add_row(
+279        self, table: str, values: tuple[Any], columns: tuple[str] | None =
 None
-276    ) -> bool:
-277        """Add a row of values to a table.
-278
-279        Returns whether the addition was successful or not.
-280
-281        #### :params:
+280    ) -> bool:
+281        """Add a row of values to a table.
 282
-283        `table`: The table to insert values into.
+283        Returns whether the addition was successful or not.
 284
-285        `values`: A tuple of values to be inserted into the table.
+285        #### :params:
 286
-287        `columns`: If `None`, `values` is expected to supply a value for
+287        `table`: The table to insert values into.
+288
+289        `values`: A tuple of values to be inserted into the table.
+290
+291        `columns`: If `None`, `values` is expected to supply a value for
 every column in the table.
-288        If `columns` is provided, it should contain the same number of
+292        If `columns` is provided, it should contain the same number of
 elements as `values`."""
-289        parameterizer = ", ".join("?" for _ in values)
-290        logger_values = ", ".join(str(value) for value in values)
-291        try:
-292            if columns:
-293                columns_query = ", ".join(column for column in columns)
-294                self.cursor.execute(
-295                    f"insert into [{table}] ({columns_query}) values(
+293        parameterizer = ", ".join("?" for _ in values)
+294        logger_values = ", ".join(str(value) for value in values)
+295        try:
+296            if columns:
+297                columns_query = ", ".join(column for column in columns)
+298                self.cursor.execute(
+299                    f"insert into [{table}] ({columns_query}) values(
 {parameterizer});",
-296                    values,
-297                )
-298            else:
-299                self.cursor.execute(
-300                    f"insert into [{table}] values({parameterizer});",
-values
+300                    values,
 301                )
-302            self.logger.info(f'Added "{logger_values}" to {table} table.')
-303            return True
-304        except Exception as e:
-305            if "constraint" not in str(e).lower():
-306                self.logger.exception(
-307                    f'Error adding "{logger_values}" to {table} table.'
-308                )
-309            else:
-310                self.logger.debug(str(e))
-311            return False
+302            else:
+303                self.cursor.execute(
+304                    f"insert into [{table}] values({parameterizer});",
+values
+305                )
+306            self.logger.info(f'Added "{logger_values}" to {table} table.')
+307            return True
+308        except Exception as e:
+309            if "constraint" not in str(e).lower():
+310                self.logger.exception(
+311                    f'Error adding "{logger_values}" to {table} table.'
+312                )
+313            else:
+314                self.logger.debug(str(e))
+315            return False
 Add a row of values to a table.
 Returns whether the addition was successful or not.
 *** :params: ***
 table: The table to insert values into.
 values: A tuple of values to be inserted into the table.
 columns: If None, values is expected to supply a value for every column in the
 table. If columns is provided, it should contain the same number of elements as
 values.
 ⁰
 def add_rows(
 self,
 table: str,
 values: list[tuple[typing.Any]],
 columns: tuple[str] | None = None) -> tuple[int, int]: View Source
-313    @_connect
-314    def add_rows(
-315        self, table: str, values: list[tuple[Any]], columns: tuple[str] |
+317    @_connect
+318    def add_rows(
+319        self, table: str, values: list[tuple[Any]], columns: tuple[str] |
 None = None
-316    ) -> tuple[int, int]:
-317        """Add multiple rows of values to a table.
-318
-319        Returns a tuple containing the number of successful additions and
-the number of failed additions.
-320
-321        #### :params:
+320    ) -> tuple[int, int]:
+321        """Add multiple rows of values to a table.
 322
-323        `table`: The table to insert values into.
+323        Returns a tuple containing the number of successful additions and
+the number of failed additions.
 324
-325        `values`: A list of tuples of values to be inserted into the table.
-326        Each tuple constitutes a single row to be inserted
-327
-328        `columns`: If `None`, `values` is expected to supply a value for
+325        #### :params:
+326
+327        `table`: The table to insert values into.
+328
+329        `values`: A list of tuples of values to be inserted into the table.
+330        Each tuple constitutes a single row to be inserted
+331
+332        `columns`: If `None`, `values` is expected to supply a value for
 every column in the table.
-329        If `columns` is provided, it should contain the same number of
+333        If `columns` is provided, it should contain the same number of
 elements as `values`."""
-330        successes = 0
-331        failures = 0
-332        for row in values:
-333            if self.add_row(table, row, columns):
-334                successes += 1
-335            else:
-336                failures += 1
-337        return (successes, failures)
+334        successes = 0
+335        failures = 0
+336        for row in values:
+337            if self.add_row(table, row, columns):
+338                successes += 1
+339            else:
+340                failures += 1
+341        return (successes, failures)
 Add multiple rows of values to a table.
 Returns a tuple containing the number of successful additions and the number of
 failed additions.
 *** :params: ***
 table: The table to insert values into.
 values: A list of tuples of values to be inserted into the table. Each tuple
 constitutes a single row to be inserted
@@ -1575,87 +1588,87 @@
 sort_by_column: str | None = None,
 columns_to_return: list[str] | None = None,
 return_as_dataframe: bool = False,
 values_only: bool = False,
 order_by: str | None = None,
 limit: str | int | None = None) -> list[dict] | list[tuple] |
 pandas.core.frame.DataFrame: View Source
-339    @_connect
-340    def get_rows(
-341        self,
-342        table: str,
-343        match_criteria: list[tuple] | dict | None = None,
-344        exact_match: bool = True,
-345        sort_by_column: str | None = None,
-346        columns_to_return: list[str] | None = None,
-347        return_as_dataframe: bool = False,
-348        values_only: bool = False,
-349        order_by: str | None = None,
-350        limit: str | int | None = None,
-351    ) -> list[dict] | list[tuple] | pandas.DataFrame:
-352        """Return matching rows from `table`.
-353
-354        By default, rows will be returned as a list of dictionaries of the
+343    @_connect
+344    def get_rows(
+345        self,
+346        table: str,
+347        match_criteria: list[tuple] | dict | None = None,
+348        exact_match: bool = True,
+349        sort_by_column: str | None = None,
+350        columns_to_return: list[str] | None = None,
+351        return_as_dataframe: bool = False,
+352        values_only: bool = False,
+353        order_by: str | None = None,
+354        limit: str | int | None = None,
+355    ) -> list[dict] | list[tuple] | pandas.DataFrame:
+356        """Return matching rows from `table`.
+357
+358        By default, rows will be returned as a list of dictionaries of the
 form `[{"column_name": value, ...}, ...]`
-355
-356
-357        #### :params:
-358
-359        `match_criteria`: Can be a list of 2-tuples where each
-360        tuple is `(columnName, rowValue)` or a dictionary where
-361        keys are column names and values are row values.
+359
+360
+361        #### :params:
 362
-363        `exact_match`: If `False`, the row value for a given column will be
+363        `match_criteria`: Can be a list of 2-tuples where each
+364        tuple is `(columnName, rowValue)` or a dictionary where
+365        keys are column names and values are row values.
+366
+367        `exact_match`: If `False`, the row value for a given column will be
 matched as a substring.
-364
-365        `sort_by_column`: A column name to sort the results by.
-366        This will sort results in Python after retrieving them from the db.
-367        Use the 'order_by' param to use SQLite engine for ordering.
 368
-369        `columns_to_return`: Optional list of column names.
-370        If provided, the elements returned by this function will only
-contain the provided columns.
-371        Otherwise every column in the row is returned.
+369        `sort_by_column`: A column name to sort the results by.
+370        This will sort results in Python after retrieving them from the db.
+371        Use the 'order_by' param to use SQLite engine for ordering.
 372
-373        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
-object.
-374
-375        `values_only`: Return the results as a list of tuples.
+373        `columns_to_return`: Optional list of column names.
+374        If provided, the elements returned by this function will only
+contain the provided columns.
+375        Otherwise every column in the row is returned.
 376
-377        `order_by`: If given, a `order by {order_by}` clause will be added
-to the select query.
+377        `return_as_dataframe`: Return the results as a `pandas.DataFrame`
+object.
 378
-379        `limit`: If given, a `limit {limit}` clause will be added to the
+379        `values_only`: Return the results as a list of tuples.
+380
+381        `order_by`: If given, a `order by {order_by}` clause will be added
+to the select query.
+382
+383        `limit`: If given, a `limit {limit}` clause will be added to the
 select query.
-380        """
-381
-382        if type(columns_to_return) is str:
-383            columns_to_return = [columns_to_return]
-384        query = f"select * from [{table}]"
-385        matches = []
-386        if match_criteria:
-387            query += f" where {self._get_conditions(match_criteria,
+384        """
+385
+386        if type(columns_to_return) is str:
+387            columns_to_return = [columns_to_return]
+388        query = f"select * from [{table}]"
+389        matches = []
+390        if match_criteria:
+391            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
-388        if order_by:
-389            query += f" order by {order_by}"
-390        if limit:
-391            query += f" limit {limit}"
-392        query += ";"
-393        self.cursor.execute(query)
-394        matches = self.cursor.fetchall()
-395        results = [self._get_dict(table, match, columns_to_return) for match
+392        if order_by:
+393            query += f" order by {order_by}"
+394        if limit:
+395            query += f" limit {limit}"
+396        query += ";"
+397        self.cursor.execute(query)
+398        matches = self.cursor.fetchall()
+399        results = [self._get_dict(table, match, columns_to_return) for match
 in matches]
-396        if sort_by_column:
-397            results = sorted(results, key=lambda x: x[sort_by_column])
-398        if return_as_dataframe:
-399            return pandas.DataFrame(results)
-400        if values_only:
-401            return [tuple(row.values()) for row in results]
-402        else:
-403            return results
+400        if sort_by_column:
+401            results = sorted(results, key=lambda x: x[sort_by_column])
+402        if return_as_dataframe:
+403            return pandas.DataFrame(results)
+404        if values_only:
+405            return [tuple(row.values()) for row in results]
+406        else:
+407            return results
 Return matching rows from table.
 By default, rows will be returned as a list of dictionaries of the form [
 {"column_name": value, ...}, ...]
 *** :params: ***
 match_criteria: Can be a list of 2-tuples where each tuple is (columnName,
 rowValue) or a dictionary where keys are column names and values are row
 values.
@@ -1674,94 +1687,94 @@
 limit: If given, a limit {limit} clause will be added to the select query.
 ⁰
 def find(
 self,
 table: str,
 query_string: str,
 columns: list[str] | None = None) -> list[dict]: View Source
-405    @_connect
-406    def find(
-407        self, table: str, query_string: str, columns: list[str] | None =
+409    @_connect
+410    def find(
+411        self, table: str, query_string: str, columns: list[str] | None =
 None
-408    ) -> list[dict]:
-409        """Search for rows that contain `query_string` as a substring of any
+412    ) -> list[dict]:
+413        """Search for rows that contain `query_string` as a substring of any
 column.
-410
-411        #### :params:
-412
-413        `table`: The table to search.
 414
-415        `query_string`: The substring to search for in all columns.
+415        #### :params:
 416
-417        `columns`: A list of columns to search for query_string.
-418        If None, all columns in the table will be searched.
-419        """
-420        if type(columns) is str:
-421            columns = [columns]
-422        results = []
-423        if not columns:
-424            columns = self.get_column_names(table)
-425        for column in columns:
-426            results.extend(
-427                [
-428                    row
-429                    for row in self.get_rows(
-430                        table, [(column, query_string)], exact_match=False
-431                    )
-432                    if row not in results
-433                ]
-434            )
-435        return results
+417        `table`: The table to search.
+418
+419        `query_string`: The substring to search for in all columns.
+420
+421        `columns`: A list of columns to search for query_string.
+422        If None, all columns in the table will be searched.
+423        """
+424        if type(columns) is str:
+425            columns = [columns]
+426        results = []
+427        if not columns:
+428            columns = self.get_column_names(table)
+429        for column in columns:
+430            results.extend(
+431                [
+432                    row
+433                    for row in self.get_rows(
+434                        table, [(column, query_string)], exact_match=False
+435                    )
+436                    if row not in results
+437                ]
+438            )
+439        return results
 Search for rows that contain query_string as a substring of any column.
 *** :params: ***
 table: The table to search.
 query_string: The substring to search for in all columns.
 columns: A list of columns to search for query_string. If None, all columns in
 the table will be searched.
 ⁰
 def delete(
 self,
 table: str,
 match_criteria: list[tuple] | dict,
 exact_match: bool = True) -> int: View Source
-437    @_connect
-438    def delete(
-439        self, table: str, match_criteria: list[tuple] | dict, exact_match:
+441    @_connect
+442    def delete(
+443        self, table: str, match_criteria: list[tuple] | dict, exact_match:
 bool = True
-440    ) -> int:
-441        """Delete records from `table`.
-442
-443        Returns the number of deleted records.
-444
-445        #### :params:
+444    ) -> int:
+445        """Delete records from `table`.
 446
-447        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+447        Returns the number of deleted records.
+448
+449        #### :params:
+450
+451        `match_criteria`: Can be a list of 2-tuples where each tuple is `
 (column_name, value)`
-448        or a dictionary where keys are column names and values are
+452        or a dictionary where keys are column names and values are
 corresponding values.
-449
-450        `exact_match`: If `False`, the value for a given column will be
+453
+454        `exact_match`: If `False`, the value for a given column will be
 matched as a substring.
-451        """
-452        conditions = self._get_conditions(match_criteria, exact_match)
-453        try:
-454            self.cursor.execute(f"delete from [{table}] where
+455        """
+456        conditions = self._get_conditions(match_criteria, exact_match)
+457        try:
+458            self.cursor.execute(f"delete from [{table}] where
 {conditions};")
-455            num_deletions = self.cursor.rowcount
-456            self.logger.info(
-457                f'Deleted {num_deletions} rows from "{table}" where
+459            num_deletions = self.cursor.rowcount
+460            self.logger.info(
+461                f'Deleted {num_deletions} rows from "{table}" where
 {conditions}".'
-458            )
-459            return num_deletions
-460        except Exception as e:
-461            self.logger.debug(
-462                f'Error deleting rows from "{table}" where {conditions}.\n
+462            )
+463            return num_deletions
+464        except Exception as e:
+465            self.logger.debug(
+466                f'Error deleting rows from "{table}" where {conditions}.\n
 {e}'
-463            )
-464            return 0
+467            )
+468            return 0
 Delete records from table.
 Returns the number of deleted records.
 *** :params: ***
 match_criteria: Can be a list of 2-tuples where each tuple is (column_name,
 value) or a dictionary where keys are column names and values are corresponding
 values.
 exact_match: If False, the value for a given column will be matched as a
@@ -1770,209 +1783,209 @@
 def update(
 self,
 table: str,
 column_to_update: str,
 new_value: Any,
 match_criteria: list[tuple] | dict | None = None,
 exact_match: bool = True) -> int: View Source
-466    @_connect
-467    def update(
-468        self,
-469        table: str,
-470        column_to_update: str,
-471        new_value: Any,
-472        match_criteria: list[tuple] | dict | None = None,
-473        exact_match: bool = True,
-474    ) -> int:
-475        """Update the value in `column_to_update` to `new_value` for rows
+470    @_connect
+471    def update(
+472        self,
+473        table: str,
+474        column_to_update: str,
+475        new_value: Any,
+476        match_criteria: list[tuple] | dict | None = None,
+477        exact_match: bool = True,
+478    ) -> int:
+479        """Update the value in `column_to_update` to `new_value` for rows
 matched with `match_criteria`.
-476
-477        #### :params:
-478
-479        `table`: The table to update rows in.
 480
-481        `column_to_update`: The column to be updated in the matched rows.
+481        #### :params:
 482
-483        `new_value`: The new value to insert.
+483        `table`: The table to update rows in.
 484
-485        `match_criteria`: Can be a list of 2-tuples where each tuple is `
+485        `column_to_update`: The column to be updated in the matched rows.
+486
+487        `new_value`: The new value to insert.
+488
+489        `match_criteria`: Can be a list of 2-tuples where each tuple is `
 (columnName, rowValue)`
-486        or a dictionary where keys are column names and values are
+490        or a dictionary where keys are column names and values are
 corresponding values.
-487        If `None`, every row in `table` will be updated.
-488
-489        `exact_match`: If `False`, `match_criteria` values will be treated
+491        If `None`, every row in `table` will be updated.
+492
+493        `exact_match`: If `False`, `match_criteria` values will be treated
 as substrings.
-490
-491        Returns the number of updated rows."""
-492        query = f"update [{table}] set {column_to_update} = ?"
-493        conditions = ""
-494        if match_criteria:
-495            conditions = self._get_conditions(match_criteria, exact_match)
-496            query += f" where {conditions}"
-497        else:
-498            conditions = None
-499        query += ";"
-500        try:
-501            self.cursor.execute(
-502                query,
-503                (new_value,),
-504            )
-505            num_updates = self.cursor.rowcount
-506            self.logger.info(
-507                f'In {num_updates} rows, updated "{column_to_update}" in "
-{table}" table to "{new_value}" where {conditions}'
+494
+495        Returns the number of updated rows."""
+496        query = f"update [{table}] set {column_to_update} = ?"
+497        conditions = ""
+498        if match_criteria:
+499            conditions = self._get_conditions(match_criteria, exact_match)
+500            query += f" where {conditions}"
+501        else:
+502            conditions = None
+503        query += ";"
+504        try:
+505            self.cursor.execute(
+506                query,
+507                (new_value,),
 508            )
-509            return num_updates
-510        except Exception as e:
-511            self.logger.error(
-512                f'Failed to update "{column_to_update}" in "{table}" table
+509            num_updates = self.cursor.rowcount
+510            self.logger.info(
+511                f'In {num_updates} rows, updated "{column_to_update}" in "
+{table}" table to "{new_value}" where {conditions}'
+512            )
+513            return num_updates
+514        except Exception as e:
+515            self.logger.error(
+516                f'Failed to update "{column_to_update}" in "{table}" table
 to "{new_value}" where {conditions}"\n{e}'
-513            )
-514            return 0
+517            )
+518            return 0
 Update the value in column_to_update to new_value for rows matched with
 match_criteria.
 *** :params: ***
 table: The table to update rows in.
 column_to_update: The column to be updated in the matched rows.
 new_value: The new value to insert.
 match_criteria: Can be a list of 2-tuples where each tuple is (columnName,
 rowValue) or a dictionary where keys are column names and values are
 corresponding values. If None, every row in table will be updated.
 exact_match: If False, match_criteria values will be treated as substrings.
 Returns the number of updated rows.
 ⁰
 def drop_table(self, table: str) -> bool: View Source
-516    @_connect
-517    def drop_table(self, table: str) -> bool:
-518        """Drop `table` from the database.
-519
-520        Returns `True` if successful, `False` if not."""
-521        try:
-522            self.cursor.execute(f"drop Table [{table}];")
-523            self.logger.info(f'Dropped table "{table}"')
-524            return True
-525        except Exception as e:
-526            print(e)
-527            self.logger.error(f'Failed to drop table "{table}"')
-528            return False
+520    @_connect
+521    def drop_table(self, table: str) -> bool:
+522        """Drop `table` from the database.
+523
+524        Returns `True` if successful, `False` if not."""
+525        try:
+526            self.cursor.execute(f"drop Table [{table}];")
+527            self.logger.info(f'Dropped table "{table}"')
+528            return True
+529        except Exception as e:
+530            print(e)
+531            self.logger.error(f'Failed to drop table "{table}"')
+532            return False
 Drop table from the database.
 Returns True if successful, False if not.
 ⁰
 def add_column(
 self,
 table: str,
 column: str,
 _type: str,
 default_value: str | None = None): View Source
-530    @_connect
-531    def add_column(
-532        self, table: str, column: str, _type: str, default_value: str | None
+534    @_connect
+535    def add_column(
+536        self, table: str, column: str, _type: str, default_value: str | None
 = None
-533    ):
-534        """Add a new column to `table`.
-535
-536        #### :params:
-537
-538        `column`: Name of the column to add.
+537    ):
+538        """Add a new column to `table`.
 539
-540        `_type`: The data type of the new column.
+540        #### :params:
 541
-542        `default_value`: Optional default value for the column."""
-543        try:
-544            if default_value:
-545                self.cursor.execute(
-546                    f"alter table [{table}] add column {column} {_type}
+542        `column`: Name of the column to add.
+543
+544        `_type`: The data type of the new column.
+545
+546        `default_value`: Optional default value for the column."""
+547        try:
+548            if default_value:
+549                self.cursor.execute(
+550                    f"alter table [{table}] add column {column} {_type}
 default {default_value};"
-547                )
-548                self.update(table, column, default_value)
-549            else:
-550                self.cursor.execute(
-551                    f"alter table [{table}] add column {column} {_type};"
-552                )
-553            self.logger.info(f'Added column "{column}" to "{table}" table.')
-554        except Exception as e:
-555            self.logger.error(f'Failed to add column "{column}" to "{table}"
+551                )
+552                self.update(table, column, default_value)
+553            else:
+554                self.cursor.execute(
+555                    f"alter table [{table}] add column {column} {_type};"
+556                )
+557            self.logger.info(f'Added column "{column}" to "{table}" table.')
+558        except Exception as e:
+559            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
 Add a new column to table.
 *** :params: ***
 column: Name of the column to add.
 _type: The data type of the new column.
 default_value: Optional default value for the column.
 ⁰
 @staticmethod
 def data_to_string(
 data: list[dict],
 sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-557    @staticmethod
-558    def data_to_string(
-559        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+561    @staticmethod
+562    def data_to_string(
+563        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-560    ) -> str:
-561        """Uses tabulate to produce pretty string output from a list of
+564    ) -> str:
+565        """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-562
-563        #### :params:
-564
-565        `data`: The list of dictionaries to create a grid from.
-566        Assumes all dictionaries in list have the same set of keys.
-567
-568        `sort_key`: Optional dictionary key to sort data with.
-569
-570        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+566
+567        #### :params:
+568
+569        `data`: The list of dictionaries to create a grid from.
+570        Assumes all dictionaries in list have the same set of keys.
+571
+572        `sort_key`: Optional dictionary key to sort data with.
+573
+574        `wrap_to_terminal`: If `True`, the table width will be wrapped to
 fit within the current terminal window.
-571        Pass as `False` if the output is going into something like a `.txt`
+575        Pass as `False` if the output is going into something like a `.txt`
 file."""
-572        return data_to_string(data, sort_key, wrap_to_terminal)
+576        return data_to_string(data, sort_key, wrap_to_terminal)
 Uses tabulate to produce pretty string output from a list of dictionaries.
 *** :params: ***
 data: The list of dictionaries to create a grid from. Assumes all dictionaries
 in list have the same set of keys.
 sort_key: Optional dictionary key to sort data with.
 wrap_to_terminal: If True, the table width will be wrapped to fit within the
 current terminal window. Pass as False if the output is going into something
 like a .txt file.
   ⁰
 def data_to_string(
 data: list[dict],
 sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-575def data_to_string(
-576    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
+579def data_to_string(
+580    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
 True
-577) -> str:
-578    """Uses tabulate to produce pretty string output from a list of
+581) -> str:
+582    """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-579
-580    #### :params:
-581
-582    `data`: The list of dictionaries to create a grid from.
-583    Assumes all dictionaries in list have the same set of keys.
-584
-585    `sort_key`: Optional dictionary key to sort data with.
-586
-587    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
+583
+584    #### :params:
+585
+586    `data`: The list of dictionaries to create a grid from.
+587    Assumes all dictionaries in list have the same set of keys.
+588
+589    `sort_key`: Optional dictionary key to sort data with.
+590
+591    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
 within the current terminal window.
-588    Pass as `False` if the output is going into something like a `.txt`
+592    Pass as `False` if the output is going into something like a `.txt`
 file."""
-589    if len(data) == 0:
-590        return ""
-591    if sort_key:
-592        data = sorted(data, key=lambda d: d[sort_key])
-593    for i, d in enumerate(data):
-594        for k in d:
-595            data[i][k] = str(data[i][k])
-596
-597    try:
-598        print("Resizing grid to fit within the terminal...\n")
-599        return griddy(data, "keys", wrap_to_terminal)
-600    except RuntimeError as e:
-601        print(e)
-602        return str(data)
+593    if len(data) == 0:
+594        return ""
+595    if sort_key:
+596        data = sorted(data, key=lambda d: d[sort_key])
+597    for i, d in enumerate(data):
+598        for k in d:
+599            data[i][k] = str(data[i][k])
+600
+601    try:
+602        print("Resizing grid to fit within the terminal...\n")
+603        return griddy(data, "keys", wrap_to_terminal)
+604    except RuntimeError as e:
+605        print(e)
+606        return str(data)
 Uses tabulate to produce pretty string output from a list of dictionaries.
 *** :params: ***
 data: The list of dictionaries to create a grid from. Assumes all dictionaries
 in list have the same set of keys.
 sort_key: Optional dictionary key to sort data with.
 wrap_to_terminal: If True, the table width will be wrapped to fit within the
 current terminal window. Pass as False if the output is going into something
```

### Comparing `databased-2.4.1/docs/databased/dbparsers.html` & `databased-2.5.0/docs/databased/dbparsers.html`

 * *Files identical despite different names*

### Comparing `databased-2.4.1/docs/databased/dbshell.html` & `databased-2.5.0/docs/databased/dbshell.html`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
                         <label class="view-source-button" for="mod-dbshell-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argshell</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">from</span> <span class="nn">griddle</span> <span class="kn">import</span> <span class="n">griddy</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">dbparsers</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">databased</span> <span class="kn">import</span> <span class="n">DataBased</span><span class="p">,</span> <span class="n">create_shell</span><span class="p">,</span> <span class="n">dbparsers</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="k">class</span> <span class="nc">DBShell</span><span class="p">(</span><span class="n">argshell</span><span class="o">.</span><span class="n">ArgShell</span><span class="p">):</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>    <span class="n">intro</span> <span class="o">=</span> <span class="s2">&quot;Starting dbshell (enter help or ? for arg info)...&quot;</span>
 </span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="n">prompt</span> <span class="o">=</span> <span class="s2">&quot;based&gt;&quot;</span>
 </span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>    <span class="n">dbpath</span><span class="p">:</span> <span class="n">Pathier</span> <span class="o">=</span> <span class="kc">None</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
@@ -154,15 +154,15 @@
 </span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
 </span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
 </span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
 </span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
 </span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
 </span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
 </span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
 </span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
 </span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
 </span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
@@ -347,94 +347,88 @@
 </span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
 </span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
 </span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
 </span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
 </span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
 </span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="p">)</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>                    <span class="k">continue</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                <span class="p">)</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>
-</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="n">create_shell</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>            <span class="n">freedspace</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">freedspace</span><span class="p">)</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>                    <span class="k">continue</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>                <span class="p">)</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DBShell">
                             <input id="DBShell-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -473,15 +467,15 @@
 </span><span id="DBShell-33"><a href="#DBShell-33"><span class="linenos"> 33</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating a back up for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
 </span><span id="DBShell-34"><a href="#DBShell-34"><span class="linenos"> 34</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">timestamp</span><span class="p">)</span>
 </span><span id="DBShell-35"><a href="#DBShell-35"><span class="linenos"> 35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Creating backup is complete.&quot;</span><span class="p">)</span>
 </span><span id="DBShell-36"><a href="#DBShell-36"><span class="linenos"> 36</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Backup path: </span><span class="si">{</span><span class="n">backup_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="DBShell-37"><a href="#DBShell-37"><span class="linenos"> 37</span></a>
 </span><span id="DBShell-38"><a href="#DBShell-38"><span class="linenos"> 38</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="DBShell-39"><a href="#DBShell-39"><span class="linenos"> 39</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
-</span><span id="DBShell-40"><a href="#DBShell-40"><span class="linenos"> 40</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-40"><a href="#DBShell-40"><span class="linenos"> 40</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span><span id="DBShell-41"><a href="#DBShell-41"><span class="linenos"> 41</span></a>
 </span><span id="DBShell-42"><a href="#DBShell-42"><span class="linenos"> 42</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_create_table_parser</span><span class="p">)</span>
 </span><span id="DBShell-43"><a href="#DBShell-43"><span class="linenos"> 43</span></a>    <span class="k">def</span> <span class="nf">do_add_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
 </span><span id="DBShell-44"><a href="#DBShell-44"><span class="linenos"> 44</span></a>        <span class="sd">&quot;&quot;&quot;Add a new table to the database.&quot;&quot;&quot;</span>
 </span><span id="DBShell-45"><a href="#DBShell-45"><span class="linenos"> 45</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
 </span><span id="DBShell-46"><a href="#DBShell-46"><span class="linenos"> 46</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">create_table</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">table_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">)</span>
 </span><span id="DBShell-47"><a href="#DBShell-47"><span class="linenos"> 47</span></a>
@@ -666,90 +660,84 @@
 </span><span id="DBShell-226"><a href="#DBShell-226"><span class="linenos">226</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
 </span><span id="DBShell-227"><a href="#DBShell-227"><span class="linenos">227</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
 </span><span id="DBShell-228"><a href="#DBShell-228"><span class="linenos">228</span></a>
 </span><span id="DBShell-229"><a href="#DBShell-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="DBShell-230"><a href="#DBShell-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
 </span><span id="DBShell-231"><a href="#DBShell-231"><span class="linenos">231</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
 </span><span id="DBShell-232"><a href="#DBShell-232"><span class="linenos">232</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="DBShell-233"><a href="#DBShell-233"><span class="linenos">233</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="DBShell-234"><a href="#DBShell-234"><span class="linenos">234</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-235"><a href="#DBShell-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-236"><a href="#DBShell-236"><span class="linenos">236</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-237"><a href="#DBShell-237"><span class="linenos">237</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell-238"><a href="#DBShell-238"><span class="linenos">238</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell-239"><a href="#DBShell-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DBShell-240"><a href="#DBShell-240"><span class="linenos">240</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="DBShell-241"><a href="#DBShell-241"><span class="linenos">241</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="DBShell-242"><a href="#DBShell-242"><span class="linenos">242</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>
-</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>
-</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>            <span class="p">)</span>
-</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>                    <span class="k">continue</span>
-</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>
-</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                <span class="p">)</span>
-</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-301"><a href="#DBShell-301"><span class="linenos">301</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-302"><a href="#DBShell-302"><span class="linenos">302</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-303"><a href="#DBShell-303"><span class="linenos">303</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-304"><a href="#DBShell-304"><span class="linenos">304</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell-305"><a href="#DBShell-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-306"><a href="#DBShell-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-307"><a href="#DBShell-307"><span class="linenos">307</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell-308"><a href="#DBShell-308"><span class="linenos">308</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-233"><a href="#DBShell-233"><span class="linenos">233</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-234"><a href="#DBShell-234"><span class="linenos">234</span></a>            <span class="n">create_shell</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell-235"><a href="#DBShell-235"><span class="linenos">235</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-236"><a href="#DBShell-236"><span class="linenos">236</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-237"><a href="#DBShell-237"><span class="linenos">237</span></a>
+</span><span id="DBShell-238"><a href="#DBShell-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-239"><a href="#DBShell-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="DBShell-240"><a href="#DBShell-240"><span class="linenos">240</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="DBShell-241"><a href="#DBShell-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-242"><a href="#DBShell-242"><span class="linenos">242</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>            <span class="n">freedspace</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">freedspace</span><span class="p">)</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>
+</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>            <span class="p">)</span>
+</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>                    <span class="k">continue</span>
+</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>
+</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>                <span class="p">)</span>
+</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-301"><a href="#DBShell-301"><span class="linenos">301</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell-302"><a href="#DBShell-302"><span class="linenos">302</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass this to create custom ArgShells.</p>
 </div>
 
 
@@ -841,15 +829,15 @@
 
                 <label class="view-source-button" for="DBShell.do_size-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_size"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_size-38"><a href="#DBShell.do_size-38"><span class="linenos">38</span></a>    <span class="k">def</span> <span class="nf">do_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="DBShell.do_size-39"><a href="#DBShell.do_size-39"><span class="linenos">39</span></a>        <span class="sd">&quot;&quot;&quot;Display the size of the the current db file.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_size-40"><a href="#DBShell.do_size-40"><span class="linenos">40</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_size-40"><a href="#DBShell.do_size-40"><span class="linenos">40</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> is </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Display the size of the the current db file.</p>
 </div>
 
 
@@ -1329,24 +1317,18 @@
 
     </div>
     <a class="headerlink" href="#DBShell.do_customize"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_customize-229"><a href="#DBShell.do_customize-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="DBShell.do_customize-230"><a href="#DBShell.do_customize-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
 </span><span id="DBShell.do_customize-231"><a href="#DBShell.do_customize-231"><span class="linenos">231</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
 </span><span id="DBShell.do_customize-232"><a href="#DBShell.do_customize-232"><span class="linenos">232</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_customize-233"><a href="#DBShell.do_customize-233"><span class="linenos">233</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-234"><a href="#DBShell.do_customize-234"><span class="linenos">234</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.do_customize-235"><a href="#DBShell.do_customize-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-236"><a href="#DBShell.do_customize-236"><span class="linenos">236</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_customize-237"><a href="#DBShell.do_customize-237"><span class="linenos">237</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell.do_customize-238"><a href="#DBShell.do_customize-238"><span class="linenos">238</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell.do_customize-239"><a href="#DBShell.do_customize-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DBShell.do_customize-240"><a href="#DBShell.do_customize-240"><span class="linenos">240</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-241"><a href="#DBShell.do_customize-241"><span class="linenos">241</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-242"><a href="#DBShell.do_customize-242"><span class="linenos">242</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-233"><a href="#DBShell.do_customize-233"><span class="linenos">233</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell.do_customize-234"><a href="#DBShell.do_customize-234"><span class="linenos">234</span></a>            <span class="n">create_shell</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-235"><a href="#DBShell.do_customize-235"><span class="linenos">235</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell.do_customize-236"><a href="#DBShell.do_customize-236"><span class="linenos">236</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate a template file in the current working directory for creating a custom DBShell class.
 Expects one argument: the name of the custom dbshell.
 This will be used to name the generated file as well as several components in the file content.</p>
 </div>
@@ -1360,23 +1342,23 @@
         <span class="def">def</span>
         <span class="name">do_vacuum</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_vacuum-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_vacuum"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_vacuum-245"><a href="#DBShell.do_vacuum-245"><span class="linenos">245</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_vacuum-246"><a href="#DBShell.do_vacuum-246"><span class="linenos">246</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="DBShell.do_vacuum-247"><a href="#DBShell.do_vacuum-247"><span class="linenos">247</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-248"><a href="#DBShell.do_vacuum-248"><span class="linenos">248</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-249"><a href="#DBShell.do_vacuum-249"><span class="linenos">249</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_vacuum-250"><a href="#DBShell.do_vacuum-250"><span class="linenos">250</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="DBShell.do_vacuum-251"><a href="#DBShell.do_vacuum-251"><span class="linenos">251</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-252"><a href="#DBShell.do_vacuum-252"><span class="linenos">252</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_vacuum-238"><a href="#DBShell.do_vacuum-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_vacuum-239"><a href="#DBShell.do_vacuum-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_vacuum-240"><a href="#DBShell.do_vacuum-240"><span class="linenos">240</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span>
+</span><span id="DBShell.do_vacuum-241"><a href="#DBShell.do_vacuum-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-242"><a href="#DBShell.do_vacuum-242"><span class="linenos">242</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-243"><a href="#DBShell.do_vacuum-243"><span class="linenos">243</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>            <span class="n">freedspace</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell.do_vacuum-245"><a href="#DBShell.do_vacuum-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">formatted_size</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-246"><a href="#DBShell.do_vacuum-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">freedspace</span><span class="p">)</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Reduce database disk memory.</p>
 </div>
 
 
@@ -1388,51 +1370,51 @@
         <span class="def">def</span>
         <span class="name">preloop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.preloop-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.preloop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                <span class="p">)</span>
-</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-301"><a href="#DBShell.preloop-301"><span class="linenos">301</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-302"><a href="#DBShell.preloop-302"><span class="linenos">302</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-303"><a href="#DBShell.preloop-303"><span class="linenos">303</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-304"><a href="#DBShell.preloop-304"><span class="linenos">304</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-305"><a href="#DBShell.preloop-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.preloop-306"><a href="#DBShell.preloop-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-307"><a href="#DBShell.preloop-307"><span class="linenos">307</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell.preloop-308"><a href="#DBShell.preloop-308"><span class="linenos">308</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-266"><a href="#DBShell.preloop-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell.preloop-267"><a href="#DBShell.preloop-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell.preloop-268"><a href="#DBShell.preloop-268"><span class="linenos">268</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell.preloop-269"><a href="#DBShell.preloop-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell.preloop-270"><a href="#DBShell.preloop-270"><span class="linenos">270</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell.preloop-271"><a href="#DBShell.preloop-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>                <span class="p">)</span>
+</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-301"><a href="#DBShell.preloop-301"><span class="linenos">301</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell.preloop-302"><a href="#DBShell.preloop-302"><span class="linenos">302</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan the current directory for a .db file to use.
 If not found, prompt the user for one or to try again recursively.</p>
 </div>
 
@@ -1476,16 +1458,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-311"><a href="#main-311"><span class="linenos">311</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-312"><a href="#main-312"><span class="linenos">312</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-305"><a href="#main-305"><span class="linenos">305</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-306"><a href="#main-306"><span class="linenos">306</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -29,15 +29,15 @@
 
 ****** databased.dbshell ******
 ⁰ View Source
 __1import argshell
 __2from griddle import griddy
 __3from pathier import Pathier
 __4
-__5from databased import DataBased, dbparsers
+__5from databased import DataBased, create_shell, dbparsers
 __6
 __7
 __8class DBShell(argshell.ArgShell):
 __9    intro = "Starting dbshell (enter help or ? for arg info)..."
 _10    prompt = "based>"
 _11    dbpath: Pathier = None  # type: ignore
 _12
@@ -63,15 +63,15 @@
 _32        print(f"Creating a back up for {self.dbpath}...")
 _33        backup_path = self.dbpath.backup(args.timestamp)
 _34        print("Creating backup is complete.")
 _35        print(f"Backup path: {backup_path}")
 _36
 _37    def do_size(self, arg: str):
 _38        """Display the size of the the current db file."""
-_39        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
+_39        print(f"{self.dbpath.name} is {self.dbpath.formatted_size}.")
 _40
 _41    @argshell.with_parser(dbparsers.get_create_table_parser)
 _42    def do_add_table(self, args: argshell.Namespace):
 _43        """Add a new table to the database."""
 _44        with DataBased(self.dbpath) as db:
 _45            db.create_table(args.table_name, args.columns)
 _46
@@ -284,102 +284,94 @@
 227
 228    def do_customize(self, arg: str):
 229        """Generate a template file in the current working directory for
 creating a custom DBShell class.
 230        Expects one argument: the name of the custom dbshell.
 231        This will be used to name the generated file as well as several
 components in the file content."""
-232        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
-(".py")
-233        if custom_file.exists():
-234            print(f"Error: {custom_file.name} already exists in this
-location.")
-235        else:
-236            variable_name = "_".join(word for word in arg.lower().split())
-237            class_name = "".join(word.capitalize() for word in arg.split())
-238            content = (Pathier(__file__).parent /
-"customshell.py").read_text()
-239            content = content.replace("CustomShell", class_name)
-240            content = content.replace("customshell", variable_name)
-241            custom_file.write_text(content)
-242
-243    def do_vacuum(self, arg: str):
-244        """Reduce database disk memory."""
-245        starting_size = self.dbpath.size()
-246        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-247        print("Vacuuming database...")
-248        with DataBased(self.dbpath) as db:
-249            db.vacuum()
-250        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-251        print(f"Freed up {Pathier.format_size(starting_size -
-self.dbpath.size())} of disk space.")  # type: ignore
-252
-253    def _choose_db(self, options: list[Pathier]) -> Pathier:
-254        """Prompt the user to select from a list of files."""
-255        cwd = Pathier.cwd()
-256        paths = [path.separate(cwd.stem) for path in options]
-257        while True:
-258            print(
-259                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+232        try:
+233            create_shell(arg)
+234        except Exception as e:
+235            print(f"{type(e).__name__}: {e}")
+236
+237    def do_vacuum(self, arg: str):
+238        """Reduce database disk memory."""
+239        starting_size = self.dbpath.size
+240        print(f"Database size before vacuuming:
+{self.dbpath.formatted_size}")
+241        print("Vacuuming database...")
+242        with DataBased(self.dbpath) as db:
+243            freedspace = db.vacuum()
+244        print(f"Database size after vacuuming:
+{self.dbpath.formatted_size}")
+245        print(f"Freed up {Pathier.format_bytes(freedspace)} of disk space.")
+246
+247    def _choose_db(self, options: list[Pathier]) -> Pathier:
+248        """Prompt the user to select from a list of files."""
+249        cwd = Pathier.cwd()
+250        paths = [path.separate(cwd.stem) for path in options]
+251        while True:
+252            print(
+253                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
 enumerate(paths,1)])}"
-260            )
-261            choice = input("Enter the number of the option to use: ")
-262            try:
-263                index = int(choice)
-264                if not 1 <= index <= len(options):
-265                    print("Choice out of range.")
-266                    continue
-267                return options[index - 1]
-268            except Exception as e:
-269                print(f"{choice} is not a valid option.")
-270
-271    def preloop(self):
-272        """Scan the current directory for a .db file to use.
-273        If not found, prompt the user for one or to try again
+254            )
+255            choice = input("Enter the number of the option to use: ")
+256            try:
+257                index = int(choice)
+258                if not 1 <= index <= len(options):
+259                    print("Choice out of range.")
+260                    continue
+261                return options[index - 1]
+262            except Exception as e:
+263                print(f"{choice} is not a valid option.")
+264
+265    def preloop(self):
+266        """Scan the current directory for a .db file to use.
+267        If not found, prompt the user for one or to try again
 recursively."""
-274        if self.dbpath:
-275            self.dbpath = Pathier(self.dbpath)
-276            print(f"Defaulting to database {self.dbpath}")
-277        else:
-278            print("Searching for database...")
-279            cwd = Pathier.cwd()
-280            dbs = list(cwd.glob("*.db"))
-281            if len(dbs) == 1:
-282                self.dbpath = dbs[0]
-283                print(f"Using database {self.dbpath}.")
-284            elif dbs:
-285                self.dbpath = self._choose_db(dbs)
-286            else:
-287                print(f"Could not find a .db file in {cwd}.")
-288                path = input(
-289                    "Enter path to .db file to use or press enter to search
+268        if self.dbpath:
+269            self.dbpath = Pathier(self.dbpath)
+270            print(f"Defaulting to database {self.dbpath}")
+271        else:
+272            print("Searching for database...")
+273            cwd = Pathier.cwd()
+274            dbs = list(cwd.glob("*.db"))
+275            if len(dbs) == 1:
+276                self.dbpath = dbs[0]
+277                print(f"Using database {self.dbpath}.")
+278            elif dbs:
+279                self.dbpath = self._choose_db(dbs)
+280            else:
+281                print(f"Could not find a .db file in {cwd}.")
+282                path = input(
+283                    "Enter path to .db file to use or press enter to search
 again recursively: "
-290                )
-291                if path:
-292                    self.dbpath = Pathier(path)
-293                elif not path:
-294                    print("Searching recursively...")
-295                    dbs = list(cwd.rglob("*.db"))
-296                    if len(dbs) == 1:
-297                        self.dbpath = dbs[0]
-298                        print(f"Using database {self.dbpath}.")
-299                    elif dbs:
-300                        self.dbpath = self._choose_db(dbs)
-301                    else:
-302                        print("Could not find a .db file.")
-303                        self.dbpath = Pathier(input("Enter path to a .db
+284                )
+285                if path:
+286                    self.dbpath = Pathier(path)
+287                elif not path:
+288                    print("Searching recursively...")
+289                    dbs = list(cwd.rglob("*.db"))
+290                    if len(dbs) == 1:
+291                        self.dbpath = dbs[0]
+292                        print(f"Using database {self.dbpath}.")
+293                    elif dbs:
+294                        self.dbpath = self._choose_db(dbs)
+295                    else:
+296                        print("Could not find a .db file.")
+297                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-304        if not self.dbpath.exists():
-305            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-306        if not self.dbpath.is_file():
-307            raise ValueError(f"{self.dbpath} is not a file.")
-308
-309
-310def main():
-311    DBShell().cmdloop()
+298        if not self.dbpath.exists():
+299            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+300        if not self.dbpath.is_file():
+301            raise ValueError(f"{self.dbpath} is not a file.")
+302
+303
+304def main():
+305    DBShell().cmdloop()
   ⁰
 class DBShell(argshell.argshell.ArgShell): View Source
 __9class DBShell(argshell.ArgShell):
 _10    intro = "Starting dbshell (enter help or ? for arg info)..."
 _11    prompt = "based>"
 _12    dbpath: Pathier = None  # type: ignore
 _13
@@ -405,15 +397,15 @@
 _33        print(f"Creating a back up for {self.dbpath}...")
 _34        backup_path = self.dbpath.backup(args.timestamp)
 _35        print("Creating backup is complete.")
 _36        print(f"Backup path: {backup_path}")
 _37
 _38    def do_size(self, arg: str):
 _39        """Display the size of the the current db file."""
-_40        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
+_40        print(f"{self.dbpath.name} is {self.dbpath.formatted_size}.")
 _41
 _42    @argshell.with_parser(dbparsers.get_create_table_parser)
 _43    def do_add_table(self, args: argshell.Namespace):
 _44        """Add a new table to the database."""
 _45        with DataBased(self.dbpath) as db:
 _46            db.create_table(args.table_name, args.columns)
 _47
@@ -626,98 +618,90 @@
 228
 229    def do_customize(self, arg: str):
 230        """Generate a template file in the current working directory for
 creating a custom DBShell class.
 231        Expects one argument: the name of the custom dbshell.
 232        This will be used to name the generated file as well as several
 components in the file content."""
-233        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
-(".py")
-234        if custom_file.exists():
-235            print(f"Error: {custom_file.name} already exists in this
-location.")
-236        else:
-237            variable_name = "_".join(word for word in arg.lower().split())
-238            class_name = "".join(word.capitalize() for word in arg.split())
-239            content = (Pathier(__file__).parent /
-"customshell.py").read_text()
-240            content = content.replace("CustomShell", class_name)
-241            content = content.replace("customshell", variable_name)
-242            custom_file.write_text(content)
-243
-244    def do_vacuum(self, arg: str):
-245        """Reduce database disk memory."""
-246        starting_size = self.dbpath.size()
-247        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-248        print("Vacuuming database...")
-249        with DataBased(self.dbpath) as db:
-250            db.vacuum()
-251        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-252        print(f"Freed up {Pathier.format_size(starting_size -
-self.dbpath.size())} of disk space.")  # type: ignore
-253
-254    def _choose_db(self, options: list[Pathier]) -> Pathier:
-255        """Prompt the user to select from a list of files."""
-256        cwd = Pathier.cwd()
-257        paths = [path.separate(cwd.stem) for path in options]
-258        while True:
-259            print(
-260                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+233        try:
+234            create_shell(arg)
+235        except Exception as e:
+236            print(f"{type(e).__name__}: {e}")
+237
+238    def do_vacuum(self, arg: str):
+239        """Reduce database disk memory."""
+240        starting_size = self.dbpath.size
+241        print(f"Database size before vacuuming:
+{self.dbpath.formatted_size}")
+242        print("Vacuuming database...")
+243        with DataBased(self.dbpath) as db:
+244            freedspace = db.vacuum()
+245        print(f"Database size after vacuuming:
+{self.dbpath.formatted_size}")
+246        print(f"Freed up {Pathier.format_bytes(freedspace)} of disk space.")
+247
+248    def _choose_db(self, options: list[Pathier]) -> Pathier:
+249        """Prompt the user to select from a list of files."""
+250        cwd = Pathier.cwd()
+251        paths = [path.separate(cwd.stem) for path in options]
+252        while True:
+253            print(
+254                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
 enumerate(paths,1)])}"
-261            )
-262            choice = input("Enter the number of the option to use: ")
-263            try:
-264                index = int(choice)
-265                if not 1 <= index <= len(options):
-266                    print("Choice out of range.")
-267                    continue
-268                return options[index - 1]
-269            except Exception as e:
-270                print(f"{choice} is not a valid option.")
-271
-272    def preloop(self):
-273        """Scan the current directory for a .db file to use.
-274        If not found, prompt the user for one or to try again
+255            )
+256            choice = input("Enter the number of the option to use: ")
+257            try:
+258                index = int(choice)
+259                if not 1 <= index <= len(options):
+260                    print("Choice out of range.")
+261                    continue
+262                return options[index - 1]
+263            except Exception as e:
+264                print(f"{choice} is not a valid option.")
+265
+266    def preloop(self):
+267        """Scan the current directory for a .db file to use.
+268        If not found, prompt the user for one or to try again
 recursively."""
-275        if self.dbpath:
-276            self.dbpath = Pathier(self.dbpath)
-277            print(f"Defaulting to database {self.dbpath}")
-278        else:
-279            print("Searching for database...")
-280            cwd = Pathier.cwd()
-281            dbs = list(cwd.glob("*.db"))
-282            if len(dbs) == 1:
-283                self.dbpath = dbs[0]
-284                print(f"Using database {self.dbpath}.")
-285            elif dbs:
-286                self.dbpath = self._choose_db(dbs)
-287            else:
-288                print(f"Could not find a .db file in {cwd}.")
-289                path = input(
-290                    "Enter path to .db file to use or press enter to search
+269        if self.dbpath:
+270            self.dbpath = Pathier(self.dbpath)
+271            print(f"Defaulting to database {self.dbpath}")
+272        else:
+273            print("Searching for database...")
+274            cwd = Pathier.cwd()
+275            dbs = list(cwd.glob("*.db"))
+276            if len(dbs) == 1:
+277                self.dbpath = dbs[0]
+278                print(f"Using database {self.dbpath}.")
+279            elif dbs:
+280                self.dbpath = self._choose_db(dbs)
+281            else:
+282                print(f"Could not find a .db file in {cwd}.")
+283                path = input(
+284                    "Enter path to .db file to use or press enter to search
 again recursively: "
-291                )
-292                if path:
-293                    self.dbpath = Pathier(path)
-294                elif not path:
-295                    print("Searching recursively...")
-296                    dbs = list(cwd.rglob("*.db"))
-297                    if len(dbs) == 1:
-298                        self.dbpath = dbs[0]
-299                        print(f"Using database {self.dbpath}.")
-300                    elif dbs:
-301                        self.dbpath = self._choose_db(dbs)
-302                    else:
-303                        print("Could not find a .db file.")
-304                        self.dbpath = Pathier(input("Enter path to a .db
+285                )
+286                if path:
+287                    self.dbpath = Pathier(path)
+288                elif not path:
+289                    print("Searching recursively...")
+290                    dbs = list(cwd.rglob("*.db"))
+291                    if len(dbs) == 1:
+292                        self.dbpath = dbs[0]
+293                        print(f"Using database {self.dbpath}.")
+294                    elif dbs:
+295                        self.dbpath = self._choose_db(dbs)
+296                    else:
+297                        print("Could not find a .db file.")
+298                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-305        if not self.dbpath.exists():
-306            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-307        if not self.dbpath.is_file():
-308            raise ValueError(f"{self.dbpath} is not a file.")
+299        if not self.dbpath.exists():
+300            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+301        if not self.dbpath.is_file():
+302            raise ValueError(f"{self.dbpath} is not a file.")
 Subclass this to create custom ArgShells.
 ⁰
 def do_use_db(self, arg: str): View Source
 14    def do_use_db(self, arg: str):
 15        """Set which database file to use."""
 16        dbpath = Pathier(arg)
 17        if not dbpath.exists():
@@ -746,15 +730,15 @@
 35        print("Creating backup is complete.")
 36        print(f"Backup path: {backup_path}")
 Create a backup of the current db file.
 ⁰
 def do_size(self, arg: str): View Source
 38    def do_size(self, arg: str):
 39        """Display the size of the the current db file."""
-40        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
+40        print(f"{self.dbpath.name} is {self.dbpath.formatted_size}.")
 Display the size of the the current db file.
 ⁰
 @argshell.with_parser(dbparsers.get_create_table_parser)
 def do_add_table(self, args: argshell.argshell.Namespace): View Source
 42    @argshell.with_parser(dbparsers.get_create_table_parser)
 43    def do_add_table(self, args: argshell.Namespace):
 44        """Add a new table to the database."""
@@ -1034,87 +1018,79 @@
 def do_customize(self, arg: str): View Source
 229    def do_customize(self, arg: str):
 230        """Generate a template file in the current working directory for
 creating a custom DBShell class.
 231        Expects one argument: the name of the custom dbshell.
 232        This will be used to name the generated file as well as several
 components in the file content."""
-233        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
-(".py")
-234        if custom_file.exists():
-235            print(f"Error: {custom_file.name} already exists in this
-location.")
-236        else:
-237            variable_name = "_".join(word for word in arg.lower().split())
-238            class_name = "".join(word.capitalize() for word in arg.split())
-239            content = (Pathier(__file__).parent /
-"customshell.py").read_text()
-240            content = content.replace("CustomShell", class_name)
-241            content = content.replace("customshell", variable_name)
-242            custom_file.write_text(content)
+233        try:
+234            create_shell(arg)
+235        except Exception as e:
+236            print(f"{type(e).__name__}: {e}")
 Generate a template file in the current working directory for creating a custom
 DBShell class. Expects one argument: the name of the custom dbshell. This will
 be used to name the generated file as well as several components in the file
 content.
 ⁰
 def do_vacuum(self, arg: str): View Source
-244    def do_vacuum(self, arg: str):
-245        """Reduce database disk memory."""
-246        starting_size = self.dbpath.size()
-247        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-248        print("Vacuuming database...")
-249        with DataBased(self.dbpath) as db:
-250            db.vacuum()
-251        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-252        print(f"Freed up {Pathier.format_size(starting_size -
-self.dbpath.size())} of disk space.")  # type: ignore
+238    def do_vacuum(self, arg: str):
+239        """Reduce database disk memory."""
+240        starting_size = self.dbpath.size
+241        print(f"Database size before vacuuming:
+{self.dbpath.formatted_size}")
+242        print("Vacuuming database...")
+243        with DataBased(self.dbpath) as db:
+244            freedspace = db.vacuum()
+245        print(f"Database size after vacuuming:
+{self.dbpath.formatted_size}")
+246        print(f"Freed up {Pathier.format_bytes(freedspace)} of disk space.")
 Reduce database disk memory.
 ⁰
 def preloop(self): View Source
-272    def preloop(self):
-273        """Scan the current directory for a .db file to use.
-274        If not found, prompt the user for one or to try again
+266    def preloop(self):
+267        """Scan the current directory for a .db file to use.
+268        If not found, prompt the user for one or to try again
 recursively."""
-275        if self.dbpath:
-276            self.dbpath = Pathier(self.dbpath)
-277            print(f"Defaulting to database {self.dbpath}")
-278        else:
-279            print("Searching for database...")
-280            cwd = Pathier.cwd()
-281            dbs = list(cwd.glob("*.db"))
-282            if len(dbs) == 1:
-283                self.dbpath = dbs[0]
-284                print(f"Using database {self.dbpath}.")
-285            elif dbs:
-286                self.dbpath = self._choose_db(dbs)
-287            else:
-288                print(f"Could not find a .db file in {cwd}.")
-289                path = input(
-290                    "Enter path to .db file to use or press enter to search
+269        if self.dbpath:
+270            self.dbpath = Pathier(self.dbpath)
+271            print(f"Defaulting to database {self.dbpath}")
+272        else:
+273            print("Searching for database...")
+274            cwd = Pathier.cwd()
+275            dbs = list(cwd.glob("*.db"))
+276            if len(dbs) == 1:
+277                self.dbpath = dbs[0]
+278                print(f"Using database {self.dbpath}.")
+279            elif dbs:
+280                self.dbpath = self._choose_db(dbs)
+281            else:
+282                print(f"Could not find a .db file in {cwd}.")
+283                path = input(
+284                    "Enter path to .db file to use or press enter to search
 again recursively: "
-291                )
-292                if path:
-293                    self.dbpath = Pathier(path)
-294                elif not path:
-295                    print("Searching recursively...")
-296                    dbs = list(cwd.rglob("*.db"))
-297                    if len(dbs) == 1:
-298                        self.dbpath = dbs[0]
-299                        print(f"Using database {self.dbpath}.")
-300                    elif dbs:
-301                        self.dbpath = self._choose_db(dbs)
-302                    else:
-303                        print("Could not find a .db file.")
-304                        self.dbpath = Pathier(input("Enter path to a .db
+285                )
+286                if path:
+287                    self.dbpath = Pathier(path)
+288                elif not path:
+289                    print("Searching recursively...")
+290                    dbs = list(cwd.rglob("*.db"))
+291                    if len(dbs) == 1:
+292                        self.dbpath = dbs[0]
+293                        print(f"Using database {self.dbpath}.")
+294                    elif dbs:
+295                        self.dbpath = self._choose_db(dbs)
+296                    else:
+297                        print("Could not find a .db file.")
+298                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-305        if not self.dbpath.exists():
-306            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-307        if not self.dbpath.is_file():
-308            raise ValueError(f"{self.dbpath} is not a file.")
+299        if not self.dbpath.exists():
+300            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+301        if not self.dbpath.is_file():
+302            raise ValueError(f"{self.dbpath} is not a file.")
 Scan the current directory for a .db file to use. If not found, prompt the user
 for one or to try again recursively.
 ** Inherited Members **
   ⁰
 def main(): View Source
-311def main():
-312    DBShell().cmdloop()
+305def main():
+306    DBShell().cmdloop()
```

### Comparing `databased-2.4.1/src/databased/customshell.py` & `databased-2.5.0/src/databased/customshell.py`

 * *Files identical despite different names*

### Comparing `databased-2.4.1/src/databased/databased.py` & `databased-2.5.0/src/databased/databased.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,17 +182,21 @@
         else:
             conditions = " and ".join(
                 f'"{column_row[0]}" like "%{column_row[1]}%"'
                 for column_row in match_criteria
             )
         return f"({conditions})"
 
-    def vacuum(self):
-        """Reduce disk size of the database with a `VACUUM` query."""
+    def vacuum(self) -> int:
+        """Reduce disk size of the database with a `VACUUM` query.
+
+        Returns space freed up in bytes."""
+        size = self.dbpath.size
         self.query("VACUUM;")
+        return size - self.dbpath.size
 
     @_connect
     def query(self, query_) -> list[Any]:
         """Execute an arbitrary query and return the results."""
         self.cursor.execute(query_)
         return self.cursor.fetchall()
```

### Comparing `databased-2.4.1/src/databased/dbparsers.py` & `databased-2.5.0/src/databased/dbparsers.py`

 * *Files identical despite different names*

### Comparing `databased-2.4.1/src/databased/dbshell.py` & `databased-2.5.0/src/databased/dbshell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argshell
 from griddle import griddy
 from pathier import Pathier
 
-from databased import DataBased, dbparsers
+from databased import DataBased, create_shell, dbparsers
 
 
 class DBShell(argshell.ArgShell):
     intro = "Starting dbshell (enter help or ? for arg info)..."
     prompt = "based>"
     dbpath: Pathier = None  # type: ignore
 
@@ -32,15 +32,15 @@
         print(f"Creating a back up for {self.dbpath}...")
         backup_path = self.dbpath.backup(args.timestamp)
         print("Creating backup is complete.")
         print(f"Backup path: {backup_path}")
 
     def do_size(self, arg: str):
         """Display the size of the the current db file."""
-        print(f"{self.dbpath.name} is {self.dbpath.size(True)}.")
+        print(f"{self.dbpath.name} is {self.dbpath.formatted_size}.")
 
     @argshell.with_parser(dbparsers.get_create_table_parser)
     def do_add_table(self, args: argshell.Namespace):
         """Add a new table to the database."""
         with DataBased(self.dbpath) as db:
             db.create_table(args.table_name, args.columns)
 
@@ -225,34 +225,28 @@
         for db in dbs:
             print(db.separate(cwd.stem))
 
     def do_customize(self, arg: str):
         """Generate a template file in the current working directory for creating a custom DBShell class.
         Expects one argument: the name of the custom dbshell.
         This will be used to name the generated file as well as several components in the file content."""
-        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix(".py")
-        if custom_file.exists():
-            print(f"Error: {custom_file.name} already exists in this location.")
-        else:
-            variable_name = "_".join(word for word in arg.lower().split())
-            class_name = "".join(word.capitalize() for word in arg.split())
-            content = (Pathier(__file__).parent / "customshell.py").read_text()
-            content = content.replace("CustomShell", class_name)
-            content = content.replace("customshell", variable_name)
-            custom_file.write_text(content)
+        try:
+            create_shell(arg)
+        except Exception as e:
+            print(f"{type(e).__name__}: {e}")
 
     def do_vacuum(self, arg: str):
         """Reduce database disk memory."""
-        starting_size = self.dbpath.size()
-        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
+        starting_size = self.dbpath.size
+        print(f"Database size before vacuuming: {self.dbpath.formatted_size}")
         print("Vacuuming database...")
         with DataBased(self.dbpath) as db:
-            db.vacuum()
-        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-        print(f"Freed up {Pathier.format_size(starting_size - self.dbpath.size())} of disk space.")  # type: ignore
+            freedspace = db.vacuum()
+        print(f"Database size after vacuuming: {self.dbpath.formatted_size}")
+        print(f"Freed up {Pathier.format_bytes(freedspace)} of disk space.")
 
     def _choose_db(self, options: list[Pathier]) -> Pathier:
         """Prompt the user to select from a list of files."""
         cwd = Pathier.cwd()
         paths = [path.separate(cwd.stem) for path in options]
         while True:
             print(
```

### Comparing `databased-2.4.1/LICENSE.txt` & `databased-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-2.4.1/README.md` & `databased-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `databased-2.4.1/pyproject.toml` & `databased-2.5.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "databased"
-authors = [{name="Matt Manes"}]
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "2.4.1"
+version = "2.5.0"
 requires-python = ">=3.10"
 dependencies = ["pandas", "tabulate", "pytest", "argshell", "pathier", "griddle"]
 readme = "README.md"
-keywords = [
-    "database",
-    "sqlite",
-    "sqlite3"
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
+keywords = ["database", "sqlite", "sqlite3"]
+classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
+
+[[project.authors]]
+name = "Matt Manes"
 
 [project.urls]
-"Homepage" = "https://github.com/matt-manes/databased"
-"Documentation" = "https://github.com/matt-manes/databased/tree/main/docs"
+Homepage = "https://github.com/matt-manes/databased"
+Documentation = "https://github.com/matt-manes/databased/tree/main/docs"
 "Source code" = "https://github.com/matt-manes/databased/tree/main/src/databased"
 
+[project.scripts]
+dbshell = "databased.dbshell:main"
+createshell = "databased.create_shell:main"
+
+[tool]
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
+addopts = ["--import-mode=importlib"]
 pythonpath = "src"
 
 [tool.hatch.build.targets.sdist]
-exclude = [
-    ".coverage",
-    ".pytest_cache",
-    ".vscode",
-    "tests"
-]
-[project.scripts]
-dbshell = "databased.dbshell:main"
+exclude = [".coverage", ".pytest_cache", ".vscode", "tests"]
```

### Comparing `databased-2.4.1/PKG-INFO` & `databased-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databased
-Version: 2.4.1
+Version: 2.5.0
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
```

