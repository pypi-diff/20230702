# Comparing `tmp/pathier-1.0.0.tar.gz` & `tmp/pathier-1.1.0.tar.gz`

## Comparing `pathier-1.0.0.tar` & `pathier-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 pathier-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-1.0.0/docs/index.html
--rw-r--r--   0        0        0   299385 2020-02-02 00:00:00.000000 pathier-1.0.0/docs/pathier.html
--rw-r--r--   0        0        0    61206 2020-02-02 00:00:00.000000 pathier-1.0.0/docs/search.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.0.0/src/pathier/__init__.py
--rw-r--r--   0        0        0    18994 2020-02-02 00:00:00.000000 pathier-1.0.0/src/pathier/pathier.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 pathier-1.0.0/README.md
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pathier-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 pathier-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 pathier-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-1.1.0/docs/index.html
+-rw-r--r--   0        0        0   301139 2020-02-02 00:00:00.000000 pathier-1.1.0/docs/pathier.html
+-rw-r--r--   0        0        0    61463 2020-02-02 00:00:00.000000 pathier-1.1.0/docs/search.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.1.0/src/pathier/__init__.py
+-rw-r--r--   0        0        0    19182 2020-02-02 00:00:00.000000 pathier-1.1.0/src/pathier/pathier.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pathier-1.1.0/README.md
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pathier-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 pathier-1.1.0/PKG-INFO
```

### Comparing `pathier-1.0.0/CHANGELOG.md` & `pathier-1.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## v1.0.0 (2023-07-02)
+
+#### Performance improvements
+
+* BREAKING: replace() accepts a list of 2-tuples instead of only an old and new string
+#### Refactorings
+
+* BREAKING: change `format_size()` to `format_bytes()`
+* BREAKING: change `size` to a property
+#### Docs
+
+* update readme
+
 ## v0.14.1 (2023-06-21)
 
 #### Performance improvements
 
 * toml files will have their datatypes converted to python types when loaded
 #### Others
```

### Comparing `pathier-1.0.0/docs/pathier.html` & `pathier-1.1.0/docs/pathier.html`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,17 @@
                         <li>
                                 <a class="variable" href="#Pathier.modified_since_last_read">modified_since_last_read</a>
                         </li>
                         <li>
                                 <a class="variable" href="#Pathier.size">size</a>
                         </li>
                         <li>
+                                <a class="variable" href="#Pathier.formatted_size">formatted_size</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#Pathier.format_bytes">format_bytes</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.is_larger">is_larger</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.is_older">is_older</a>
@@ -273,409 +276,414 @@
 </span><span id="Pathier-95"><a href="#Pathier-95"><span class="linenos"> 95</span></a>            <span class="k">return</span> <span class="mi">0</span>
 </span><span id="Pathier-96"><a href="#Pathier-96"><span class="linenos"> 96</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
 </span><span id="Pathier-97"><a href="#Pathier-97"><span class="linenos"> 97</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
 </span><span id="Pathier-98"><a href="#Pathier-98"><span class="linenos"> 98</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
 </span><span id="Pathier-99"><a href="#Pathier-99"><span class="linenos"> 99</span></a>            <span class="k">return</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
 </span><span id="Pathier-100"><a href="#Pathier-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="mi">0</span>
 </span><span id="Pathier-101"><a href="#Pathier-101"><span class="linenos">101</span></a>
-</span><span id="Pathier-102"><a href="#Pathier-102"><span class="linenos">102</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Pathier-103"><a href="#Pathier-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">format_bytes</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Pathier-104"><a href="#Pathier-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;Format `size` with common file size abbreviations and rounded to two decimal places.</span>
-</span><span id="Pathier-105"><a href="#Pathier-105"><span class="linenos">105</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-106"><a href="#Pathier-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
-</span><span id="Pathier-107"><a href="#Pathier-107"><span class="linenos">107</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
-</span><span id="Pathier-108"><a href="#Pathier-108"><span class="linenos">108</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
-</span><span id="Pathier-109"><a href="#Pathier-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
-</span><span id="Pathier-110"><a href="#Pathier-110"><span class="linenos">110</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Pathier-111"><a href="#Pathier-111"><span class="linenos">111</span></a>
-</span><span id="Pathier-112"><a href="#Pathier-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-113"><a href="#Pathier-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than the one pointed to by `path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier-114"><a href="#Pathier-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
-</span><span id="Pathier-115"><a href="#Pathier-115"><span class="linenos">115</span></a>
-</span><span id="Pathier-116"><a href="#Pathier-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-117"><a href="#Pathier-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than the one pointed to by `path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier-118"><a href="#Pathier-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
-</span><span id="Pathier-119"><a href="#Pathier-119"><span class="linenos">119</span></a>
-</span><span id="Pathier-120"><a href="#Pathier-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-121"><a href="#Pathier-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified more recently than the one pointed to by `path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier-122"><a href="#Pathier-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
-</span><span id="Pathier-123"><a href="#Pathier-123"><span class="linenos">123</span></a>
-</span><span id="Pathier-124"><a href="#Pathier-124"><span class="linenos">124</span></a>    <span class="c1"># ===============================================navigation===============================================</span>
-</span><span id="Pathier-125"><a href="#Pathier-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-126"><a href="#Pathier-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-127"><a href="#Pathier-127"><span class="linenos">127</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-102"><a href="#Pathier-102"><span class="linenos">102</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-103"><a href="#Pathier-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">formatted_size</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Pathier-104"><a href="#Pathier-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;The size of this file or directory formatted with `self.format_bytes()`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-105"><a href="#Pathier-105"><span class="linenos">105</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">)</span>
+</span><span id="Pathier-106"><a href="#Pathier-106"><span class="linenos">106</span></a>
+</span><span id="Pathier-107"><a href="#Pathier-107"><span class="linenos">107</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Pathier-108"><a href="#Pathier-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">format_bytes</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Pathier-109"><a href="#Pathier-109"><span class="linenos">109</span></a>        <span class="sd">&quot;&quot;&quot;Format `size` with common file size abbreviations and rounded to two decimal places.</span>
+</span><span id="Pathier-110"><a href="#Pathier-110"><span class="linenos">110</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-111"><a href="#Pathier-111"><span class="linenos">111</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
+</span><span id="Pathier-112"><a href="#Pathier-112"><span class="linenos">112</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
+</span><span id="Pathier-113"><a href="#Pathier-113"><span class="linenos">113</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
+</span><span id="Pathier-114"><a href="#Pathier-114"><span class="linenos">114</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
+</span><span id="Pathier-115"><a href="#Pathier-115"><span class="linenos">115</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Pathier-116"><a href="#Pathier-116"><span class="linenos">116</span></a>
+</span><span id="Pathier-117"><a href="#Pathier-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-118"><a href="#Pathier-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-119"><a href="#Pathier-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
+</span><span id="Pathier-120"><a href="#Pathier-120"><span class="linenos">120</span></a>
+</span><span id="Pathier-121"><a href="#Pathier-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-122"><a href="#Pathier-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-123"><a href="#Pathier-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
+</span><span id="Pathier-124"><a href="#Pathier-124"><span class="linenos">124</span></a>
+</span><span id="Pathier-125"><a href="#Pathier-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-126"><a href="#Pathier-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified more recently than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-127"><a href="#Pathier-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
 </span><span id="Pathier-128"><a href="#Pathier-128"><span class="linenos">128</span></a>
-</span><span id="Pathier-129"><a href="#Pathier-129"><span class="linenos">129</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-130"><a href="#Pathier-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">in_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-131"><a href="#Pathier-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Return `True` if this path is in `sys.path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier-132"><a href="#Pathier-132"><span class="linenos">132</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="ow">in</span> <span class="n">sys</span><span class="o">.</span><span class="n">path</span>
+</span><span id="Pathier-129"><a href="#Pathier-129"><span class="linenos">129</span></a>    <span class="c1"># ===============================================navigation===============================================</span>
+</span><span id="Pathier-130"><a href="#Pathier-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-131"><a href="#Pathier-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-132"><a href="#Pathier-132"><span class="linenos">132</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
 </span><span id="Pathier-133"><a href="#Pathier-133"><span class="linenos">133</span></a>
-</span><span id="Pathier-134"><a href="#Pathier-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
-</span><span id="Pathier-135"><a href="#Pathier-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into `sys.path` if it isn&#39;t already there.</span>
-</span><span id="Pathier-136"><a href="#Pathier-136"><span class="linenos">136</span></a>
-</span><span id="Pathier-137"><a href="#Pathier-137"><span class="linenos">137</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-134"><a href="#Pathier-134"><span class="linenos">134</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-135"><a href="#Pathier-135"><span class="linenos">135</span></a>    <span class="k">def</span> <span class="nf">in_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-136"><a href="#Pathier-136"><span class="linenos">136</span></a>        <span class="sd">&quot;&quot;&quot;Return `True` if this path is in `sys.path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-137"><a href="#Pathier-137"><span class="linenos">137</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="ow">in</span> <span class="n">sys</span><span class="o">.</span><span class="n">path</span>
 </span><span id="Pathier-138"><a href="#Pathier-138"><span class="linenos">138</span></a>
-</span><span id="Pathier-139"><a href="#Pathier-139"><span class="linenos">139</span></a><span class="sd">        `index`: The index of `sys.path` to insert this path at.&quot;&quot;&quot;</span>
-</span><span id="Pathier-140"><a href="#Pathier-140"><span class="linenos">140</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-141"><a href="#Pathier-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-142"><a href="#Pathier-142"><span class="linenos">142</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
+</span><span id="Pathier-139"><a href="#Pathier-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
+</span><span id="Pathier-140"><a href="#Pathier-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into `sys.path` if it isn&#39;t already there.</span>
+</span><span id="Pathier-141"><a href="#Pathier-141"><span class="linenos">141</span></a>
+</span><span id="Pathier-142"><a href="#Pathier-142"><span class="linenos">142</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier-143"><a href="#Pathier-143"><span class="linenos">143</span></a>
-</span><span id="Pathier-144"><a href="#Pathier-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-145"><a href="#Pathier-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to `sys.path` if it isn&#39;t already there.&quot;&quot;&quot;</span>
-</span><span id="Pathier-146"><a href="#Pathier-146"><span class="linenos">146</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-147"><a href="#Pathier-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-148"><a href="#Pathier-148"><span class="linenos">148</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="Pathier-149"><a href="#Pathier-149"><span class="linenos">149</span></a>
-</span><span id="Pathier-150"><a href="#Pathier-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-151"><a href="#Pathier-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from `sys.path` if it&#39;s in `sys.path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier-152"><a href="#Pathier-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-153"><a href="#Pathier-153"><span class="linenos">153</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
+</span><span id="Pathier-144"><a href="#Pathier-144"><span class="linenos">144</span></a><span class="sd">        `index`: The index of `sys.path` to insert this path at.&quot;&quot;&quot;</span>
+</span><span id="Pathier-145"><a href="#Pathier-145"><span class="linenos">145</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-146"><a href="#Pathier-146"><span class="linenos">146</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-147"><a href="#Pathier-147"><span class="linenos">147</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
+</span><span id="Pathier-148"><a href="#Pathier-148"><span class="linenos">148</span></a>
+</span><span id="Pathier-149"><a href="#Pathier-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-150"><a href="#Pathier-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to `sys.path` if it isn&#39;t already there.&quot;&quot;&quot;</span>
+</span><span id="Pathier-151"><a href="#Pathier-151"><span class="linenos">151</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-152"><a href="#Pathier-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-153"><a href="#Pathier-153"><span class="linenos">153</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
 </span><span id="Pathier-154"><a href="#Pathier-154"><span class="linenos">154</span></a>
-</span><span id="Pathier-155"><a href="#Pathier-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-156"><a href="#Pathier-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is a parent of this instance.</span>
-</span><span id="Pathier-157"><a href="#Pathier-157"><span class="linenos">157</span></a>
-</span><span id="Pathier-158"><a href="#Pathier-158"><span class="linenos">158</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
-</span><span id="Pathier-159"><a href="#Pathier-159"><span class="linenos">159</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier-160"><a href="#Pathier-160"><span class="linenos">160</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
-</span><span id="Pathier-161"><a href="#Pathier-161"><span class="linenos">161</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
-</span><span id="Pathier-162"><a href="#Pathier-162"><span class="linenos">162</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
-</span><span id="Pathier-163"><a href="#Pathier-163"><span class="linenos">163</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-164"><a href="#Pathier-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-165"><a href="#Pathier-165"><span class="linenos">165</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-166"><a href="#Pathier-166"><span class="linenos">166</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
-</span><span id="Pathier-167"><a href="#Pathier-167"><span class="linenos">167</span></a>
-</span><span id="Pathier-168"><a href="#Pathier-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="fm">__sub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">levels</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-169"><a href="#Pathier-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object moved up `levels` number of parents from the current path.</span>
-</span><span id="Pathier-170"><a href="#Pathier-170"><span class="linenos">170</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier-171"><a href="#Pathier-171"><span class="linenos">171</span></a><span class="sd">        &gt;&gt;&gt; new_p = p - 3</span>
-</span><span id="Pathier-172"><a href="#Pathier-172"><span class="linenos">172</span></a><span class="sd">        &gt;&gt;&gt; print(new_p)</span>
-</span><span id="Pathier-173"><a href="#Pathier-173"><span class="linenos">173</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-174"><a href="#Pathier-174"><span class="linenos">174</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span>
-</span><span id="Pathier-175"><a href="#Pathier-175"><span class="linenos">175</span></a>        <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">levels</span><span class="p">):</span>
-</span><span id="Pathier-176"><a href="#Pathier-176"><span class="linenos">176</span></a>            <span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="Pathier-177"><a href="#Pathier-177"><span class="linenos">177</span></a>        <span class="k">return</span> <span class="n">path</span>
-</span><span id="Pathier-178"><a href="#Pathier-178"><span class="linenos">178</span></a>
-</span><span id="Pathier-179"><a href="#Pathier-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-180"><a href="#Pathier-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object such that the stem is one level below the given folder `name`.</span>
-</span><span id="Pathier-181"><a href="#Pathier-181"><span class="linenos">181</span></a>
-</span><span id="Pathier-182"><a href="#Pathier-182"><span class="linenos">182</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
-</span><span id="Pathier-183"><a href="#Pathier-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier-184"><a href="#Pathier-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
-</span><span id="Pathier-185"><a href="#Pathier-185"><span class="linenos">185</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier-186"><a href="#Pathier-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-187"><a href="#Pathier-187"><span class="linenos">187</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-188"><a href="#Pathier-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
-</span><span id="Pathier-189"><a href="#Pathier-189"><span class="linenos">189</span></a>
-</span><span id="Pathier-190"><a href="#Pathier-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-191"><a href="#Pathier-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is the relative child path after `name`.</span>
-</span><span id="Pathier-192"><a href="#Pathier-192"><span class="linenos">192</span></a>
-</span><span id="Pathier-193"><a href="#Pathier-193"><span class="linenos">193</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier-155"><a href="#Pathier-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-156"><a href="#Pathier-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from `sys.path` if it&#39;s in `sys.path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-157"><a href="#Pathier-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-158"><a href="#Pathier-158"><span class="linenos">158</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
+</span><span id="Pathier-159"><a href="#Pathier-159"><span class="linenos">159</span></a>
+</span><span id="Pathier-160"><a href="#Pathier-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-161"><a href="#Pathier-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is a parent of this instance.</span>
+</span><span id="Pathier-162"><a href="#Pathier-162"><span class="linenos">162</span></a>
+</span><span id="Pathier-163"><a href="#Pathier-163"><span class="linenos">163</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier-164"><a href="#Pathier-164"><span class="linenos">164</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier-165"><a href="#Pathier-165"><span class="linenos">165</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
+</span><span id="Pathier-166"><a href="#Pathier-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
+</span><span id="Pathier-167"><a href="#Pathier-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
+</span><span id="Pathier-168"><a href="#Pathier-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-169"><a href="#Pathier-169"><span class="linenos">169</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-170"><a href="#Pathier-170"><span class="linenos">170</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-171"><a href="#Pathier-171"><span class="linenos">171</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
+</span><span id="Pathier-172"><a href="#Pathier-172"><span class="linenos">172</span></a>
+</span><span id="Pathier-173"><a href="#Pathier-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="fm">__sub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">levels</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-174"><a href="#Pathier-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object moved up `levels` number of parents from the current path.</span>
+</span><span id="Pathier-175"><a href="#Pathier-175"><span class="linenos">175</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier-176"><a href="#Pathier-176"><span class="linenos">176</span></a><span class="sd">        &gt;&gt;&gt; new_p = p - 3</span>
+</span><span id="Pathier-177"><a href="#Pathier-177"><span class="linenos">177</span></a><span class="sd">        &gt;&gt;&gt; print(new_p)</span>
+</span><span id="Pathier-178"><a href="#Pathier-178"><span class="linenos">178</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-179"><a href="#Pathier-179"><span class="linenos">179</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span>
+</span><span id="Pathier-180"><a href="#Pathier-180"><span class="linenos">180</span></a>        <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">levels</span><span class="p">):</span>
+</span><span id="Pathier-181"><a href="#Pathier-181"><span class="linenos">181</span></a>            <span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="Pathier-182"><a href="#Pathier-182"><span class="linenos">182</span></a>        <span class="k">return</span> <span class="n">path</span>
+</span><span id="Pathier-183"><a href="#Pathier-183"><span class="linenos">183</span></a>
+</span><span id="Pathier-184"><a href="#Pathier-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-185"><a href="#Pathier-185"><span class="linenos">185</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object such that the stem is one level below the given folder `name`.</span>
+</span><span id="Pathier-186"><a href="#Pathier-186"><span class="linenos">186</span></a>
+</span><span id="Pathier-187"><a href="#Pathier-187"><span class="linenos">187</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier-188"><a href="#Pathier-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier-189"><a href="#Pathier-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
+</span><span id="Pathier-190"><a href="#Pathier-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier-191"><a href="#Pathier-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-192"><a href="#Pathier-192"><span class="linenos">192</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-193"><a href="#Pathier-193"><span class="linenos">193</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
 </span><span id="Pathier-194"><a href="#Pathier-194"><span class="linenos">194</span></a>
-</span><span id="Pathier-195"><a href="#Pathier-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier-196"><a href="#Pathier-196"><span class="linenos">196</span></a>
-</span><span id="Pathier-197"><a href="#Pathier-197"><span class="linenos">197</span></a><span class="sd">        `keep_name`: If `True`, the returned path will start with `name`.</span>
-</span><span id="Pathier-198"><a href="#Pathier-198"><span class="linenos">198</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier-199"><a href="#Pathier-199"><span class="linenos">199</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
-</span><span id="Pathier-200"><a href="#Pathier-200"><span class="linenos">200</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
-</span><span id="Pathier-201"><a href="#Pathier-201"><span class="linenos">201</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
-</span><span id="Pathier-202"><a href="#Pathier-202"><span class="linenos">202</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier-203"><a href="#Pathier-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-204"><a href="#Pathier-204"><span class="linenos">204</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-205"><a href="#Pathier-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
-</span><span id="Pathier-206"><a href="#Pathier-206"><span class="linenos">206</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
-</span><span id="Pathier-207"><a href="#Pathier-207"><span class="linenos">207</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
-</span><span id="Pathier-208"><a href="#Pathier-208"><span class="linenos">208</span></a>
-</span><span id="Pathier-209"><a href="#Pathier-209"><span class="linenos">209</span></a>    <span class="c1"># ============================================write and read============================================</span>
-</span><span id="Pathier-210"><a href="#Pathier-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-211"><a href="#Pathier-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
-</span><span id="Pathier-212"><a href="#Pathier-212"><span class="linenos">212</span></a>
-</span><span id="Pathier-213"><a href="#Pathier-213"><span class="linenos">213</span></a><span class="sd">        Same as `Path().mkdir()` except `parents` and `exist_ok` default to `True` instead of `False`.&quot;&quot;&quot;</span>
-</span><span id="Pathier-214"><a href="#Pathier-214"><span class="linenos">214</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
-</span><span id="Pathier-215"><a href="#Pathier-215"><span class="linenos">215</span></a>
-</span><span id="Pathier-216"><a href="#Pathier-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-217"><a href="#Pathier-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Create file (and parents if necessary).&quot;&quot;&quot;</span>
-</span><span id="Pathier-218"><a href="#Pathier-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="Pathier-219"><a href="#Pathier-219"><span class="linenos">219</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+</span><span id="Pathier-195"><a href="#Pathier-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-196"><a href="#Pathier-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is the relative child path after `name`.</span>
+</span><span id="Pathier-197"><a href="#Pathier-197"><span class="linenos">197</span></a>
+</span><span id="Pathier-198"><a href="#Pathier-198"><span class="linenos">198</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier-199"><a href="#Pathier-199"><span class="linenos">199</span></a>
+</span><span id="Pathier-200"><a href="#Pathier-200"><span class="linenos">200</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-201"><a href="#Pathier-201"><span class="linenos">201</span></a>
+</span><span id="Pathier-202"><a href="#Pathier-202"><span class="linenos">202</span></a><span class="sd">        `keep_name`: If `True`, the returned path will start with `name`.</span>
+</span><span id="Pathier-203"><a href="#Pathier-203"><span class="linenos">203</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier-204"><a href="#Pathier-204"><span class="linenos">204</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
+</span><span id="Pathier-205"><a href="#Pathier-205"><span class="linenos">205</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
+</span><span id="Pathier-206"><a href="#Pathier-206"><span class="linenos">206</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
+</span><span id="Pathier-207"><a href="#Pathier-207"><span class="linenos">207</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier-208"><a href="#Pathier-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-209"><a href="#Pathier-209"><span class="linenos">209</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-210"><a href="#Pathier-210"><span class="linenos">210</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
+</span><span id="Pathier-211"><a href="#Pathier-211"><span class="linenos">211</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
+</span><span id="Pathier-212"><a href="#Pathier-212"><span class="linenos">212</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
+</span><span id="Pathier-213"><a href="#Pathier-213"><span class="linenos">213</span></a>
+</span><span id="Pathier-214"><a href="#Pathier-214"><span class="linenos">214</span></a>    <span class="c1"># ============================================write and read============================================</span>
+</span><span id="Pathier-215"><a href="#Pathier-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-216"><a href="#Pathier-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
+</span><span id="Pathier-217"><a href="#Pathier-217"><span class="linenos">217</span></a>
+</span><span id="Pathier-218"><a href="#Pathier-218"><span class="linenos">218</span></a><span class="sd">        Same as `Path().mkdir()` except `parents` and `exist_ok` default to `True` instead of `False`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-219"><a href="#Pathier-219"><span class="linenos">219</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
 </span><span id="Pathier-220"><a href="#Pathier-220"><span class="linenos">220</span></a>
-</span><span id="Pathier-221"><a href="#Pathier-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s2">&quot;r&quot;</span><span class="p">,</span> <span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">newline</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="Pathier-222"><a href="#Pathier-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Pathier-223"><a href="#Pathier-223"><span class="linenos">223</span></a><span class="sd">        Open the file pointed by this path and return a file object, as</span>
-</span><span id="Pathier-224"><a href="#Pathier-224"><span class="linenos">224</span></a><span class="sd">        the built-in open() function does.</span>
-</span><span id="Pathier-225"><a href="#Pathier-225"><span class="linenos">225</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Pathier-226"><a href="#Pathier-226"><span class="linenos">226</span></a>        <span class="n">stream</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">buffering</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">)</span>
-</span><span id="Pathier-227"><a href="#Pathier-227"><span class="linenos">227</span></a>        <span class="k">if</span> <span class="s2">&quot;r&quot;</span> <span class="ow">in</span> <span class="n">mode</span><span class="p">:</span>
-</span><span id="Pathier-228"><a href="#Pathier-228"><span class="linenos">228</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Pathier-229"><a href="#Pathier-229"><span class="linenos">229</span></a>        <span class="k">return</span> <span class="n">stream</span>
-</span><span id="Pathier-230"><a href="#Pathier-230"><span class="linenos">230</span></a>
-</span><span id="Pathier-231"><a href="#Pathier-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
-</span><span id="Pathier-232"><a href="#Pathier-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-233"><a href="#Pathier-233"><span class="linenos">233</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-234"><a href="#Pathier-234"><span class="linenos">234</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-235"><a href="#Pathier-235"><span class="linenos">235</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-236"><a href="#Pathier-236"><span class="linenos">236</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-237"><a href="#Pathier-237"><span class="linenos">237</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-238"><a href="#Pathier-238"><span class="linenos">238</span></a>    <span class="p">):</span>
-</span><span id="Pathier-239"><a href="#Pathier-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file.</span>
-</span><span id="Pathier-240"><a href="#Pathier-240"><span class="linenos">240</span></a>
-</span><span id="Pathier-241"><a href="#Pathier-241"><span class="linenos">241</span></a><span class="sd">        If a `TypeError` is raised, the function  will attempt to cast `data` to a `str` and try the write again.</span>
-</span><span id="Pathier-242"><a href="#Pathier-242"><span class="linenos">242</span></a>
-</span><span id="Pathier-243"><a href="#Pathier-243"><span class="linenos">243</span></a><span class="sd">        If a `FileNotFoundError` is raised and `parents = True`, `self.parent` will be created.&quot;&quot;&quot;</span>
-</span><span id="Pathier-244"><a href="#Pathier-244"><span class="linenos">244</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
-</span><span id="Pathier-245"><a href="#Pathier-245"><span class="linenos">245</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
-</span><span id="Pathier-246"><a href="#Pathier-246"><span class="linenos">246</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier-247"><a href="#Pathier-247"><span class="linenos">247</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier-248"><a href="#Pathier-248"><span class="linenos">248</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier-249"><a href="#Pathier-249"><span class="linenos">249</span></a>        <span class="p">)</span>
-</span><span id="Pathier-250"><a href="#Pathier-250"><span class="linenos">250</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier-251"><a href="#Pathier-251"><span class="linenos">251</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-252"><a href="#Pathier-252"><span class="linenos">252</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
-</span><span id="Pathier-253"><a href="#Pathier-253"><span class="linenos">253</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-254"><a href="#Pathier-254"><span class="linenos">254</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-255"><a href="#Pathier-255"><span class="linenos">255</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier-256"><a href="#Pathier-256"><span class="linenos">256</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier-257"><a href="#Pathier-257"><span class="linenos">257</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-258"><a href="#Pathier-258"><span class="linenos">258</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-259"><a href="#Pathier-259"><span class="linenos">259</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-260"><a href="#Pathier-260"><span class="linenos">260</span></a>                <span class="k">raise</span>
-</span><span id="Pathier-261"><a href="#Pathier-261"><span class="linenos">261</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier-262"><a href="#Pathier-262"><span class="linenos">262</span></a>            <span class="k">raise</span>
-</span><span id="Pathier-263"><a href="#Pathier-263"><span class="linenos">263</span></a>
-</span><span id="Pathier-264"><a href="#Pathier-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-265"><a href="#Pathier-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
-</span><span id="Pathier-266"><a href="#Pathier-266"><span class="linenos">266</span></a>
-</span><span id="Pathier-267"><a href="#Pathier-267"><span class="linenos">267</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-221"><a href="#Pathier-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-222"><a href="#Pathier-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;Create file (and parents if necessary).&quot;&quot;&quot;</span>
+</span><span id="Pathier-223"><a href="#Pathier-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="Pathier-224"><a href="#Pathier-224"><span class="linenos">224</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+</span><span id="Pathier-225"><a href="#Pathier-225"><span class="linenos">225</span></a>
+</span><span id="Pathier-226"><a href="#Pathier-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s2">&quot;r&quot;</span><span class="p">,</span> <span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">newline</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier-227"><a href="#Pathier-227"><span class="linenos">227</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Pathier-228"><a href="#Pathier-228"><span class="linenos">228</span></a><span class="sd">        Open the file pointed by this path and return a file object, as</span>
+</span><span id="Pathier-229"><a href="#Pathier-229"><span class="linenos">229</span></a><span class="sd">        the built-in open() function does.</span>
+</span><span id="Pathier-230"><a href="#Pathier-230"><span class="linenos">230</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Pathier-231"><a href="#Pathier-231"><span class="linenos">231</span></a>        <span class="n">stream</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">buffering</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">)</span>
+</span><span id="Pathier-232"><a href="#Pathier-232"><span class="linenos">232</span></a>        <span class="k">if</span> <span class="s2">&quot;r&quot;</span> <span class="ow">in</span> <span class="n">mode</span><span class="p">:</span>
+</span><span id="Pathier-233"><a href="#Pathier-233"><span class="linenos">233</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Pathier-234"><a href="#Pathier-234"><span class="linenos">234</span></a>        <span class="k">return</span> <span class="n">stream</span>
+</span><span id="Pathier-235"><a href="#Pathier-235"><span class="linenos">235</span></a>
+</span><span id="Pathier-236"><a href="#Pathier-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
+</span><span id="Pathier-237"><a href="#Pathier-237"><span class="linenos">237</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-238"><a href="#Pathier-238"><span class="linenos">238</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-239"><a href="#Pathier-239"><span class="linenos">239</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-240"><a href="#Pathier-240"><span class="linenos">240</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-241"><a href="#Pathier-241"><span class="linenos">241</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-242"><a href="#Pathier-242"><span class="linenos">242</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-243"><a href="#Pathier-243"><span class="linenos">243</span></a>    <span class="p">):</span>
+</span><span id="Pathier-244"><a href="#Pathier-244"><span class="linenos">244</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file.</span>
+</span><span id="Pathier-245"><a href="#Pathier-245"><span class="linenos">245</span></a>
+</span><span id="Pathier-246"><a href="#Pathier-246"><span class="linenos">246</span></a><span class="sd">        If a `TypeError` is raised, the function  will attempt to cast `data` to a `str` and try the write again.</span>
+</span><span id="Pathier-247"><a href="#Pathier-247"><span class="linenos">247</span></a>
+</span><span id="Pathier-248"><a href="#Pathier-248"><span class="linenos">248</span></a><span class="sd">        If a `FileNotFoundError` is raised and `parents = True`, `self.parent` will be created.&quot;&quot;&quot;</span>
+</span><span id="Pathier-249"><a href="#Pathier-249"><span class="linenos">249</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
+</span><span id="Pathier-250"><a href="#Pathier-250"><span class="linenos">250</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
+</span><span id="Pathier-251"><a href="#Pathier-251"><span class="linenos">251</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier-252"><a href="#Pathier-252"><span class="linenos">252</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier-253"><a href="#Pathier-253"><span class="linenos">253</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier-254"><a href="#Pathier-254"><span class="linenos">254</span></a>        <span class="p">)</span>
+</span><span id="Pathier-255"><a href="#Pathier-255"><span class="linenos">255</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier-256"><a href="#Pathier-256"><span class="linenos">256</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-257"><a href="#Pathier-257"><span class="linenos">257</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
+</span><span id="Pathier-258"><a href="#Pathier-258"><span class="linenos">258</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-259"><a href="#Pathier-259"><span class="linenos">259</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-260"><a href="#Pathier-260"><span class="linenos">260</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier-261"><a href="#Pathier-261"><span class="linenos">261</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier-262"><a href="#Pathier-262"><span class="linenos">262</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-263"><a href="#Pathier-263"><span class="linenos">263</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-264"><a href="#Pathier-264"><span class="linenos">264</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-265"><a href="#Pathier-265"><span class="linenos">265</span></a>                <span class="k">raise</span>
+</span><span id="Pathier-266"><a href="#Pathier-266"><span class="linenos">266</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier-267"><a href="#Pathier-267"><span class="linenos">267</span></a>            <span class="k">raise</span>
 </span><span id="Pathier-268"><a href="#Pathier-268"><span class="linenos">268</span></a>
-</span><span id="Pathier-269"><a href="#Pathier-269"><span class="linenos">269</span></a><span class="sd">        `parents`: If `True` and the write operation fails with a `FileNotFoundError`,</span>
-</span><span id="Pathier-270"><a href="#Pathier-270"><span class="linenos">270</span></a><span class="sd">        make the parent directory and retry the write.&quot;&quot;&quot;</span>
-</span><span id="Pathier-271"><a href="#Pathier-271"><span class="linenos">271</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier-272"><a href="#Pathier-272"><span class="linenos">272</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-273"><a href="#Pathier-273"><span class="linenos">273</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier-274"><a href="#Pathier-274"><span class="linenos">274</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier-275"><a href="#Pathier-275"><span class="linenos">275</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-276"><a href="#Pathier-276"><span class="linenos">276</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-277"><a href="#Pathier-277"><span class="linenos">277</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-278"><a href="#Pathier-278"><span class="linenos">278</span></a>                <span class="k">raise</span>
-</span><span id="Pathier-279"><a href="#Pathier-279"><span class="linenos">279</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier-280"><a href="#Pathier-280"><span class="linenos">280</span></a>            <span class="k">raise</span>
-</span><span id="Pathier-281"><a href="#Pathier-281"><span class="linenos">281</span></a>
-</span><span id="Pathier-282"><a href="#Pathier-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">append</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="Pathier-283"><a href="#Pathier-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Append `data` to the file pointed to by this `Pathier` object.</span>
-</span><span id="Pathier-284"><a href="#Pathier-284"><span class="linenos">284</span></a>
-</span><span id="Pathier-285"><a href="#Pathier-285"><span class="linenos">285</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-269"><a href="#Pathier-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-270"><a href="#Pathier-270"><span class="linenos">270</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
+</span><span id="Pathier-271"><a href="#Pathier-271"><span class="linenos">271</span></a>
+</span><span id="Pathier-272"><a href="#Pathier-272"><span class="linenos">272</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-273"><a href="#Pathier-273"><span class="linenos">273</span></a>
+</span><span id="Pathier-274"><a href="#Pathier-274"><span class="linenos">274</span></a><span class="sd">        `parents`: If `True` and the write operation fails with a `FileNotFoundError`,</span>
+</span><span id="Pathier-275"><a href="#Pathier-275"><span class="linenos">275</span></a><span class="sd">        make the parent directory and retry the write.&quot;&quot;&quot;</span>
+</span><span id="Pathier-276"><a href="#Pathier-276"><span class="linenos">276</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier-277"><a href="#Pathier-277"><span class="linenos">277</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-278"><a href="#Pathier-278"><span class="linenos">278</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier-279"><a href="#Pathier-279"><span class="linenos">279</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier-280"><a href="#Pathier-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-281"><a href="#Pathier-281"><span class="linenos">281</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-282"><a href="#Pathier-282"><span class="linenos">282</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-283"><a href="#Pathier-283"><span class="linenos">283</span></a>                <span class="k">raise</span>
+</span><span id="Pathier-284"><a href="#Pathier-284"><span class="linenos">284</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier-285"><a href="#Pathier-285"><span class="linenos">285</span></a>            <span class="k">raise</span>
 </span><span id="Pathier-286"><a href="#Pathier-286"><span class="linenos">286</span></a>
-</span><span id="Pathier-287"><a href="#Pathier-287"><span class="linenos">287</span></a><span class="sd">        `new_line`: If `True`, add `\\n` to `data`.</span>
-</span><span id="Pathier-288"><a href="#Pathier-288"><span class="linenos">288</span></a>
-</span><span id="Pathier-289"><a href="#Pathier-289"><span class="linenos">289</span></a><span class="sd">        `encoding`: The file encoding to use.&quot;&quot;&quot;</span>
-</span><span id="Pathier-290"><a href="#Pathier-290"><span class="linenos">290</span></a>        <span class="k">if</span> <span class="n">new_line</span><span class="p">:</span>
-</span><span id="Pathier-291"><a href="#Pathier-291"><span class="linenos">291</span></a>            <span class="n">data</span> <span class="o">+=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="Pathier-292"><a href="#Pathier-292"><span class="linenos">292</span></a>        <span class="k">with</span> <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;a&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
-</span><span id="Pathier-293"><a href="#Pathier-293"><span class="linenos">293</span></a>            <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-294"><a href="#Pathier-294"><span class="linenos">294</span></a>
-</span><span id="Pathier-295"><a href="#Pathier-295"><span class="linenos">295</span></a>    <span class="k">def</span> <span class="nf">replace</span><span class="p">(</span>
-</span><span id="Pathier-296"><a href="#Pathier-296"><span class="linenos">296</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-297"><a href="#Pathier-297"><span class="linenos">297</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
-</span><span id="Pathier-298"><a href="#Pathier-298"><span class="linenos">298</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
-</span><span id="Pathier-299"><a href="#Pathier-299"><span class="linenos">299</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-300"><a href="#Pathier-300"><span class="linenos">300</span></a>    <span class="p">):</span>
-</span><span id="Pathier-301"><a href="#Pathier-301"><span class="linenos">301</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
-</span><span id="Pathier-302"><a href="#Pathier-302"><span class="linenos">302</span></a>
-</span><span id="Pathier-303"><a href="#Pathier-303"><span class="linenos">303</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier-304"><a href="#Pathier-304"><span class="linenos">304</span></a>
-</span><span id="Pathier-305"><a href="#Pathier-305"><span class="linenos">305</span></a><span class="sd">        `count`: Only replace this many occurences of each pair.</span>
-</span><span id="Pathier-306"><a href="#Pathier-306"><span class="linenos">306</span></a><span class="sd">        By default (`-1`), all occurences are replaced.</span>
+</span><span id="Pathier-287"><a href="#Pathier-287"><span class="linenos">287</span></a>    <span class="k">def</span> <span class="nf">append</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier-288"><a href="#Pathier-288"><span class="linenos">288</span></a>        <span class="sd">&quot;&quot;&quot;Append `data` to the file pointed to by this `Pathier` object.</span>
+</span><span id="Pathier-289"><a href="#Pathier-289"><span class="linenos">289</span></a>
+</span><span id="Pathier-290"><a href="#Pathier-290"><span class="linenos">290</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-291"><a href="#Pathier-291"><span class="linenos">291</span></a>
+</span><span id="Pathier-292"><a href="#Pathier-292"><span class="linenos">292</span></a><span class="sd">        `new_line`: If `True`, add `\\n` to `data`.</span>
+</span><span id="Pathier-293"><a href="#Pathier-293"><span class="linenos">293</span></a>
+</span><span id="Pathier-294"><a href="#Pathier-294"><span class="linenos">294</span></a><span class="sd">        `encoding`: The file encoding to use.&quot;&quot;&quot;</span>
+</span><span id="Pathier-295"><a href="#Pathier-295"><span class="linenos">295</span></a>        <span class="k">if</span> <span class="n">new_line</span><span class="p">:</span>
+</span><span id="Pathier-296"><a href="#Pathier-296"><span class="linenos">296</span></a>            <span class="n">data</span> <span class="o">+=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="Pathier-297"><a href="#Pathier-297"><span class="linenos">297</span></a>        <span class="k">with</span> <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;a&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
+</span><span id="Pathier-298"><a href="#Pathier-298"><span class="linenos">298</span></a>            <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-299"><a href="#Pathier-299"><span class="linenos">299</span></a>
+</span><span id="Pathier-300"><a href="#Pathier-300"><span class="linenos">300</span></a>    <span class="k">def</span> <span class="nf">replace</span><span class="p">(</span>
+</span><span id="Pathier-301"><a href="#Pathier-301"><span class="linenos">301</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-302"><a href="#Pathier-302"><span class="linenos">302</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
+</span><span id="Pathier-303"><a href="#Pathier-303"><span class="linenos">303</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
+</span><span id="Pathier-304"><a href="#Pathier-304"><span class="linenos">304</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-305"><a href="#Pathier-305"><span class="linenos">305</span></a>    <span class="p">):</span>
+</span><span id="Pathier-306"><a href="#Pathier-306"><span class="linenos">306</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
 </span><span id="Pathier-307"><a href="#Pathier-307"><span class="linenos">307</span></a>
-</span><span id="Pathier-308"><a href="#Pathier-308"><span class="linenos">308</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier-308"><a href="#Pathier-308"><span class="linenos">308</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier-309"><a href="#Pathier-309"><span class="linenos">309</span></a>
-</span><span id="Pathier-310"><a href="#Pathier-310"><span class="linenos">310</span></a><span class="sd">        e.g.</span>
-</span><span id="Pathier-311"><a href="#Pathier-311"><span class="linenos">311</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;somefile.txt&quot;)</span>
-</span><span id="Pathier-312"><a href="#Pathier-312"><span class="linenos">312</span></a><span class="sd">        &gt;&gt;&gt;</span>
-</span><span id="Pathier-313"><a href="#Pathier-313"><span class="linenos">313</span></a><span class="sd">        &gt;&gt;&gt; path.replace([(&quot;hello&quot;, &quot;yeet&quot;), (&quot;goodbye&quot;, &quot;yeehaw&quot;)])</span>
-</span><span id="Pathier-314"><a href="#Pathier-314"><span class="linenos">314</span></a><span class="sd">        equivalent to</span>
-</span><span id="Pathier-315"><a href="#Pathier-315"><span class="linenos">315</span></a><span class="sd">        &gt;&gt;&gt; path.write_text(path.read_text().replace(&quot;hello&quot;, &quot;yeet&quot;).replace(&quot;goodbye&quot;, &quot;yeehaw&quot;))&quot;&quot;&quot;</span>
-</span><span id="Pathier-316"><a href="#Pathier-316"><span class="linenos">316</span></a>        <span class="n">text</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">)</span>
-</span><span id="Pathier-317"><a href="#Pathier-317"><span class="linenos">317</span></a>        <span class="k">for</span> <span class="n">sub</span> <span class="ow">in</span> <span class="n">substitutions</span><span class="p">:</span>
-</span><span id="Pathier-318"><a href="#Pathier-318"><span class="linenos">318</span></a>            <span class="n">text</span> <span class="o">=</span> <span class="n">text</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">sub</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">sub</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">count</span><span class="p">)</span>
-</span><span id="Pathier-319"><a href="#Pathier-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">text</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
-</span><span id="Pathier-320"><a href="#Pathier-320"><span class="linenos">320</span></a>
-</span><span id="Pathier-321"><a href="#Pathier-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
-</span><span id="Pathier-322"><a href="#Pathier-322"><span class="linenos">322</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
-</span><span id="Pathier-323"><a href="#Pathier-323"><span class="linenos">323</span></a>
-</span><span id="Pathier-324"><a href="#Pathier-324"><span class="linenos">324</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
+</span><span id="Pathier-310"><a href="#Pathier-310"><span class="linenos">310</span></a><span class="sd">        `count`: Only replace this many occurences of each pair.</span>
+</span><span id="Pathier-311"><a href="#Pathier-311"><span class="linenos">311</span></a><span class="sd">        By default (`-1`), all occurences are replaced.</span>
+</span><span id="Pathier-312"><a href="#Pathier-312"><span class="linenos">312</span></a>
+</span><span id="Pathier-313"><a href="#Pathier-313"><span class="linenos">313</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier-314"><a href="#Pathier-314"><span class="linenos">314</span></a>
+</span><span id="Pathier-315"><a href="#Pathier-315"><span class="linenos">315</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier-316"><a href="#Pathier-316"><span class="linenos">316</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;somefile.txt&quot;)</span>
+</span><span id="Pathier-317"><a href="#Pathier-317"><span class="linenos">317</span></a><span class="sd">        &gt;&gt;&gt;</span>
+</span><span id="Pathier-318"><a href="#Pathier-318"><span class="linenos">318</span></a><span class="sd">        &gt;&gt;&gt; path.replace([(&quot;hello&quot;, &quot;yeet&quot;), (&quot;goodbye&quot;, &quot;yeehaw&quot;)])</span>
+</span><span id="Pathier-319"><a href="#Pathier-319"><span class="linenos">319</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier-320"><a href="#Pathier-320"><span class="linenos">320</span></a><span class="sd">        &gt;&gt;&gt; path.write_text(path.read_text().replace(&quot;hello&quot;, &quot;yeet&quot;).replace(&quot;goodbye&quot;, &quot;yeehaw&quot;))&quot;&quot;&quot;</span>
+</span><span id="Pathier-321"><a href="#Pathier-321"><span class="linenos">321</span></a>        <span class="n">text</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier-322"><a href="#Pathier-322"><span class="linenos">322</span></a>        <span class="k">for</span> <span class="n">sub</span> <span class="ow">in</span> <span class="n">substitutions</span><span class="p">:</span>
+</span><span id="Pathier-323"><a href="#Pathier-323"><span class="linenos">323</span></a>            <span class="n">text</span> <span class="o">=</span> <span class="n">text</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">sub</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">sub</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">count</span><span class="p">)</span>
+</span><span id="Pathier-324"><a href="#Pathier-324"><span class="linenos">324</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">text</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
 </span><span id="Pathier-325"><a href="#Pathier-325"><span class="linenos">325</span></a>
-</span><span id="Pathier-326"><a href="#Pathier-326"><span class="linenos">326</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier-327"><a href="#Pathier-327"><span class="linenos">327</span></a>
-</span><span id="Pathier-328"><a href="#Pathier-328"><span class="linenos">328</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
-</span><span id="Pathier-329"><a href="#Pathier-329"><span class="linenos">329</span></a>
-</span><span id="Pathier-330"><a href="#Pathier-330"><span class="linenos">330</span></a><span class="sd">        `sep`: The separator to use when joining `data`.&quot;&quot;&quot;</span>
-</span><span id="Pathier-331"><a href="#Pathier-331"><span class="linenos">331</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">sep</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">data</span><span class="p">),</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier-326"><a href="#Pathier-326"><span class="linenos">326</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
+</span><span id="Pathier-327"><a href="#Pathier-327"><span class="linenos">327</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
+</span><span id="Pathier-328"><a href="#Pathier-328"><span class="linenos">328</span></a>
+</span><span id="Pathier-329"><a href="#Pathier-329"><span class="linenos">329</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
+</span><span id="Pathier-330"><a href="#Pathier-330"><span class="linenos">330</span></a>
+</span><span id="Pathier-331"><a href="#Pathier-331"><span class="linenos">331</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier-332"><a href="#Pathier-332"><span class="linenos">332</span></a>
-</span><span id="Pathier-333"><a href="#Pathier-333"><span class="linenos">333</span></a>    <span class="k">def</span> <span class="nf">split</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="Pathier-334"><a href="#Pathier-334"><span class="linenos">334</span></a>        <span class="sd">&quot;&quot;&quot;Returns the content of the pointed at file as a list of strings, splitting at new line characters.</span>
-</span><span id="Pathier-335"><a href="#Pathier-335"><span class="linenos">335</span></a>
-</span><span id="Pathier-336"><a href="#Pathier-336"><span class="linenos">336</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).read_text(encoding=encoding).splitlines()`</span>
+</span><span id="Pathier-333"><a href="#Pathier-333"><span class="linenos">333</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier-334"><a href="#Pathier-334"><span class="linenos">334</span></a>
+</span><span id="Pathier-335"><a href="#Pathier-335"><span class="linenos">335</span></a><span class="sd">        `sep`: The separator to use when joining `data`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-336"><a href="#Pathier-336"><span class="linenos">336</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">sep</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">data</span><span class="p">),</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
 </span><span id="Pathier-337"><a href="#Pathier-337"><span class="linenos">337</span></a>
-</span><span id="Pathier-338"><a href="#Pathier-338"><span class="linenos">338</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier-339"><a href="#Pathier-339"><span class="linenos">339</span></a>
-</span><span id="Pathier-340"><a href="#Pathier-340"><span class="linenos">340</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
-</span><span id="Pathier-341"><a href="#Pathier-341"><span class="linenos">341</span></a>
-</span><span id="Pathier-342"><a href="#Pathier-342"><span class="linenos">342</span></a><span class="sd">        `keepend`: If `True`, line breaks will be included in returned strings.&quot;&quot;&quot;</span>
-</span><span id="Pathier-343"><a href="#Pathier-343"><span class="linenos">343</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="n">keepends</span><span class="p">)</span>
+</span><span id="Pathier-338"><a href="#Pathier-338"><span class="linenos">338</span></a>    <span class="k">def</span> <span class="nf">split</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Pathier-339"><a href="#Pathier-339"><span class="linenos">339</span></a>        <span class="sd">&quot;&quot;&quot;Returns the content of the pointed at file as a list of strings, splitting at new line characters.</span>
+</span><span id="Pathier-340"><a href="#Pathier-340"><span class="linenos">340</span></a>
+</span><span id="Pathier-341"><a href="#Pathier-341"><span class="linenos">341</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).read_text(encoding=encoding).splitlines()`</span>
+</span><span id="Pathier-342"><a href="#Pathier-342"><span class="linenos">342</span></a>
+</span><span id="Pathier-343"><a href="#Pathier-343"><span class="linenos">343</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier-344"><a href="#Pathier-344"><span class="linenos">344</span></a>
-</span><span id="Pathier-345"><a href="#Pathier-345"><span class="linenos">345</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-346"><a href="#Pathier-346"><span class="linenos">346</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-347"><a href="#Pathier-347"><span class="linenos">347</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
-</span><span id="Pathier-348"><a href="#Pathier-348"><span class="linenos">348</span></a>
-</span><span id="Pathier-349"><a href="#Pathier-349"><span class="linenos">349</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier-350"><a href="#Pathier-350"><span class="linenos">350</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-351"><a href="#Pathier-351"><span class="linenos">351</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-352"><a href="#Pathier-352"><span class="linenos">352</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-353"><a href="#Pathier-353"><span class="linenos">353</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-354"><a href="#Pathier-354"><span class="linenos">354</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-355"><a href="#Pathier-355"><span class="linenos">355</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-356"><a href="#Pathier-356"><span class="linenos">356</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-357"><a href="#Pathier-357"><span class="linenos">357</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-358"><a href="#Pathier-358"><span class="linenos">358</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-359"><a href="#Pathier-359"><span class="linenos">359</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-360"><a href="#Pathier-360"><span class="linenos">360</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-361"><a href="#Pathier-361"><span class="linenos">361</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier-362"><a href="#Pathier-362"><span class="linenos">362</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
-</span><span id="Pathier-363"><a href="#Pathier-363"><span class="linenos">363</span></a>            <span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier-364"><a href="#Pathier-364"><span class="linenos">364</span></a>            <span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier-365"><a href="#Pathier-365"><span class="linenos">365</span></a>            <span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier-366"><a href="#Pathier-366"><span class="linenos">366</span></a>            <span class="n">parents</span><span class="p">,</span>
-</span><span id="Pathier-367"><a href="#Pathier-367"><span class="linenos">367</span></a>        <span class="p">)</span>
-</span><span id="Pathier-368"><a href="#Pathier-368"><span class="linenos">368</span></a>
-</span><span id="Pathier-369"><a href="#Pathier-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-370"><a href="#Pathier-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-371"><a href="#Pathier-371"><span class="linenos">371</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span><span class="o">.</span><span class="n">unwrap</span><span class="p">()</span>
-</span><span id="Pathier-372"><a href="#Pathier-372"><span class="linenos">372</span></a>
-</span><span id="Pathier-373"><a href="#Pathier-373"><span class="linenos">373</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
-</span><span id="Pathier-374"><a href="#Pathier-374"><span class="linenos">374</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-375"><a href="#Pathier-375"><span class="linenos">375</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-376"><a href="#Pathier-376"><span class="linenos">376</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-377"><a href="#Pathier-377"><span class="linenos">377</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-378"><a href="#Pathier-378"><span class="linenos">378</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-379"><a href="#Pathier-379"><span class="linenos">379</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-380"><a href="#Pathier-380"><span class="linenos">380</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-381"><a href="#Pathier-381"><span class="linenos">381</span></a>    <span class="p">):</span>
-</span><span id="Pathier-382"><a href="#Pathier-382"><span class="linenos">382</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-383"><a href="#Pathier-383"><span class="linenos">383</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier-384"><a href="#Pathier-384"><span class="linenos">384</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier-385"><a href="#Pathier-385"><span class="linenos">385</span></a>        <span class="p">)</span>
-</span><span id="Pathier-386"><a href="#Pathier-386"><span class="linenos">386</span></a>
-</span><span id="Pathier-387"><a href="#Pathier-387"><span class="linenos">387</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-388"><a href="#Pathier-388"><span class="linenos">388</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier-389"><a href="#Pathier-389"><span class="linenos">389</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier-390"><a href="#Pathier-390"><span class="linenos">390</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier-391"><a href="#Pathier-391"><span class="linenos">391</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier-392"><a href="#Pathier-392"><span class="linenos">392</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier-393"><a href="#Pathier-393"><span class="linenos">393</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier-394"><a href="#Pathier-394"><span class="linenos">394</span></a>
-</span><span id="Pathier-395"><a href="#Pathier-395"><span class="linenos">395</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
-</span><span id="Pathier-396"><a href="#Pathier-396"><span class="linenos">396</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-397"><a href="#Pathier-397"><span class="linenos">397</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-398"><a href="#Pathier-398"><span class="linenos">398</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-399"><a href="#Pathier-399"><span class="linenos">399</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-400"><a href="#Pathier-400"><span class="linenos">400</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-401"><a href="#Pathier-401"><span class="linenos">401</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-402"><a href="#Pathier-402"><span class="linenos">402</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-403"><a href="#Pathier-403"><span class="linenos">403</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-404"><a href="#Pathier-404"><span class="linenos">404</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-405"><a href="#Pathier-405"><span class="linenos">405</span></a>    <span class="p">):</span>
-</span><span id="Pathier-406"><a href="#Pathier-406"><span class="linenos">406</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier-407"><a href="#Pathier-407"><span class="linenos">407</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier-408"><a href="#Pathier-408"><span class="linenos">408</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier-409"><a href="#Pathier-409"><span class="linenos">409</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier-410"><a href="#Pathier-410"><span class="linenos">410</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier-411"><a href="#Pathier-411"><span class="linenos">411</span></a>                <span class="p">)</span>
-</span><span id="Pathier-412"><a href="#Pathier-412"><span class="linenos">412</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier-413"><a href="#Pathier-413"><span class="linenos">413</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
-</span><span id="Pathier-414"><a href="#Pathier-414"><span class="linenos">414</span></a>
-</span><span id="Pathier-415"><a href="#Pathier-415"><span class="linenos">415</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-416"><a href="#Pathier-416"><span class="linenos">416</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
-</span><span id="Pathier-417"><a href="#Pathier-417"><span class="linenos">417</span></a>
-</span><span id="Pathier-418"><a href="#Pathier-418"><span class="linenos">418</span></a><span class="sd">        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-419"><a href="#Pathier-419"><span class="linenos">419</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-420"><a href="#Pathier-420"><span class="linenos">420</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
-</span><span id="Pathier-421"><a href="#Pathier-421"><span class="linenos">421</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-422"><a href="#Pathier-422"><span class="linenos">422</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-423"><a href="#Pathier-423"><span class="linenos">423</span></a>
-</span><span id="Pathier-424"><a href="#Pathier-424"><span class="linenos">424</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
-</span><span id="Pathier-425"><a href="#Pathier-425"><span class="linenos">425</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Pathier-426"><a href="#Pathier-426"><span class="linenos">426</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-427"><a href="#Pathier-427"><span class="linenos">427</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
-</span><span id="Pathier-428"><a href="#Pathier-428"><span class="linenos">428</span></a><span class="sd">        to the instance pointed to by `new_path` using `shutil.copyfile`</span>
-</span><span id="Pathier-429"><a href="#Pathier-429"><span class="linenos">429</span></a><span class="sd">        or `shutil.copytree`.</span>
-</span><span id="Pathier-430"><a href="#Pathier-430"><span class="linenos">430</span></a>
-</span><span id="Pathier-431"><a href="#Pathier-431"><span class="linenos">431</span></a><span class="sd">        Returns the new path.</span>
-</span><span id="Pathier-432"><a href="#Pathier-432"><span class="linenos">432</span></a>
-</span><span id="Pathier-433"><a href="#Pathier-433"><span class="linenos">433</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier-434"><a href="#Pathier-434"><span class="linenos">434</span></a>
-</span><span id="Pathier-435"><a href="#Pathier-435"><span class="linenos">435</span></a><span class="sd">        `new_path`: The copy destination.</span>
-</span><span id="Pathier-436"><a href="#Pathier-436"><span class="linenos">436</span></a>
-</span><span id="Pathier-437"><a href="#Pathier-437"><span class="linenos">437</span></a><span class="sd">        `overwrite`: If `True`, files already existing in `new_path` will be overwritten.</span>
-</span><span id="Pathier-438"><a href="#Pathier-438"><span class="linenos">438</span></a><span class="sd">        If `False`, only files that don&#39;t exist in `new_path` will be copied.&quot;&quot;&quot;</span>
-</span><span id="Pathier-439"><a href="#Pathier-439"><span class="linenos">439</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier-440"><a href="#Pathier-440"><span class="linenos">440</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-441"><a href="#Pathier-441"><span class="linenos">441</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-442"><a href="#Pathier-442"><span class="linenos">442</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-443"><a href="#Pathier-443"><span class="linenos">443</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-444"><a href="#Pathier-444"><span class="linenos">444</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
-</span><span id="Pathier-445"><a href="#Pathier-445"><span class="linenos">445</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Pathier-446"><a href="#Pathier-446"><span class="linenos">446</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="Pathier-447"><a href="#Pathier-447"><span class="linenos">447</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-448"><a href="#Pathier-448"><span class="linenos">448</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
-</span><span id="Pathier-449"><a href="#Pathier-449"><span class="linenos">449</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-450"><a href="#Pathier-450"><span class="linenos">450</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-451"><a href="#Pathier-451"><span class="linenos">451</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier-452"><a href="#Pathier-452"><span class="linenos">452</span></a>        <span class="k">return</span> <span class="n">new_path</span>
-</span><span id="Pathier-453"><a href="#Pathier-453"><span class="linenos">453</span></a>
-</span><span id="Pathier-454"><a href="#Pathier-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-455"><a href="#Pathier-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
-</span><span id="Pathier-456"><a href="#Pathier-456"><span class="linenos">456</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
-</span><span id="Pathier-457"><a href="#Pathier-457"><span class="linenos">457</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
+</span><span id="Pathier-345"><a href="#Pathier-345"><span class="linenos">345</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier-346"><a href="#Pathier-346"><span class="linenos">346</span></a>
+</span><span id="Pathier-347"><a href="#Pathier-347"><span class="linenos">347</span></a><span class="sd">        `keepend`: If `True`, line breaks will be included in returned strings.&quot;&quot;&quot;</span>
+</span><span id="Pathier-348"><a href="#Pathier-348"><span class="linenos">348</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="n">keepends</span><span class="p">)</span>
+</span><span id="Pathier-349"><a href="#Pathier-349"><span class="linenos">349</span></a>
+</span><span id="Pathier-350"><a href="#Pathier-350"><span class="linenos">350</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-351"><a href="#Pathier-351"><span class="linenos">351</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-352"><a href="#Pathier-352"><span class="linenos">352</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+</span><span id="Pathier-353"><a href="#Pathier-353"><span class="linenos">353</span></a>
+</span><span id="Pathier-354"><a href="#Pathier-354"><span class="linenos">354</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier-355"><a href="#Pathier-355"><span class="linenos">355</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-356"><a href="#Pathier-356"><span class="linenos">356</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-357"><a href="#Pathier-357"><span class="linenos">357</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-358"><a href="#Pathier-358"><span class="linenos">358</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-359"><a href="#Pathier-359"><span class="linenos">359</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-360"><a href="#Pathier-360"><span class="linenos">360</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-361"><a href="#Pathier-361"><span class="linenos">361</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-362"><a href="#Pathier-362"><span class="linenos">362</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-363"><a href="#Pathier-363"><span class="linenos">363</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-364"><a href="#Pathier-364"><span class="linenos">364</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-365"><a href="#Pathier-365"><span class="linenos">365</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-366"><a href="#Pathier-366"><span class="linenos">366</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier-367"><a href="#Pathier-367"><span class="linenos">367</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
+</span><span id="Pathier-368"><a href="#Pathier-368"><span class="linenos">368</span></a>            <span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier-369"><a href="#Pathier-369"><span class="linenos">369</span></a>            <span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier-370"><a href="#Pathier-370"><span class="linenos">370</span></a>            <span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier-371"><a href="#Pathier-371"><span class="linenos">371</span></a>            <span class="n">parents</span><span class="p">,</span>
+</span><span id="Pathier-372"><a href="#Pathier-372"><span class="linenos">372</span></a>        <span class="p">)</span>
+</span><span id="Pathier-373"><a href="#Pathier-373"><span class="linenos">373</span></a>
+</span><span id="Pathier-374"><a href="#Pathier-374"><span class="linenos">374</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-375"><a href="#Pathier-375"><span class="linenos">375</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-376"><a href="#Pathier-376"><span class="linenos">376</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span><span class="o">.</span><span class="n">unwrap</span><span class="p">()</span>
+</span><span id="Pathier-377"><a href="#Pathier-377"><span class="linenos">377</span></a>
+</span><span id="Pathier-378"><a href="#Pathier-378"><span class="linenos">378</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
+</span><span id="Pathier-379"><a href="#Pathier-379"><span class="linenos">379</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-380"><a href="#Pathier-380"><span class="linenos">380</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-381"><a href="#Pathier-381"><span class="linenos">381</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-382"><a href="#Pathier-382"><span class="linenos">382</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-383"><a href="#Pathier-383"><span class="linenos">383</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-384"><a href="#Pathier-384"><span class="linenos">384</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-385"><a href="#Pathier-385"><span class="linenos">385</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-386"><a href="#Pathier-386"><span class="linenos">386</span></a>    <span class="p">):</span>
+</span><span id="Pathier-387"><a href="#Pathier-387"><span class="linenos">387</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-388"><a href="#Pathier-388"><span class="linenos">388</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier-389"><a href="#Pathier-389"><span class="linenos">389</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier-390"><a href="#Pathier-390"><span class="linenos">390</span></a>        <span class="p">)</span>
+</span><span id="Pathier-391"><a href="#Pathier-391"><span class="linenos">391</span></a>
+</span><span id="Pathier-392"><a href="#Pathier-392"><span class="linenos">392</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-393"><a href="#Pathier-393"><span class="linenos">393</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier-394"><a href="#Pathier-394"><span class="linenos">394</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier-395"><a href="#Pathier-395"><span class="linenos">395</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier-396"><a href="#Pathier-396"><span class="linenos">396</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier-397"><a href="#Pathier-397"><span class="linenos">397</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier-398"><a href="#Pathier-398"><span class="linenos">398</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier-399"><a href="#Pathier-399"><span class="linenos">399</span></a>
+</span><span id="Pathier-400"><a href="#Pathier-400"><span class="linenos">400</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
+</span><span id="Pathier-401"><a href="#Pathier-401"><span class="linenos">401</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-402"><a href="#Pathier-402"><span class="linenos">402</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-403"><a href="#Pathier-403"><span class="linenos">403</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-404"><a href="#Pathier-404"><span class="linenos">404</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-405"><a href="#Pathier-405"><span class="linenos">405</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-406"><a href="#Pathier-406"><span class="linenos">406</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-407"><a href="#Pathier-407"><span class="linenos">407</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-408"><a href="#Pathier-408"><span class="linenos">408</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-409"><a href="#Pathier-409"><span class="linenos">409</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-410"><a href="#Pathier-410"><span class="linenos">410</span></a>    <span class="p">):</span>
+</span><span id="Pathier-411"><a href="#Pathier-411"><span class="linenos">411</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier-412"><a href="#Pathier-412"><span class="linenos">412</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier-413"><a href="#Pathier-413"><span class="linenos">413</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier-414"><a href="#Pathier-414"><span class="linenos">414</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier-415"><a href="#Pathier-415"><span class="linenos">415</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier-416"><a href="#Pathier-416"><span class="linenos">416</span></a>                <span class="p">)</span>
+</span><span id="Pathier-417"><a href="#Pathier-417"><span class="linenos">417</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier-418"><a href="#Pathier-418"><span class="linenos">418</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
+</span><span id="Pathier-419"><a href="#Pathier-419"><span class="linenos">419</span></a>
+</span><span id="Pathier-420"><a href="#Pathier-420"><span class="linenos">420</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-421"><a href="#Pathier-421"><span class="linenos">421</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
+</span><span id="Pathier-422"><a href="#Pathier-422"><span class="linenos">422</span></a>
+</span><span id="Pathier-423"><a href="#Pathier-423"><span class="linenos">423</span></a><span class="sd">        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-424"><a href="#Pathier-424"><span class="linenos">424</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-425"><a href="#Pathier-425"><span class="linenos">425</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
+</span><span id="Pathier-426"><a href="#Pathier-426"><span class="linenos">426</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-427"><a href="#Pathier-427"><span class="linenos">427</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-428"><a href="#Pathier-428"><span class="linenos">428</span></a>
+</span><span id="Pathier-429"><a href="#Pathier-429"><span class="linenos">429</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
+</span><span id="Pathier-430"><a href="#Pathier-430"><span class="linenos">430</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Pathier-431"><a href="#Pathier-431"><span class="linenos">431</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-432"><a href="#Pathier-432"><span class="linenos">432</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
+</span><span id="Pathier-433"><a href="#Pathier-433"><span class="linenos">433</span></a><span class="sd">        to the instance pointed to by `new_path` using `shutil.copyfile`</span>
+</span><span id="Pathier-434"><a href="#Pathier-434"><span class="linenos">434</span></a><span class="sd">        or `shutil.copytree`.</span>
+</span><span id="Pathier-435"><a href="#Pathier-435"><span class="linenos">435</span></a>
+</span><span id="Pathier-436"><a href="#Pathier-436"><span class="linenos">436</span></a><span class="sd">        Returns the new path.</span>
+</span><span id="Pathier-437"><a href="#Pathier-437"><span class="linenos">437</span></a>
+</span><span id="Pathier-438"><a href="#Pathier-438"><span class="linenos">438</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-439"><a href="#Pathier-439"><span class="linenos">439</span></a>
+</span><span id="Pathier-440"><a href="#Pathier-440"><span class="linenos">440</span></a><span class="sd">        `new_path`: The copy destination.</span>
+</span><span id="Pathier-441"><a href="#Pathier-441"><span class="linenos">441</span></a>
+</span><span id="Pathier-442"><a href="#Pathier-442"><span class="linenos">442</span></a><span class="sd">        `overwrite`: If `True`, files already existing in `new_path` will be overwritten.</span>
+</span><span id="Pathier-443"><a href="#Pathier-443"><span class="linenos">443</span></a><span class="sd">        If `False`, only files that don&#39;t exist in `new_path` will be copied.&quot;&quot;&quot;</span>
+</span><span id="Pathier-444"><a href="#Pathier-444"><span class="linenos">444</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier-445"><a href="#Pathier-445"><span class="linenos">445</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-446"><a href="#Pathier-446"><span class="linenos">446</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-447"><a href="#Pathier-447"><span class="linenos">447</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-448"><a href="#Pathier-448"><span class="linenos">448</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-449"><a href="#Pathier-449"><span class="linenos">449</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
+</span><span id="Pathier-450"><a href="#Pathier-450"><span class="linenos">450</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Pathier-451"><a href="#Pathier-451"><span class="linenos">451</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="Pathier-452"><a href="#Pathier-452"><span class="linenos">452</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-453"><a href="#Pathier-453"><span class="linenos">453</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
+</span><span id="Pathier-454"><a href="#Pathier-454"><span class="linenos">454</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-455"><a href="#Pathier-455"><span class="linenos">455</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-456"><a href="#Pathier-456"><span class="linenos">456</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier-457"><a href="#Pathier-457"><span class="linenos">457</span></a>        <span class="k">return</span> <span class="n">new_path</span>
 </span><span id="Pathier-458"><a href="#Pathier-458"><span class="linenos">458</span></a>
-</span><span id="Pathier-459"><a href="#Pathier-459"><span class="linenos">459</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier-460"><a href="#Pathier-460"><span class="linenos">460</span></a>
-</span><span id="Pathier-461"><a href="#Pathier-461"><span class="linenos">461</span></a><span class="sd">        `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
-</span><span id="Pathier-462"><a href="#Pathier-462"><span class="linenos">462</span></a>
-</span><span id="Pathier-463"><a href="#Pathier-463"><span class="linenos">463</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
-</span><span id="Pathier-464"><a href="#Pathier-464"><span class="linenos">464</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
-</span><span id="Pathier-465"><a href="#Pathier-465"><span class="linenos">465</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier-466"><a href="#Pathier-466"><span class="linenos">466</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
-</span><span id="Pathier-467"><a href="#Pathier-467"><span class="linenos">467</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
-</span><span id="Pathier-468"><a href="#Pathier-468"><span class="linenos">468</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier-469"><a href="#Pathier-469"><span class="linenos">469</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
-</span><span id="Pathier-470"><a href="#Pathier-470"><span class="linenos">470</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-471"><a href="#Pathier-471"><span class="linenos">471</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-472"><a href="#Pathier-472"><span class="linenos">472</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
-</span><span id="Pathier-473"><a href="#Pathier-473"><span class="linenos">473</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
-</span><span id="Pathier-474"><a href="#Pathier-474"><span class="linenos">474</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Pathier-475"><a href="#Pathier-475"><span class="linenos">475</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
-</span><span id="Pathier-476"><a href="#Pathier-476"><span class="linenos">476</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-477"><a href="#Pathier-477"><span class="linenos">477</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
-</span><span id="Pathier-478"><a href="#Pathier-478"><span class="linenos">478</span></a>
-</span><span id="Pathier-479"><a href="#Pathier-479"><span class="linenos">479</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Pathier-480"><a href="#Pathier-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Make a call to `os.system` using the path pointed to by this Pathier object.</span>
-</span><span id="Pathier-481"><a href="#Pathier-481"><span class="linenos">481</span></a>
-</span><span id="Pathier-482"><a href="#Pathier-482"><span class="linenos">482</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-459"><a href="#Pathier-459"><span class="linenos">459</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-460"><a href="#Pathier-460"><span class="linenos">460</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
+</span><span id="Pathier-461"><a href="#Pathier-461"><span class="linenos">461</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
+</span><span id="Pathier-462"><a href="#Pathier-462"><span class="linenos">462</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
+</span><span id="Pathier-463"><a href="#Pathier-463"><span class="linenos">463</span></a>
+</span><span id="Pathier-464"><a href="#Pathier-464"><span class="linenos">464</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-465"><a href="#Pathier-465"><span class="linenos">465</span></a>
+</span><span id="Pathier-466"><a href="#Pathier-466"><span class="linenos">466</span></a><span class="sd">        `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
+</span><span id="Pathier-467"><a href="#Pathier-467"><span class="linenos">467</span></a>
+</span><span id="Pathier-468"><a href="#Pathier-468"><span class="linenos">468</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
+</span><span id="Pathier-469"><a href="#Pathier-469"><span class="linenos">469</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
+</span><span id="Pathier-470"><a href="#Pathier-470"><span class="linenos">470</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier-471"><a href="#Pathier-471"><span class="linenos">471</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
+</span><span id="Pathier-472"><a href="#Pathier-472"><span class="linenos">472</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
+</span><span id="Pathier-473"><a href="#Pathier-473"><span class="linenos">473</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier-474"><a href="#Pathier-474"><span class="linenos">474</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
+</span><span id="Pathier-475"><a href="#Pathier-475"><span class="linenos">475</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-476"><a href="#Pathier-476"><span class="linenos">476</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-477"><a href="#Pathier-477"><span class="linenos">477</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
+</span><span id="Pathier-478"><a href="#Pathier-478"><span class="linenos">478</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
+</span><span id="Pathier-479"><a href="#Pathier-479"><span class="linenos">479</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Pathier-480"><a href="#Pathier-480"><span class="linenos">480</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
+</span><span id="Pathier-481"><a href="#Pathier-481"><span class="linenos">481</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-482"><a href="#Pathier-482"><span class="linenos">482</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
 </span><span id="Pathier-483"><a href="#Pathier-483"><span class="linenos">483</span></a>
-</span><span id="Pathier-484"><a href="#Pathier-484"><span class="linenos">484</span></a><span class="sd">        `command`: Program/command to precede the path with.</span>
-</span><span id="Pathier-485"><a href="#Pathier-485"><span class="linenos">485</span></a>
-</span><span id="Pathier-486"><a href="#Pathier-486"><span class="linenos">486</span></a><span class="sd">        `args`: Any arguments that should come after the path.</span>
-</span><span id="Pathier-487"><a href="#Pathier-487"><span class="linenos">487</span></a>
-</span><span id="Pathier-488"><a href="#Pathier-488"><span class="linenos">488</span></a><span class="sd">        :returns: The integer output of `os.system`.</span>
-</span><span id="Pathier-489"><a href="#Pathier-489"><span class="linenos">489</span></a>
-</span><span id="Pathier-490"><a href="#Pathier-490"><span class="linenos">490</span></a><span class="sd">        e.g.</span>
-</span><span id="Pathier-491"><a href="#Pathier-491"><span class="linenos">491</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;mydirectory&quot;) / &quot;myscript.py&quot;</span>
-</span><span id="Pathier-492"><a href="#Pathier-492"><span class="linenos">492</span></a><span class="sd">        then</span>
-</span><span id="Pathier-493"><a href="#Pathier-493"><span class="linenos">493</span></a><span class="sd">        &gt;&gt;&gt; path.execute(&quot;py&quot;, &quot;--iterations 10&quot;)</span>
-</span><span id="Pathier-494"><a href="#Pathier-494"><span class="linenos">494</span></a><span class="sd">        equivalent to</span>
-</span><span id="Pathier-495"><a href="#Pathier-495"><span class="linenos">495</span></a><span class="sd">        &gt;&gt;&gt; os.system(f&quot;py {path} --iterations 10&quot;)&quot;&quot;&quot;</span>
-</span><span id="Pathier-496"><a href="#Pathier-496"><span class="linenos">496</span></a>        <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-484"><a href="#Pathier-484"><span class="linenos">484</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Pathier-485"><a href="#Pathier-485"><span class="linenos">485</span></a>        <span class="sd">&quot;&quot;&quot;Make a call to `os.system` using the path pointed to by this Pathier object.</span>
+</span><span id="Pathier-486"><a href="#Pathier-486"><span class="linenos">486</span></a>
+</span><span id="Pathier-487"><a href="#Pathier-487"><span class="linenos">487</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-488"><a href="#Pathier-488"><span class="linenos">488</span></a>
+</span><span id="Pathier-489"><a href="#Pathier-489"><span class="linenos">489</span></a><span class="sd">        `command`: Program/command to precede the path with.</span>
+</span><span id="Pathier-490"><a href="#Pathier-490"><span class="linenos">490</span></a>
+</span><span id="Pathier-491"><a href="#Pathier-491"><span class="linenos">491</span></a><span class="sd">        `args`: Any arguments that should come after the path.</span>
+</span><span id="Pathier-492"><a href="#Pathier-492"><span class="linenos">492</span></a>
+</span><span id="Pathier-493"><a href="#Pathier-493"><span class="linenos">493</span></a><span class="sd">        :returns: The integer output of `os.system`.</span>
+</span><span id="Pathier-494"><a href="#Pathier-494"><span class="linenos">494</span></a>
+</span><span id="Pathier-495"><a href="#Pathier-495"><span class="linenos">495</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier-496"><a href="#Pathier-496"><span class="linenos">496</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;mydirectory&quot;) / &quot;myscript.py&quot;</span>
+</span><span id="Pathier-497"><a href="#Pathier-497"><span class="linenos">497</span></a><span class="sd">        then</span>
+</span><span id="Pathier-498"><a href="#Pathier-498"><span class="linenos">498</span></a><span class="sd">        &gt;&gt;&gt; path.execute(&quot;py&quot;, &quot;--iterations 10&quot;)</span>
+</span><span id="Pathier-499"><a href="#Pathier-499"><span class="linenos">499</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier-500"><a href="#Pathier-500"><span class="linenos">500</span></a><span class="sd">        &gt;&gt;&gt; os.system(f&quot;py {path} --iterations 10&quot;)&quot;&quot;&quot;</span>
+</span><span id="Pathier-501"><a href="#Pathier-501"><span class="linenos">501</span></a>        <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclasses the standard library pathlib.Path class.</p>
 </div>
 
 
@@ -793,35 +801,48 @@
             <div class="docstring"><p>Returns the size in bytes of this file or directory.</p>
 
 <p>If this path doesn't exist, <code>0</code> will be returned.</p>
 </div>
 
 
                             </div>
+                            <div id="Pathier.formatted_size" class="classattr">
+                                <div class="attr variable">
+            <span class="name">formatted_size</span><span class="annotation">: str</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Pathier.formatted_size"></a>
+    
+            <div class="docstring"><p>The size of this file or directory formatted with <code>self.format_bytes()</code>.</p>
+</div>
+
+
+                            </div>
                             <div id="Pathier.format_bytes" class="classattr">
                                         <input id="Pathier.format_bytes-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
                     <div class="decorator">@staticmethod</div>
 
         <span class="def">def</span>
         <span class="name">format_bytes</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">size</span><span class="p">:</span> <span class="nb">int</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.format_bytes-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.format_bytes"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.format_bytes-102"><a href="#Pathier.format_bytes-102"><span class="linenos">102</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Pathier.format_bytes-103"><a href="#Pathier.format_bytes-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">format_bytes</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Pathier.format_bytes-104"><a href="#Pathier.format_bytes-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;Format `size` with common file size abbreviations and rounded to two decimal places.</span>
-</span><span id="Pathier.format_bytes-105"><a href="#Pathier.format_bytes-105"><span class="linenos">105</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier.format_bytes-106"><a href="#Pathier.format_bytes-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
-</span><span id="Pathier.format_bytes-107"><a href="#Pathier.format_bytes-107"><span class="linenos">107</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
-</span><span id="Pathier.format_bytes-108"><a href="#Pathier.format_bytes-108"><span class="linenos">108</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
-</span><span id="Pathier.format_bytes-109"><a href="#Pathier.format_bytes-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
-</span><span id="Pathier.format_bytes-110"><a href="#Pathier.format_bytes-110"><span class="linenos">110</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.format_bytes-107"><a href="#Pathier.format_bytes-107"><span class="linenos">107</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Pathier.format_bytes-108"><a href="#Pathier.format_bytes-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">format_bytes</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Pathier.format_bytes-109"><a href="#Pathier.format_bytes-109"><span class="linenos">109</span></a>        <span class="sd">&quot;&quot;&quot;Format `size` with common file size abbreviations and rounded to two decimal places.</span>
+</span><span id="Pathier.format_bytes-110"><a href="#Pathier.format_bytes-110"><span class="linenos">110</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier.format_bytes-111"><a href="#Pathier.format_bytes-111"><span class="linenos">111</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
+</span><span id="Pathier.format_bytes-112"><a href="#Pathier.format_bytes-112"><span class="linenos">112</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
+</span><span id="Pathier.format_bytes-113"><a href="#Pathier.format_bytes-113"><span class="linenos">113</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
+</span><span id="Pathier.format_bytes-114"><a href="#Pathier.format_bytes-114"><span class="linenos">114</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
+</span><span id="Pathier.format_bytes-115"><a href="#Pathier.format_bytes-115"><span class="linenos">115</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Format <code><a href="#Pathier.size">size</a></code> with common file size abbreviations and rounded to two decimal places.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="mi">1234</span> <span class="o">-&gt;</span> <span class="s2">&quot;1.23 kb&quot;</span>
@@ -838,17 +859,17 @@
         <span class="def">def</span>
         <span class="name">is_larger</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.is_larger-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.is_larger"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_larger-112"><a href="#Pathier.is_larger-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.is_larger-113"><a href="#Pathier.is_larger-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than the one pointed to by `path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier.is_larger-114"><a href="#Pathier.is_larger-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_larger-117"><a href="#Pathier.is_larger-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.is_larger-118"><a href="#Pathier.is_larger-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.is_larger-119"><a href="#Pathier.is_larger-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether this file or folder is larger than the one pointed to by <code>path</code>.</p>
 </div>
 
 
@@ -860,17 +881,17 @@
         <span class="def">def</span>
         <span class="name">is_older</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.is_older-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.is_older"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_older-116"><a href="#Pathier.is_older-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.is_older-117"><a href="#Pathier.is_older-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than the one pointed to by `path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier.is_older-118"><a href="#Pathier.is_older-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_older-121"><a href="#Pathier.is_older-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.is_older-122"><a href="#Pathier.is_older-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.is_older-123"><a href="#Pathier.is_older-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether this file or folder is older than the one pointed to by <code>path</code>.</p>
 </div>
 
 
@@ -882,17 +903,17 @@
         <span class="def">def</span>
         <span class="name">modified_more_recently</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.modified_more_recently-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.modified_more_recently"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.modified_more_recently-120"><a href="#Pathier.modified_more_recently-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.modified_more_recently-121"><a href="#Pathier.modified_more_recently-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified more recently than the one pointed to by `path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier.modified_more_recently-122"><a href="#Pathier.modified_more_recently-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.modified_more_recently-125"><a href="#Pathier.modified_more_recently-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.modified_more_recently-126"><a href="#Pathier.modified_more_recently-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified more recently than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.modified_more_recently-127"><a href="#Pathier.modified_more_recently-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns whether this file or folder was modified more recently than the one pointed to by <code>path</code>.</p>
 </div>
 
 
@@ -904,17 +925,17 @@
         <span class="def">def</span>
         <span class="name">mkcwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.mkcwd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.mkcwd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkcwd-125"><a href="#Pathier.mkcwd-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.mkcwd-126"><a href="#Pathier.mkcwd-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier.mkcwd-127"><a href="#Pathier.mkcwd-127"><span class="linenos">127</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkcwd-130"><a href="#Pathier.mkcwd-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.mkcwd-131"><a href="#Pathier.mkcwd-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier.mkcwd-132"><a href="#Pathier.mkcwd-132"><span class="linenos">132</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make this path your current working directory.</p>
 </div>
 
 
@@ -939,23 +960,23 @@
         <span class="def">def</span>
         <span class="name">add_to_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.add_to_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.add_to_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.add_to_PATH-134"><a href="#Pathier.add_to_PATH-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
-</span><span id="Pathier.add_to_PATH-135"><a href="#Pathier.add_to_PATH-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into `sys.path` if it isn&#39;t already there.</span>
-</span><span id="Pathier.add_to_PATH-136"><a href="#Pathier.add_to_PATH-136"><span class="linenos">136</span></a>
-</span><span id="Pathier.add_to_PATH-137"><a href="#Pathier.add_to_PATH-137"><span class="linenos">137</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.add_to_PATH-138"><a href="#Pathier.add_to_PATH-138"><span class="linenos">138</span></a>
-</span><span id="Pathier.add_to_PATH-139"><a href="#Pathier.add_to_PATH-139"><span class="linenos">139</span></a><span class="sd">        `index`: The index of `sys.path` to insert this path at.&quot;&quot;&quot;</span>
-</span><span id="Pathier.add_to_PATH-140"><a href="#Pathier.add_to_PATH-140"><span class="linenos">140</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier.add_to_PATH-141"><a href="#Pathier.add_to_PATH-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.add_to_PATH-142"><a href="#Pathier.add_to_PATH-142"><span class="linenos">142</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.add_to_PATH-139"><a href="#Pathier.add_to_PATH-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
+</span><span id="Pathier.add_to_PATH-140"><a href="#Pathier.add_to_PATH-140"><span class="linenos">140</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into `sys.path` if it isn&#39;t already there.</span>
+</span><span id="Pathier.add_to_PATH-141"><a href="#Pathier.add_to_PATH-141"><span class="linenos">141</span></a>
+</span><span id="Pathier.add_to_PATH-142"><a href="#Pathier.add_to_PATH-142"><span class="linenos">142</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.add_to_PATH-143"><a href="#Pathier.add_to_PATH-143"><span class="linenos">143</span></a>
+</span><span id="Pathier.add_to_PATH-144"><a href="#Pathier.add_to_PATH-144"><span class="linenos">144</span></a><span class="sd">        `index`: The index of `sys.path` to insert this path at.&quot;&quot;&quot;</span>
+</span><span id="Pathier.add_to_PATH-145"><a href="#Pathier.add_to_PATH-145"><span class="linenos">145</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier.add_to_PATH-146"><a href="#Pathier.add_to_PATH-146"><span class="linenos">146</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.add_to_PATH-147"><a href="#Pathier.add_to_PATH-147"><span class="linenos">147</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Insert this path into <code>sys.path</code> if it isn't already there.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -971,19 +992,19 @@
         <span class="def">def</span>
         <span class="name">append_to_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.append_to_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.append_to_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append_to_PATH-144"><a href="#Pathier.append_to_PATH-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.append_to_PATH-145"><a href="#Pathier.append_to_PATH-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to `sys.path` if it isn&#39;t already there.&quot;&quot;&quot;</span>
-</span><span id="Pathier.append_to_PATH-146"><a href="#Pathier.append_to_PATH-146"><span class="linenos">146</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier.append_to_PATH-147"><a href="#Pathier.append_to_PATH-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.append_to_PATH-148"><a href="#Pathier.append_to_PATH-148"><span class="linenos">148</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append_to_PATH-149"><a href="#Pathier.append_to_PATH-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.append_to_PATH-150"><a href="#Pathier.append_to_PATH-150"><span class="linenos">150</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to `sys.path` if it isn&#39;t already there.&quot;&quot;&quot;</span>
+</span><span id="Pathier.append_to_PATH-151"><a href="#Pathier.append_to_PATH-151"><span class="linenos">151</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier.append_to_PATH-152"><a href="#Pathier.append_to_PATH-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.append_to_PATH-153"><a href="#Pathier.append_to_PATH-153"><span class="linenos">153</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Append this path to <code>sys.path</code> if it isn't already there.</p>
 </div>
 
 
@@ -995,18 +1016,18 @@
         <span class="def">def</span>
         <span class="name">remove_from_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.remove_from_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.remove_from_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.remove_from_PATH-150"><a href="#Pathier.remove_from_PATH-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.remove_from_PATH-151"><a href="#Pathier.remove_from_PATH-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from `sys.path` if it&#39;s in `sys.path`.&quot;&quot;&quot;</span>
-</span><span id="Pathier.remove_from_PATH-152"><a href="#Pathier.remove_from_PATH-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.remove_from_PATH-153"><a href="#Pathier.remove_from_PATH-153"><span class="linenos">153</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.remove_from_PATH-155"><a href="#Pathier.remove_from_PATH-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.remove_from_PATH-156"><a href="#Pathier.remove_from_PATH-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from `sys.path` if it&#39;s in `sys.path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.remove_from_PATH-157"><a href="#Pathier.remove_from_PATH-157"><span class="linenos">157</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.remove_from_PATH-158"><a href="#Pathier.remove_from_PATH-158"><span class="linenos">158</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Remove this path from <code>sys.path</code> if it's in <code>sys.path</code>.</p>
 </div>
 
 
@@ -1018,26 +1039,26 @@
         <span class="def">def</span>
         <span class="name">moveup</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.moveup-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.moveup"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.moveup-155"><a href="#Pathier.moveup-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.moveup-156"><a href="#Pathier.moveup-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is a parent of this instance.</span>
-</span><span id="Pathier.moveup-157"><a href="#Pathier.moveup-157"><span class="linenos">157</span></a>
-</span><span id="Pathier.moveup-158"><a href="#Pathier.moveup-158"><span class="linenos">158</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
-</span><span id="Pathier.moveup-159"><a href="#Pathier.moveup-159"><span class="linenos">159</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier.moveup-160"><a href="#Pathier.moveup-160"><span class="linenos">160</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
-</span><span id="Pathier.moveup-161"><a href="#Pathier.moveup-161"><span class="linenos">161</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
-</span><span id="Pathier.moveup-162"><a href="#Pathier.moveup-162"><span class="linenos">162</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
-</span><span id="Pathier.moveup-163"><a href="#Pathier.moveup-163"><span class="linenos">163</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier.moveup-164"><a href="#Pathier.moveup-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.moveup-165"><a href="#Pathier.moveup-165"><span class="linenos">165</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.moveup-166"><a href="#Pathier.moveup-166"><span class="linenos">166</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.moveup-160"><a href="#Pathier.moveup-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.moveup-161"><a href="#Pathier.moveup-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is a parent of this instance.</span>
+</span><span id="Pathier.moveup-162"><a href="#Pathier.moveup-162"><span class="linenos">162</span></a>
+</span><span id="Pathier.moveup-163"><a href="#Pathier.moveup-163"><span class="linenos">163</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier.moveup-164"><a href="#Pathier.moveup-164"><span class="linenos">164</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier.moveup-165"><a href="#Pathier.moveup-165"><span class="linenos">165</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
+</span><span id="Pathier.moveup-166"><a href="#Pathier.moveup-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
+</span><span id="Pathier.moveup-167"><a href="#Pathier.moveup-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
+</span><span id="Pathier.moveup-168"><a href="#Pathier.moveup-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier.moveup-169"><a href="#Pathier.moveup-169"><span class="linenos">169</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.moveup-170"><a href="#Pathier.moveup-170"><span class="linenos">170</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.moveup-171"><a href="#Pathier.moveup-171"><span class="linenos">171</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a new <code><a href="#Pathier">Pathier</a></code> object that is a parent of this instance.</p>
 
 <p><code><a href="#Pathier.name">name</a></code> is case-sensitive and raises an exception if it isn't in <code>self.parts</code>.</p>
 
@@ -1060,24 +1081,24 @@
         <span class="def">def</span>
         <span class="name">move_under</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.move_under-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.move_under"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.move_under-179"><a href="#Pathier.move_under-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.move_under-180"><a href="#Pathier.move_under-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object such that the stem is one level below the given folder `name`.</span>
-</span><span id="Pathier.move_under-181"><a href="#Pathier.move_under-181"><span class="linenos">181</span></a>
-</span><span id="Pathier.move_under-182"><a href="#Pathier.move_under-182"><span class="linenos">182</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
-</span><span id="Pathier.move_under-183"><a href="#Pathier.move_under-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier.move_under-184"><a href="#Pathier.move_under-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
-</span><span id="Pathier.move_under-185"><a href="#Pathier.move_under-185"><span class="linenos">185</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier.move_under-186"><a href="#Pathier.move_under-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.move_under-187"><a href="#Pathier.move_under-187"><span class="linenos">187</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.move_under-188"><a href="#Pathier.move_under-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.move_under-184"><a href="#Pathier.move_under-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.move_under-185"><a href="#Pathier.move_under-185"><span class="linenos">185</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object such that the stem is one level below the given folder `name`.</span>
+</span><span id="Pathier.move_under-186"><a href="#Pathier.move_under-186"><span class="linenos">186</span></a>
+</span><span id="Pathier.move_under-187"><a href="#Pathier.move_under-187"><span class="linenos">187</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier.move_under-188"><a href="#Pathier.move_under-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier.move_under-189"><a href="#Pathier.move_under-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
+</span><span id="Pathier.move_under-190"><a href="#Pathier.move_under-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier.move_under-191"><a href="#Pathier.move_under-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.move_under-192"><a href="#Pathier.move_under-192"><span class="linenos">192</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.move_under-193"><a href="#Pathier.move_under-193"><span class="linenos">193</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a new <code><a href="#Pathier">Pathier</a></code> object such that the stem is one level below the given folder <code><a href="#Pathier.name">name</a></code>.</p>
 
 <p><code><a href="#Pathier.name">name</a></code> is case-sensitive and raises an exception if it isn't in <code>self.parts</code>.</p>
 
@@ -1098,32 +1119,32 @@
         <span class="def">def</span>
         <span class="name">separate</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.separate-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.separate"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.separate-190"><a href="#Pathier.separate-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.separate-191"><a href="#Pathier.separate-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is the relative child path after `name`.</span>
-</span><span id="Pathier.separate-192"><a href="#Pathier.separate-192"><span class="linenos">192</span></a>
-</span><span id="Pathier.separate-193"><a href="#Pathier.separate-193"><span class="linenos">193</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
-</span><span id="Pathier.separate-194"><a href="#Pathier.separate-194"><span class="linenos">194</span></a>
-</span><span id="Pathier.separate-195"><a href="#Pathier.separate-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.separate-196"><a href="#Pathier.separate-196"><span class="linenos">196</span></a>
-</span><span id="Pathier.separate-197"><a href="#Pathier.separate-197"><span class="linenos">197</span></a><span class="sd">        `keep_name`: If `True`, the returned path will start with `name`.</span>
-</span><span id="Pathier.separate-198"><a href="#Pathier.separate-198"><span class="linenos">198</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier.separate-199"><a href="#Pathier.separate-199"><span class="linenos">199</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
-</span><span id="Pathier.separate-200"><a href="#Pathier.separate-200"><span class="linenos">200</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
-</span><span id="Pathier.separate-201"><a href="#Pathier.separate-201"><span class="linenos">201</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
-</span><span id="Pathier.separate-202"><a href="#Pathier.separate-202"><span class="linenos">202</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier.separate-203"><a href="#Pathier.separate-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.separate-204"><a href="#Pathier.separate-204"><span class="linenos">204</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.separate-205"><a href="#Pathier.separate-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
-</span><span id="Pathier.separate-206"><a href="#Pathier.separate-206"><span class="linenos">206</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
-</span><span id="Pathier.separate-207"><a href="#Pathier.separate-207"><span class="linenos">207</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.separate-195"><a href="#Pathier.separate-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.separate-196"><a href="#Pathier.separate-196"><span class="linenos">196</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is the relative child path after `name`.</span>
+</span><span id="Pathier.separate-197"><a href="#Pathier.separate-197"><span class="linenos">197</span></a>
+</span><span id="Pathier.separate-198"><a href="#Pathier.separate-198"><span class="linenos">198</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier.separate-199"><a href="#Pathier.separate-199"><span class="linenos">199</span></a>
+</span><span id="Pathier.separate-200"><a href="#Pathier.separate-200"><span class="linenos">200</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.separate-201"><a href="#Pathier.separate-201"><span class="linenos">201</span></a>
+</span><span id="Pathier.separate-202"><a href="#Pathier.separate-202"><span class="linenos">202</span></a><span class="sd">        `keep_name`: If `True`, the returned path will start with `name`.</span>
+</span><span id="Pathier.separate-203"><a href="#Pathier.separate-203"><span class="linenos">203</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier.separate-204"><a href="#Pathier.separate-204"><span class="linenos">204</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
+</span><span id="Pathier.separate-205"><a href="#Pathier.separate-205"><span class="linenos">205</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
+</span><span id="Pathier.separate-206"><a href="#Pathier.separate-206"><span class="linenos">206</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
+</span><span id="Pathier.separate-207"><a href="#Pathier.separate-207"><span class="linenos">207</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier.separate-208"><a href="#Pathier.separate-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.separate-209"><a href="#Pathier.separate-209"><span class="linenos">209</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.separate-210"><a href="#Pathier.separate-210"><span class="linenos">210</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
+</span><span id="Pathier.separate-211"><a href="#Pathier.separate-211"><span class="linenos">211</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
+</span><span id="Pathier.separate-212"><a href="#Pathier.separate-212"><span class="linenos">212</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a new <code><a href="#Pathier">Pathier</a></code> object that is the relative child path after <code><a href="#Pathier.name">name</a></code>.</p>
 
 <p><code><a href="#Pathier.name">name</a></code> is case-sensitive and raises an exception if it isn't in <code>self.parts</code>.</p>
 
@@ -1150,19 +1171,19 @@
         <span class="def">def</span>
         <span class="name">mkdir</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span>, </span><span class="param"><span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>, </span><span class="param"><span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.mkdir-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.mkdir"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkdir-210"><a href="#Pathier.mkdir-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.mkdir-211"><a href="#Pathier.mkdir-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
-</span><span id="Pathier.mkdir-212"><a href="#Pathier.mkdir-212"><span class="linenos">212</span></a>
-</span><span id="Pathier.mkdir-213"><a href="#Pathier.mkdir-213"><span class="linenos">213</span></a><span class="sd">        Same as `Path().mkdir()` except `parents` and `exist_ok` default to `True` instead of `False`.&quot;&quot;&quot;</span>
-</span><span id="Pathier.mkdir-214"><a href="#Pathier.mkdir-214"><span class="linenos">214</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkdir-215"><a href="#Pathier.mkdir-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.mkdir-216"><a href="#Pathier.mkdir-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
+</span><span id="Pathier.mkdir-217"><a href="#Pathier.mkdir-217"><span class="linenos">217</span></a>
+</span><span id="Pathier.mkdir-218"><a href="#Pathier.mkdir-218"><span class="linenos">218</span></a><span class="sd">        Same as `Path().mkdir()` except `parents` and `exist_ok` default to `True` instead of `False`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.mkdir-219"><a href="#Pathier.mkdir-219"><span class="linenos">219</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create this directory.</p>
 
 <p>Same as <code>Path().mkdir()</code> except <code><a href="#Pathier.parents">parents</a></code> and <code>exist_ok</code> default to <code>True</code> instead of <code>False</code>.</p>
 </div>
@@ -1176,18 +1197,18 @@
         <span class="def">def</span>
         <span class="name">touch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.touch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.touch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.touch-216"><a href="#Pathier.touch-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.touch-217"><a href="#Pathier.touch-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Create file (and parents if necessary).&quot;&quot;&quot;</span>
-</span><span id="Pathier.touch-218"><a href="#Pathier.touch-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="Pathier.touch-219"><a href="#Pathier.touch-219"><span class="linenos">219</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.touch-221"><a href="#Pathier.touch-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.touch-222"><a href="#Pathier.touch-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;Create file (and parents if necessary).&quot;&quot;&quot;</span>
+</span><span id="Pathier.touch-223"><a href="#Pathier.touch-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="Pathier.touch-224"><a href="#Pathier.touch-224"><span class="linenos">224</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create file (and parents if necessary).</p>
 </div>
 
 
@@ -1199,23 +1220,23 @@
         <span class="def">def</span>
         <span class="name">open</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">mode</span><span class="o">=</span><span class="s1">&#39;r&#39;</span>,</span><span class="param">	<span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span>,</span><span class="param">	<span class="n">encoding</span><span class="o">=</span><span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="o">=</span><span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="o">=</span><span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.open-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.open"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.open-221"><a href="#Pathier.open-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s2">&quot;r&quot;</span><span class="p">,</span> <span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">newline</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
-</span><span id="Pathier.open-222"><a href="#Pathier.open-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Pathier.open-223"><a href="#Pathier.open-223"><span class="linenos">223</span></a><span class="sd">        Open the file pointed by this path and return a file object, as</span>
-</span><span id="Pathier.open-224"><a href="#Pathier.open-224"><span class="linenos">224</span></a><span class="sd">        the built-in open() function does.</span>
-</span><span id="Pathier.open-225"><a href="#Pathier.open-225"><span class="linenos">225</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Pathier.open-226"><a href="#Pathier.open-226"><span class="linenos">226</span></a>        <span class="n">stream</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">buffering</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">)</span>
-</span><span id="Pathier.open-227"><a href="#Pathier.open-227"><span class="linenos">227</span></a>        <span class="k">if</span> <span class="s2">&quot;r&quot;</span> <span class="ow">in</span> <span class="n">mode</span><span class="p">:</span>
-</span><span id="Pathier.open-228"><a href="#Pathier.open-228"><span class="linenos">228</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
-</span><span id="Pathier.open-229"><a href="#Pathier.open-229"><span class="linenos">229</span></a>        <span class="k">return</span> <span class="n">stream</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.open-226"><a href="#Pathier.open-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s2">&quot;r&quot;</span><span class="p">,</span> <span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">newline</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier.open-227"><a href="#Pathier.open-227"><span class="linenos">227</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Pathier.open-228"><a href="#Pathier.open-228"><span class="linenos">228</span></a><span class="sd">        Open the file pointed by this path and return a file object, as</span>
+</span><span id="Pathier.open-229"><a href="#Pathier.open-229"><span class="linenos">229</span></a><span class="sd">        the built-in open() function does.</span>
+</span><span id="Pathier.open-230"><a href="#Pathier.open-230"><span class="linenos">230</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Pathier.open-231"><a href="#Pathier.open-231"><span class="linenos">231</span></a>        <span class="n">stream</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">buffering</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">)</span>
+</span><span id="Pathier.open-232"><a href="#Pathier.open-232"><span class="linenos">232</span></a>        <span class="k">if</span> <span class="s2">&quot;r&quot;</span> <span class="ow">in</span> <span class="n">mode</span><span class="p">:</span>
+</span><span id="Pathier.open-233"><a href="#Pathier.open-233"><span class="linenos">233</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Pathier.open-234"><a href="#Pathier.open-234"><span class="linenos">234</span></a>        <span class="k">return</span> <span class="n">stream</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Open the file pointed by this path and return a file object, as
 the built-in open() function does.</p>
 </div>
 
@@ -1228,46 +1249,46 @@
         <span class="def">def</span>
         <span class="name">write_text</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.write_text-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.write_text"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_text-231"><a href="#Pathier.write_text-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
-</span><span id="Pathier.write_text-232"><a href="#Pathier.write_text-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.write_text-233"><a href="#Pathier.write_text-233"><span class="linenos">233</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.write_text-234"><a href="#Pathier.write_text-234"><span class="linenos">234</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-235"><a href="#Pathier.write_text-235"><span class="linenos">235</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-236"><a href="#Pathier.write_text-236"><span class="linenos">236</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-237"><a href="#Pathier.write_text-237"><span class="linenos">237</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.write_text-238"><a href="#Pathier.write_text-238"><span class="linenos">238</span></a>    <span class="p">):</span>
-</span><span id="Pathier.write_text-239"><a href="#Pathier.write_text-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file.</span>
-</span><span id="Pathier.write_text-240"><a href="#Pathier.write_text-240"><span class="linenos">240</span></a>
-</span><span id="Pathier.write_text-241"><a href="#Pathier.write_text-241"><span class="linenos">241</span></a><span class="sd">        If a `TypeError` is raised, the function  will attempt to cast `data` to a `str` and try the write again.</span>
-</span><span id="Pathier.write_text-242"><a href="#Pathier.write_text-242"><span class="linenos">242</span></a>
-</span><span id="Pathier.write_text-243"><a href="#Pathier.write_text-243"><span class="linenos">243</span></a><span class="sd">        If a `FileNotFoundError` is raised and `parents = True`, `self.parent` will be created.&quot;&quot;&quot;</span>
-</span><span id="Pathier.write_text-244"><a href="#Pathier.write_text-244"><span class="linenos">244</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
-</span><span id="Pathier.write_text-245"><a href="#Pathier.write_text-245"><span class="linenos">245</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
-</span><span id="Pathier.write_text-246"><a href="#Pathier.write_text-246"><span class="linenos">246</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier.write_text-247"><a href="#Pathier.write_text-247"><span class="linenos">247</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier.write_text-248"><a href="#Pathier.write_text-248"><span class="linenos">248</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier.write_text-249"><a href="#Pathier.write_text-249"><span class="linenos">249</span></a>        <span class="p">)</span>
-</span><span id="Pathier.write_text-250"><a href="#Pathier.write_text-250"><span class="linenos">250</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier.write_text-251"><a href="#Pathier.write_text-251"><span class="linenos">251</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-252"><a href="#Pathier.write_text-252"><span class="linenos">252</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
-</span><span id="Pathier.write_text-253"><a href="#Pathier.write_text-253"><span class="linenos">253</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-254"><a href="#Pathier.write_text-254"><span class="linenos">254</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-255"><a href="#Pathier.write_text-255"><span class="linenos">255</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier.write_text-256"><a href="#Pathier.write_text-256"><span class="linenos">256</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier.write_text-257"><a href="#Pathier.write_text-257"><span class="linenos">257</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.write_text-258"><a href="#Pathier.write_text-258"><span class="linenos">258</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-259"><a href="#Pathier.write_text-259"><span class="linenos">259</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.write_text-260"><a href="#Pathier.write_text-260"><span class="linenos">260</span></a>                <span class="k">raise</span>
-</span><span id="Pathier.write_text-261"><a href="#Pathier.write_text-261"><span class="linenos">261</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier.write_text-262"><a href="#Pathier.write_text-262"><span class="linenos">262</span></a>            <span class="k">raise</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_text-236"><a href="#Pathier.write_text-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
+</span><span id="Pathier.write_text-237"><a href="#Pathier.write_text-237"><span class="linenos">237</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.write_text-238"><a href="#Pathier.write_text-238"><span class="linenos">238</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.write_text-239"><a href="#Pathier.write_text-239"><span class="linenos">239</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-240"><a href="#Pathier.write_text-240"><span class="linenos">240</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-241"><a href="#Pathier.write_text-241"><span class="linenos">241</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-242"><a href="#Pathier.write_text-242"><span class="linenos">242</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.write_text-243"><a href="#Pathier.write_text-243"><span class="linenos">243</span></a>    <span class="p">):</span>
+</span><span id="Pathier.write_text-244"><a href="#Pathier.write_text-244"><span class="linenos">244</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file.</span>
+</span><span id="Pathier.write_text-245"><a href="#Pathier.write_text-245"><span class="linenos">245</span></a>
+</span><span id="Pathier.write_text-246"><a href="#Pathier.write_text-246"><span class="linenos">246</span></a><span class="sd">        If a `TypeError` is raised, the function  will attempt to cast `data` to a `str` and try the write again.</span>
+</span><span id="Pathier.write_text-247"><a href="#Pathier.write_text-247"><span class="linenos">247</span></a>
+</span><span id="Pathier.write_text-248"><a href="#Pathier.write_text-248"><span class="linenos">248</span></a><span class="sd">        If a `FileNotFoundError` is raised and `parents = True`, `self.parent` will be created.&quot;&quot;&quot;</span>
+</span><span id="Pathier.write_text-249"><a href="#Pathier.write_text-249"><span class="linenos">249</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
+</span><span id="Pathier.write_text-250"><a href="#Pathier.write_text-250"><span class="linenos">250</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
+</span><span id="Pathier.write_text-251"><a href="#Pathier.write_text-251"><span class="linenos">251</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier.write_text-252"><a href="#Pathier.write_text-252"><span class="linenos">252</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier.write_text-253"><a href="#Pathier.write_text-253"><span class="linenos">253</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier.write_text-254"><a href="#Pathier.write_text-254"><span class="linenos">254</span></a>        <span class="p">)</span>
+</span><span id="Pathier.write_text-255"><a href="#Pathier.write_text-255"><span class="linenos">255</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier.write_text-256"><a href="#Pathier.write_text-256"><span class="linenos">256</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-257"><a href="#Pathier.write_text-257"><span class="linenos">257</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
+</span><span id="Pathier.write_text-258"><a href="#Pathier.write_text-258"><span class="linenos">258</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-259"><a href="#Pathier.write_text-259"><span class="linenos">259</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-260"><a href="#Pathier.write_text-260"><span class="linenos">260</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier.write_text-261"><a href="#Pathier.write_text-261"><span class="linenos">261</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier.write_text-262"><a href="#Pathier.write_text-262"><span class="linenos">262</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.write_text-263"><a href="#Pathier.write_text-263"><span class="linenos">263</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-264"><a href="#Pathier.write_text-264"><span class="linenos">264</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.write_text-265"><a href="#Pathier.write_text-265"><span class="linenos">265</span></a>                <span class="k">raise</span>
+</span><span id="Pathier.write_text-266"><a href="#Pathier.write_text-266"><span class="linenos">266</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier.write_text-267"><a href="#Pathier.write_text-267"><span class="linenos">267</span></a>            <span class="k">raise</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Write data to file.</p>
 
 <p>If a <code>TypeError</code> is raised, the function  will attempt to cast <code>data</code> to a <code>str</code> and try the write again.</p>
 
@@ -1283,31 +1304,31 @@
         <span class="def">def</span>
         <span class="name">write_bytes</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span>, </span><span class="param"><span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.write_bytes-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.write_bytes"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_bytes-264"><a href="#Pathier.write_bytes-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.write_bytes-265"><a href="#Pathier.write_bytes-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
-</span><span id="Pathier.write_bytes-266"><a href="#Pathier.write_bytes-266"><span class="linenos">266</span></a>
-</span><span id="Pathier.write_bytes-267"><a href="#Pathier.write_bytes-267"><span class="linenos">267</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.write_bytes-268"><a href="#Pathier.write_bytes-268"><span class="linenos">268</span></a>
-</span><span id="Pathier.write_bytes-269"><a href="#Pathier.write_bytes-269"><span class="linenos">269</span></a><span class="sd">        `parents`: If `True` and the write operation fails with a `FileNotFoundError`,</span>
-</span><span id="Pathier.write_bytes-270"><a href="#Pathier.write_bytes-270"><span class="linenos">270</span></a><span class="sd">        make the parent directory and retry the write.&quot;&quot;&quot;</span>
-</span><span id="Pathier.write_bytes-271"><a href="#Pathier.write_bytes-271"><span class="linenos">271</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-272"><a href="#Pathier.write_bytes-272"><span class="linenos">272</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-273"><a href="#Pathier.write_bytes-273"><span class="linenos">273</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-274"><a href="#Pathier.write_bytes-274"><span class="linenos">274</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-275"><a href="#Pathier.write_bytes-275"><span class="linenos">275</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-276"><a href="#Pathier.write_bytes-276"><span class="linenos">276</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-277"><a href="#Pathier.write_bytes-277"><span class="linenos">277</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-278"><a href="#Pathier.write_bytes-278"><span class="linenos">278</span></a>                <span class="k">raise</span>
-</span><span id="Pathier.write_bytes-279"><a href="#Pathier.write_bytes-279"><span class="linenos">279</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-280"><a href="#Pathier.write_bytes-280"><span class="linenos">280</span></a>            <span class="k">raise</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_bytes-269"><a href="#Pathier.write_bytes-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.write_bytes-270"><a href="#Pathier.write_bytes-270"><span class="linenos">270</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
+</span><span id="Pathier.write_bytes-271"><a href="#Pathier.write_bytes-271"><span class="linenos">271</span></a>
+</span><span id="Pathier.write_bytes-272"><a href="#Pathier.write_bytes-272"><span class="linenos">272</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.write_bytes-273"><a href="#Pathier.write_bytes-273"><span class="linenos">273</span></a>
+</span><span id="Pathier.write_bytes-274"><a href="#Pathier.write_bytes-274"><span class="linenos">274</span></a><span class="sd">        `parents`: If `True` and the write operation fails with a `FileNotFoundError`,</span>
+</span><span id="Pathier.write_bytes-275"><a href="#Pathier.write_bytes-275"><span class="linenos">275</span></a><span class="sd">        make the parent directory and retry the write.&quot;&quot;&quot;</span>
+</span><span id="Pathier.write_bytes-276"><a href="#Pathier.write_bytes-276"><span class="linenos">276</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-277"><a href="#Pathier.write_bytes-277"><span class="linenos">277</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-278"><a href="#Pathier.write_bytes-278"><span class="linenos">278</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-279"><a href="#Pathier.write_bytes-279"><span class="linenos">279</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-280"><a href="#Pathier.write_bytes-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-281"><a href="#Pathier.write_bytes-281"><span class="linenos">281</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-282"><a href="#Pathier.write_bytes-282"><span class="linenos">282</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-283"><a href="#Pathier.write_bytes-283"><span class="linenos">283</span></a>                <span class="k">raise</span>
+</span><span id="Pathier.write_bytes-284"><a href="#Pathier.write_bytes-284"><span class="linenos">284</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-285"><a href="#Pathier.write_bytes-285"><span class="linenos">285</span></a>            <span class="k">raise</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Write bytes to file.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1324,26 +1345,26 @@
         <span class="def">def</span>
         <span class="name">append</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.append-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.append"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append-282"><a href="#Pathier.append-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">append</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="Pathier.append-283"><a href="#Pathier.append-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Append `data` to the file pointed to by this `Pathier` object.</span>
-</span><span id="Pathier.append-284"><a href="#Pathier.append-284"><span class="linenos">284</span></a>
-</span><span id="Pathier.append-285"><a href="#Pathier.append-285"><span class="linenos">285</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.append-286"><a href="#Pathier.append-286"><span class="linenos">286</span></a>
-</span><span id="Pathier.append-287"><a href="#Pathier.append-287"><span class="linenos">287</span></a><span class="sd">        `new_line`: If `True`, add `\\n` to `data`.</span>
-</span><span id="Pathier.append-288"><a href="#Pathier.append-288"><span class="linenos">288</span></a>
-</span><span id="Pathier.append-289"><a href="#Pathier.append-289"><span class="linenos">289</span></a><span class="sd">        `encoding`: The file encoding to use.&quot;&quot;&quot;</span>
-</span><span id="Pathier.append-290"><a href="#Pathier.append-290"><span class="linenos">290</span></a>        <span class="k">if</span> <span class="n">new_line</span><span class="p">:</span>
-</span><span id="Pathier.append-291"><a href="#Pathier.append-291"><span class="linenos">291</span></a>            <span class="n">data</span> <span class="o">+=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="Pathier.append-292"><a href="#Pathier.append-292"><span class="linenos">292</span></a>        <span class="k">with</span> <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;a&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
-</span><span id="Pathier.append-293"><a href="#Pathier.append-293"><span class="linenos">293</span></a>            <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append-287"><a href="#Pathier.append-287"><span class="linenos">287</span></a>    <span class="k">def</span> <span class="nf">append</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier.append-288"><a href="#Pathier.append-288"><span class="linenos">288</span></a>        <span class="sd">&quot;&quot;&quot;Append `data` to the file pointed to by this `Pathier` object.</span>
+</span><span id="Pathier.append-289"><a href="#Pathier.append-289"><span class="linenos">289</span></a>
+</span><span id="Pathier.append-290"><a href="#Pathier.append-290"><span class="linenos">290</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.append-291"><a href="#Pathier.append-291"><span class="linenos">291</span></a>
+</span><span id="Pathier.append-292"><a href="#Pathier.append-292"><span class="linenos">292</span></a><span class="sd">        `new_line`: If `True`, add `\\n` to `data`.</span>
+</span><span id="Pathier.append-293"><a href="#Pathier.append-293"><span class="linenos">293</span></a>
+</span><span id="Pathier.append-294"><a href="#Pathier.append-294"><span class="linenos">294</span></a><span class="sd">        `encoding`: The file encoding to use.&quot;&quot;&quot;</span>
+</span><span id="Pathier.append-295"><a href="#Pathier.append-295"><span class="linenos">295</span></a>        <span class="k">if</span> <span class="n">new_line</span><span class="p">:</span>
+</span><span id="Pathier.append-296"><a href="#Pathier.append-296"><span class="linenos">296</span></a>            <span class="n">data</span> <span class="o">+=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="Pathier.append-297"><a href="#Pathier.append-297"><span class="linenos">297</span></a>        <span class="k">with</span> <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;a&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
+</span><span id="Pathier.append-298"><a href="#Pathier.append-298"><span class="linenos">298</span></a>            <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Append <code>data</code> to the file pointed to by this <code><a href="#Pathier">Pathier</a></code> object.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1361,39 +1382,39 @@
         <span class="def">def</span>
         <span class="name">replace</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]]</span>,</span><span class="param">	<span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.replace-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.replace"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.replace-295"><a href="#Pathier.replace-295"><span class="linenos">295</span></a>    <span class="k">def</span> <span class="nf">replace</span><span class="p">(</span>
-</span><span id="Pathier.replace-296"><a href="#Pathier.replace-296"><span class="linenos">296</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.replace-297"><a href="#Pathier.replace-297"><span class="linenos">297</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
-</span><span id="Pathier.replace-298"><a href="#Pathier.replace-298"><span class="linenos">298</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
-</span><span id="Pathier.replace-299"><a href="#Pathier.replace-299"><span class="linenos">299</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.replace-300"><a href="#Pathier.replace-300"><span class="linenos">300</span></a>    <span class="p">):</span>
-</span><span id="Pathier.replace-301"><a href="#Pathier.replace-301"><span class="linenos">301</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
-</span><span id="Pathier.replace-302"><a href="#Pathier.replace-302"><span class="linenos">302</span></a>
-</span><span id="Pathier.replace-303"><a href="#Pathier.replace-303"><span class="linenos">303</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.replace-304"><a href="#Pathier.replace-304"><span class="linenos">304</span></a>
-</span><span id="Pathier.replace-305"><a href="#Pathier.replace-305"><span class="linenos">305</span></a><span class="sd">        `count`: Only replace this many occurences of each pair.</span>
-</span><span id="Pathier.replace-306"><a href="#Pathier.replace-306"><span class="linenos">306</span></a><span class="sd">        By default (`-1`), all occurences are replaced.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.replace-300"><a href="#Pathier.replace-300"><span class="linenos">300</span></a>    <span class="k">def</span> <span class="nf">replace</span><span class="p">(</span>
+</span><span id="Pathier.replace-301"><a href="#Pathier.replace-301"><span class="linenos">301</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.replace-302"><a href="#Pathier.replace-302"><span class="linenos">302</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
+</span><span id="Pathier.replace-303"><a href="#Pathier.replace-303"><span class="linenos">303</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
+</span><span id="Pathier.replace-304"><a href="#Pathier.replace-304"><span class="linenos">304</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.replace-305"><a href="#Pathier.replace-305"><span class="linenos">305</span></a>    <span class="p">):</span>
+</span><span id="Pathier.replace-306"><a href="#Pathier.replace-306"><span class="linenos">306</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
 </span><span id="Pathier.replace-307"><a href="#Pathier.replace-307"><span class="linenos">307</span></a>
-</span><span id="Pathier.replace-308"><a href="#Pathier.replace-308"><span class="linenos">308</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier.replace-308"><a href="#Pathier.replace-308"><span class="linenos">308</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier.replace-309"><a href="#Pathier.replace-309"><span class="linenos">309</span></a>
-</span><span id="Pathier.replace-310"><a href="#Pathier.replace-310"><span class="linenos">310</span></a><span class="sd">        e.g.</span>
-</span><span id="Pathier.replace-311"><a href="#Pathier.replace-311"><span class="linenos">311</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;somefile.txt&quot;)</span>
-</span><span id="Pathier.replace-312"><a href="#Pathier.replace-312"><span class="linenos">312</span></a><span class="sd">        &gt;&gt;&gt;</span>
-</span><span id="Pathier.replace-313"><a href="#Pathier.replace-313"><span class="linenos">313</span></a><span class="sd">        &gt;&gt;&gt; path.replace([(&quot;hello&quot;, &quot;yeet&quot;), (&quot;goodbye&quot;, &quot;yeehaw&quot;)])</span>
-</span><span id="Pathier.replace-314"><a href="#Pathier.replace-314"><span class="linenos">314</span></a><span class="sd">        equivalent to</span>
-</span><span id="Pathier.replace-315"><a href="#Pathier.replace-315"><span class="linenos">315</span></a><span class="sd">        &gt;&gt;&gt; path.write_text(path.read_text().replace(&quot;hello&quot;, &quot;yeet&quot;).replace(&quot;goodbye&quot;, &quot;yeehaw&quot;))&quot;&quot;&quot;</span>
-</span><span id="Pathier.replace-316"><a href="#Pathier.replace-316"><span class="linenos">316</span></a>        <span class="n">text</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">)</span>
-</span><span id="Pathier.replace-317"><a href="#Pathier.replace-317"><span class="linenos">317</span></a>        <span class="k">for</span> <span class="n">sub</span> <span class="ow">in</span> <span class="n">substitutions</span><span class="p">:</span>
-</span><span id="Pathier.replace-318"><a href="#Pathier.replace-318"><span class="linenos">318</span></a>            <span class="n">text</span> <span class="o">=</span> <span class="n">text</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">sub</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">sub</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">count</span><span class="p">)</span>
-</span><span id="Pathier.replace-319"><a href="#Pathier.replace-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">text</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier.replace-310"><a href="#Pathier.replace-310"><span class="linenos">310</span></a><span class="sd">        `count`: Only replace this many occurences of each pair.</span>
+</span><span id="Pathier.replace-311"><a href="#Pathier.replace-311"><span class="linenos">311</span></a><span class="sd">        By default (`-1`), all occurences are replaced.</span>
+</span><span id="Pathier.replace-312"><a href="#Pathier.replace-312"><span class="linenos">312</span></a>
+</span><span id="Pathier.replace-313"><a href="#Pathier.replace-313"><span class="linenos">313</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier.replace-314"><a href="#Pathier.replace-314"><span class="linenos">314</span></a>
+</span><span id="Pathier.replace-315"><a href="#Pathier.replace-315"><span class="linenos">315</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier.replace-316"><a href="#Pathier.replace-316"><span class="linenos">316</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;somefile.txt&quot;)</span>
+</span><span id="Pathier.replace-317"><a href="#Pathier.replace-317"><span class="linenos">317</span></a><span class="sd">        &gt;&gt;&gt;</span>
+</span><span id="Pathier.replace-318"><a href="#Pathier.replace-318"><span class="linenos">318</span></a><span class="sd">        &gt;&gt;&gt; path.replace([(&quot;hello&quot;, &quot;yeet&quot;), (&quot;goodbye&quot;, &quot;yeehaw&quot;)])</span>
+</span><span id="Pathier.replace-319"><a href="#Pathier.replace-319"><span class="linenos">319</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier.replace-320"><a href="#Pathier.replace-320"><span class="linenos">320</span></a><span class="sd">        &gt;&gt;&gt; path.write_text(path.read_text().replace(&quot;hello&quot;, &quot;yeet&quot;).replace(&quot;goodbye&quot;, &quot;yeehaw&quot;))&quot;&quot;&quot;</span>
+</span><span id="Pathier.replace-321"><a href="#Pathier.replace-321"><span class="linenos">321</span></a>        <span class="n">text</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier.replace-322"><a href="#Pathier.replace-322"><span class="linenos">322</span></a>        <span class="k">for</span> <span class="n">sub</span> <span class="ow">in</span> <span class="n">substitutions</span><span class="p">:</span>
+</span><span id="Pathier.replace-323"><a href="#Pathier.replace-323"><span class="linenos">323</span></a>            <span class="n">text</span> <span class="o">=</span> <span class="n">text</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">sub</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">sub</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">count</span><span class="p">)</span>
+</span><span id="Pathier.replace-324"><a href="#Pathier.replace-324"><span class="linenos">324</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">text</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>For each pair in <code>substitutions</code>, replace the first string with the second string.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1423,25 +1444,25 @@
         <span class="def">def</span>
         <span class="name">join</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.join-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.join"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.join-321"><a href="#Pathier.join-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
-</span><span id="Pathier.join-322"><a href="#Pathier.join-322"><span class="linenos">322</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
-</span><span id="Pathier.join-323"><a href="#Pathier.join-323"><span class="linenos">323</span></a>
-</span><span id="Pathier.join-324"><a href="#Pathier.join-324"><span class="linenos">324</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
-</span><span id="Pathier.join-325"><a href="#Pathier.join-325"><span class="linenos">325</span></a>
-</span><span id="Pathier.join-326"><a href="#Pathier.join-326"><span class="linenos">326</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.join-327"><a href="#Pathier.join-327"><span class="linenos">327</span></a>
-</span><span id="Pathier.join-328"><a href="#Pathier.join-328"><span class="linenos">328</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
-</span><span id="Pathier.join-329"><a href="#Pathier.join-329"><span class="linenos">329</span></a>
-</span><span id="Pathier.join-330"><a href="#Pathier.join-330"><span class="linenos">330</span></a><span class="sd">        `sep`: The separator to use when joining `data`.&quot;&quot;&quot;</span>
-</span><span id="Pathier.join-331"><a href="#Pathier.join-331"><span class="linenos">331</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">sep</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">data</span><span class="p">),</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.join-326"><a href="#Pathier.join-326"><span class="linenos">326</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
+</span><span id="Pathier.join-327"><a href="#Pathier.join-327"><span class="linenos">327</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
+</span><span id="Pathier.join-328"><a href="#Pathier.join-328"><span class="linenos">328</span></a>
+</span><span id="Pathier.join-329"><a href="#Pathier.join-329"><span class="linenos">329</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
+</span><span id="Pathier.join-330"><a href="#Pathier.join-330"><span class="linenos">330</span></a>
+</span><span id="Pathier.join-331"><a href="#Pathier.join-331"><span class="linenos">331</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.join-332"><a href="#Pathier.join-332"><span class="linenos">332</span></a>
+</span><span id="Pathier.join-333"><a href="#Pathier.join-333"><span class="linenos">333</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier.join-334"><a href="#Pathier.join-334"><span class="linenos">334</span></a>
+</span><span id="Pathier.join-335"><a href="#Pathier.join-335"><span class="linenos">335</span></a><span class="sd">        `sep`: The separator to use when joining `data`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.join-336"><a href="#Pathier.join-336"><span class="linenos">336</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">sep</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">data</span><span class="p">),</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Write a list of strings, joined by <code>sep</code>, to the file pointed at by this instance.</p>
 
 <p>Equivalent to <code>Pathier("somefile.txt").write_text(sep.join(data), encoding=encoding)</code></p>
 
@@ -1461,25 +1482,25 @@
         <span class="def">def</span>
         <span class="name">split</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.split-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.split"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.split-333"><a href="#Pathier.split-333"><span class="linenos">333</span></a>    <span class="k">def</span> <span class="nf">split</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="Pathier.split-334"><a href="#Pathier.split-334"><span class="linenos">334</span></a>        <span class="sd">&quot;&quot;&quot;Returns the content of the pointed at file as a list of strings, splitting at new line characters.</span>
-</span><span id="Pathier.split-335"><a href="#Pathier.split-335"><span class="linenos">335</span></a>
-</span><span id="Pathier.split-336"><a href="#Pathier.split-336"><span class="linenos">336</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).read_text(encoding=encoding).splitlines()`</span>
-</span><span id="Pathier.split-337"><a href="#Pathier.split-337"><span class="linenos">337</span></a>
-</span><span id="Pathier.split-338"><a href="#Pathier.split-338"><span class="linenos">338</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.split-339"><a href="#Pathier.split-339"><span class="linenos">339</span></a>
-</span><span id="Pathier.split-340"><a href="#Pathier.split-340"><span class="linenos">340</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
-</span><span id="Pathier.split-341"><a href="#Pathier.split-341"><span class="linenos">341</span></a>
-</span><span id="Pathier.split-342"><a href="#Pathier.split-342"><span class="linenos">342</span></a><span class="sd">        `keepend`: If `True`, line breaks will be included in returned strings.&quot;&quot;&quot;</span>
-</span><span id="Pathier.split-343"><a href="#Pathier.split-343"><span class="linenos">343</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="n">keepends</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.split-338"><a href="#Pathier.split-338"><span class="linenos">338</span></a>    <span class="k">def</span> <span class="nf">split</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Pathier.split-339"><a href="#Pathier.split-339"><span class="linenos">339</span></a>        <span class="sd">&quot;&quot;&quot;Returns the content of the pointed at file as a list of strings, splitting at new line characters.</span>
+</span><span id="Pathier.split-340"><a href="#Pathier.split-340"><span class="linenos">340</span></a>
+</span><span id="Pathier.split-341"><a href="#Pathier.split-341"><span class="linenos">341</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).read_text(encoding=encoding).splitlines()`</span>
+</span><span id="Pathier.split-342"><a href="#Pathier.split-342"><span class="linenos">342</span></a>
+</span><span id="Pathier.split-343"><a href="#Pathier.split-343"><span class="linenos">343</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.split-344"><a href="#Pathier.split-344"><span class="linenos">344</span></a>
+</span><span id="Pathier.split-345"><a href="#Pathier.split-345"><span class="linenos">345</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier.split-346"><a href="#Pathier.split-346"><span class="linenos">346</span></a>
+</span><span id="Pathier.split-347"><a href="#Pathier.split-347"><span class="linenos">347</span></a><span class="sd">        `keepend`: If `True`, line breaks will be included in returned strings.&quot;&quot;&quot;</span>
+</span><span id="Pathier.split-348"><a href="#Pathier.split-348"><span class="linenos">348</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="n">keepends</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Returns the content of the pointed at file as a list of strings, splitting at new line characters.</p>
 
 <p>Equivalent to <code>Pathier("somefile.txt").read_text(encoding=encoding).splitlines()</code></p>
 
@@ -1499,17 +1520,17 @@
         <span class="def">def</span>
         <span class="name">json_loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.json_loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.json_loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_loads-345"><a href="#Pathier.json_loads-345"><span class="linenos">345</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.json_loads-346"><a href="#Pathier.json_loads-346"><span class="linenos">346</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.json_loads-347"><a href="#Pathier.json_loads-347"><span class="linenos">347</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_loads-350"><a href="#Pathier.json_loads-350"><span class="linenos">350</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.json_loads-351"><a href="#Pathier.json_loads-351"><span class="linenos">351</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.json_loads-352"><a href="#Pathier.json_loads-352"><span class="linenos">352</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load json file.</p>
 </div>
 
 
@@ -1521,33 +1542,33 @@
         <span class="def">def</span>
         <span class="name">json_dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">indent</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">default</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.json_dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.json_dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_dumps-349"><a href="#Pathier.json_dumps-349"><span class="linenos">349</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier.json_dumps-350"><a href="#Pathier.json_dumps-350"><span class="linenos">350</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-351"><a href="#Pathier.json_dumps-351"><span class="linenos">351</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-352"><a href="#Pathier.json_dumps-352"><span class="linenos">352</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-353"><a href="#Pathier.json_dumps-353"><span class="linenos">353</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-354"><a href="#Pathier.json_dumps-354"><span class="linenos">354</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-355"><a href="#Pathier.json_dumps-355"><span class="linenos">355</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-356"><a href="#Pathier.json_dumps-356"><span class="linenos">356</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-357"><a href="#Pathier.json_dumps-357"><span class="linenos">357</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-358"><a href="#Pathier.json_dumps-358"><span class="linenos">358</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-359"><a href="#Pathier.json_dumps-359"><span class="linenos">359</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.json_dumps-360"><a href="#Pathier.json_dumps-360"><span class="linenos">360</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.json_dumps-361"><a href="#Pathier.json_dumps-361"><span class="linenos">361</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier.json_dumps-362"><a href="#Pathier.json_dumps-362"><span class="linenos">362</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
-</span><span id="Pathier.json_dumps-363"><a href="#Pathier.json_dumps-363"><span class="linenos">363</span></a>            <span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-364"><a href="#Pathier.json_dumps-364"><span class="linenos">364</span></a>            <span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-365"><a href="#Pathier.json_dumps-365"><span class="linenos">365</span></a>            <span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-366"><a href="#Pathier.json_dumps-366"><span class="linenos">366</span></a>            <span class="n">parents</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-367"><a href="#Pathier.json_dumps-367"><span class="linenos">367</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_dumps-354"><a href="#Pathier.json_dumps-354"><span class="linenos">354</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier.json_dumps-355"><a href="#Pathier.json_dumps-355"><span class="linenos">355</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-356"><a href="#Pathier.json_dumps-356"><span class="linenos">356</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-357"><a href="#Pathier.json_dumps-357"><span class="linenos">357</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-358"><a href="#Pathier.json_dumps-358"><span class="linenos">358</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-359"><a href="#Pathier.json_dumps-359"><span class="linenos">359</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-360"><a href="#Pathier.json_dumps-360"><span class="linenos">360</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-361"><a href="#Pathier.json_dumps-361"><span class="linenos">361</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-362"><a href="#Pathier.json_dumps-362"><span class="linenos">362</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-363"><a href="#Pathier.json_dumps-363"><span class="linenos">363</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-364"><a href="#Pathier.json_dumps-364"><span class="linenos">364</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.json_dumps-365"><a href="#Pathier.json_dumps-365"><span class="linenos">365</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.json_dumps-366"><a href="#Pathier.json_dumps-366"><span class="linenos">366</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier.json_dumps-367"><a href="#Pathier.json_dumps-367"><span class="linenos">367</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
+</span><span id="Pathier.json_dumps-368"><a href="#Pathier.json_dumps-368"><span class="linenos">368</span></a>            <span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-369"><a href="#Pathier.json_dumps-369"><span class="linenos">369</span></a>            <span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-370"><a href="#Pathier.json_dumps-370"><span class="linenos">370</span></a>            <span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-371"><a href="#Pathier.json_dumps-371"><span class="linenos">371</span></a>            <span class="n">parents</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-372"><a href="#Pathier.json_dumps-372"><span class="linenos">372</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dump <code>data</code> to json file.</p>
 </div>
 
 
@@ -1559,17 +1580,17 @@
         <span class="def">def</span>
         <span class="name">toml_loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.toml_loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.toml_loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_loads-369"><a href="#Pathier.toml_loads-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.toml_loads-370"><a href="#Pathier.toml_loads-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.toml_loads-371"><a href="#Pathier.toml_loads-371"><span class="linenos">371</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span><span class="o">.</span><span class="n">unwrap</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_loads-374"><a href="#Pathier.toml_loads-374"><span class="linenos">374</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.toml_loads-375"><a href="#Pathier.toml_loads-375"><span class="linenos">375</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.toml_loads-376"><a href="#Pathier.toml_loads-376"><span class="linenos">376</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span><span class="o">.</span><span class="n">unwrap</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load toml file.</p>
 </div>
 
 
@@ -1581,27 +1602,27 @@
         <span class="def">def</span>
         <span class="name">toml_dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.toml_dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.toml_dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_dumps-373"><a href="#Pathier.toml_dumps-373"><span class="linenos">373</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
-</span><span id="Pathier.toml_dumps-374"><a href="#Pathier.toml_dumps-374"><span class="linenos">374</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-375"><a href="#Pathier.toml_dumps-375"><span class="linenos">375</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-376"><a href="#Pathier.toml_dumps-376"><span class="linenos">376</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-377"><a href="#Pathier.toml_dumps-377"><span class="linenos">377</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-378"><a href="#Pathier.toml_dumps-378"><span class="linenos">378</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-379"><a href="#Pathier.toml_dumps-379"><span class="linenos">379</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-380"><a href="#Pathier.toml_dumps-380"><span class="linenos">380</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-381"><a href="#Pathier.toml_dumps-381"><span class="linenos">381</span></a>    <span class="p">):</span>
-</span><span id="Pathier.toml_dumps-382"><a href="#Pathier.toml_dumps-382"><span class="linenos">382</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.toml_dumps-383"><a href="#Pathier.toml_dumps-383"><span class="linenos">383</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier.toml_dumps-384"><a href="#Pathier.toml_dumps-384"><span class="linenos">384</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier.toml_dumps-385"><a href="#Pathier.toml_dumps-385"><span class="linenos">385</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_dumps-378"><a href="#Pathier.toml_dumps-378"><span class="linenos">378</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
+</span><span id="Pathier.toml_dumps-379"><a href="#Pathier.toml_dumps-379"><span class="linenos">379</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-380"><a href="#Pathier.toml_dumps-380"><span class="linenos">380</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-381"><a href="#Pathier.toml_dumps-381"><span class="linenos">381</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-382"><a href="#Pathier.toml_dumps-382"><span class="linenos">382</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-383"><a href="#Pathier.toml_dumps-383"><span class="linenos">383</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-384"><a href="#Pathier.toml_dumps-384"><span class="linenos">384</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-385"><a href="#Pathier.toml_dumps-385"><span class="linenos">385</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-386"><a href="#Pathier.toml_dumps-386"><span class="linenos">386</span></a>    <span class="p">):</span>
+</span><span id="Pathier.toml_dumps-387"><a href="#Pathier.toml_dumps-387"><span class="linenos">387</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.toml_dumps-388"><a href="#Pathier.toml_dumps-388"><span class="linenos">388</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier.toml_dumps-389"><a href="#Pathier.toml_dumps-389"><span class="linenos">389</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier.toml_dumps-390"><a href="#Pathier.toml_dumps-390"><span class="linenos">390</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dump <code>data</code> to toml file.</p>
 </div>
 
 
@@ -1613,21 +1634,21 @@
         <span class="def">def</span>
         <span class="name">loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.loads-387"><a href="#Pathier.loads-387"><span class="linenos">387</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.loads-388"><a href="#Pathier.loads-388"><span class="linenos">388</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier.loads-389"><a href="#Pathier.loads-389"><span class="linenos">389</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier.loads-390"><a href="#Pathier.loads-390"><span class="linenos">390</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier.loads-391"><a href="#Pathier.loads-391"><span class="linenos">391</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier.loads-392"><a href="#Pathier.loads-392"><span class="linenos">392</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier.loads-393"><a href="#Pathier.loads-393"><span class="linenos">393</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.loads-392"><a href="#Pathier.loads-392"><span class="linenos">392</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.loads-393"><a href="#Pathier.loads-393"><span class="linenos">393</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier.loads-394"><a href="#Pathier.loads-394"><span class="linenos">394</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier.loads-395"><a href="#Pathier.loads-395"><span class="linenos">395</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier.loads-396"><a href="#Pathier.loads-396"><span class="linenos">396</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier.loads-397"><a href="#Pathier.loads-397"><span class="linenos">397</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier.loads-398"><a href="#Pathier.loads-398"><span class="linenos">398</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load a json or toml file based off this instance's suffix.</p>
 </div>
 
 
@@ -1639,33 +1660,33 @@
         <span class="def">def</span>
         <span class="name">dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">indent</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">default</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.dumps-395"><a href="#Pathier.dumps-395"><span class="linenos">395</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
-</span><span id="Pathier.dumps-396"><a href="#Pathier.dumps-396"><span class="linenos">396</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.dumps-397"><a href="#Pathier.dumps-397"><span class="linenos">397</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.dumps-398"><a href="#Pathier.dumps-398"><span class="linenos">398</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-399"><a href="#Pathier.dumps-399"><span class="linenos">399</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-400"><a href="#Pathier.dumps-400"><span class="linenos">400</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-401"><a href="#Pathier.dumps-401"><span class="linenos">401</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.dumps-402"><a href="#Pathier.dumps-402"><span class="linenos">402</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-403"><a href="#Pathier.dumps-403"><span class="linenos">403</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-404"><a href="#Pathier.dumps-404"><span class="linenos">404</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.dumps-405"><a href="#Pathier.dumps-405"><span class="linenos">405</span></a>    <span class="p">):</span>
-</span><span id="Pathier.dumps-406"><a href="#Pathier.dumps-406"><span class="linenos">406</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier.dumps-407"><a href="#Pathier.dumps-407"><span class="linenos">407</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier.dumps-408"><a href="#Pathier.dumps-408"><span class="linenos">408</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier.dumps-409"><a href="#Pathier.dumps-409"><span class="linenos">409</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier.dumps-410"><a href="#Pathier.dumps-410"><span class="linenos">410</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier.dumps-411"><a href="#Pathier.dumps-411"><span class="linenos">411</span></a>                <span class="p">)</span>
-</span><span id="Pathier.dumps-412"><a href="#Pathier.dumps-412"><span class="linenos">412</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier.dumps-413"><a href="#Pathier.dumps-413"><span class="linenos">413</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.dumps-400"><a href="#Pathier.dumps-400"><span class="linenos">400</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
+</span><span id="Pathier.dumps-401"><a href="#Pathier.dumps-401"><span class="linenos">401</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.dumps-402"><a href="#Pathier.dumps-402"><span class="linenos">402</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.dumps-403"><a href="#Pathier.dumps-403"><span class="linenos">403</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-404"><a href="#Pathier.dumps-404"><span class="linenos">404</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-405"><a href="#Pathier.dumps-405"><span class="linenos">405</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-406"><a href="#Pathier.dumps-406"><span class="linenos">406</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.dumps-407"><a href="#Pathier.dumps-407"><span class="linenos">407</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-408"><a href="#Pathier.dumps-408"><span class="linenos">408</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-409"><a href="#Pathier.dumps-409"><span class="linenos">409</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.dumps-410"><a href="#Pathier.dumps-410"><span class="linenos">410</span></a>    <span class="p">):</span>
+</span><span id="Pathier.dumps-411"><a href="#Pathier.dumps-411"><span class="linenos">411</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier.dumps-412"><a href="#Pathier.dumps-412"><span class="linenos">412</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier.dumps-413"><a href="#Pathier.dumps-413"><span class="linenos">413</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier.dumps-414"><a href="#Pathier.dumps-414"><span class="linenos">414</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier.dumps-415"><a href="#Pathier.dumps-415"><span class="linenos">415</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier.dumps-416"><a href="#Pathier.dumps-416"><span class="linenos">416</span></a>                <span class="p">)</span>
+</span><span id="Pathier.dumps-417"><a href="#Pathier.dumps-417"><span class="linenos">417</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier.dumps-418"><a href="#Pathier.dumps-418"><span class="linenos">418</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Dump <code>data</code> to a json or toml file based off this instance's suffix.</p>
 </div>
 
 
@@ -1677,22 +1698,22 @@
         <span class="def">def</span>
         <span class="name">delete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.delete-415"><a href="#Pathier.delete-415"><span class="linenos">415</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.delete-416"><a href="#Pathier.delete-416"><span class="linenos">416</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
-</span><span id="Pathier.delete-417"><a href="#Pathier.delete-417"><span class="linenos">417</span></a>
-</span><span id="Pathier.delete-418"><a href="#Pathier.delete-418"><span class="linenos">418</span></a><span class="sd">        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier.delete-419"><a href="#Pathier.delete-419"><span class="linenos">419</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.delete-420"><a href="#Pathier.delete-420"><span class="linenos">420</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
-</span><span id="Pathier.delete-421"><a href="#Pathier.delete-421"><span class="linenos">421</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.delete-422"><a href="#Pathier.delete-422"><span class="linenos">422</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.delete-420"><a href="#Pathier.delete-420"><span class="linenos">420</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.delete-421"><a href="#Pathier.delete-421"><span class="linenos">421</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
+</span><span id="Pathier.delete-422"><a href="#Pathier.delete-422"><span class="linenos">422</span></a>
+</span><span id="Pathier.delete-423"><a href="#Pathier.delete-423"><span class="linenos">423</span></a><span class="sd">        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier.delete-424"><a href="#Pathier.delete-424"><span class="linenos">424</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier.delete-425"><a href="#Pathier.delete-425"><span class="linenos">425</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
+</span><span id="Pathier.delete-426"><a href="#Pathier.delete-426"><span class="linenos">426</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier.delete-427"><a href="#Pathier.delete-427"><span class="linenos">427</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete the file or folder pointed to by this instance.</p>
 
 <p>Uses <code>self.unlink()</code> if a file and uses <code>shutil.rmtree()</code> if a directory.</p>
 </div>
@@ -1706,43 +1727,43 @@
         <span class="def">def</span>
         <span class="name">copy</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">new_path</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">Self</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.copy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.copy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.copy-424"><a href="#Pathier.copy-424"><span class="linenos">424</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
-</span><span id="Pathier.copy-425"><a href="#Pathier.copy-425"><span class="linenos">425</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Pathier.copy-426"><a href="#Pathier.copy-426"><span class="linenos">426</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.copy-427"><a href="#Pathier.copy-427"><span class="linenos">427</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
-</span><span id="Pathier.copy-428"><a href="#Pathier.copy-428"><span class="linenos">428</span></a><span class="sd">        to the instance pointed to by `new_path` using `shutil.copyfile`</span>
-</span><span id="Pathier.copy-429"><a href="#Pathier.copy-429"><span class="linenos">429</span></a><span class="sd">        or `shutil.copytree`.</span>
-</span><span id="Pathier.copy-430"><a href="#Pathier.copy-430"><span class="linenos">430</span></a>
-</span><span id="Pathier.copy-431"><a href="#Pathier.copy-431"><span class="linenos">431</span></a><span class="sd">        Returns the new path.</span>
-</span><span id="Pathier.copy-432"><a href="#Pathier.copy-432"><span class="linenos">432</span></a>
-</span><span id="Pathier.copy-433"><a href="#Pathier.copy-433"><span class="linenos">433</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.copy-434"><a href="#Pathier.copy-434"><span class="linenos">434</span></a>
-</span><span id="Pathier.copy-435"><a href="#Pathier.copy-435"><span class="linenos">435</span></a><span class="sd">        `new_path`: The copy destination.</span>
-</span><span id="Pathier.copy-436"><a href="#Pathier.copy-436"><span class="linenos">436</span></a>
-</span><span id="Pathier.copy-437"><a href="#Pathier.copy-437"><span class="linenos">437</span></a><span class="sd">        `overwrite`: If `True`, files already existing in `new_path` will be overwritten.</span>
-</span><span id="Pathier.copy-438"><a href="#Pathier.copy-438"><span class="linenos">438</span></a><span class="sd">        If `False`, only files that don&#39;t exist in `new_path` will be copied.&quot;&quot;&quot;</span>
-</span><span id="Pathier.copy-439"><a href="#Pathier.copy-439"><span class="linenos">439</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier.copy-440"><a href="#Pathier.copy-440"><span class="linenos">440</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.copy-441"><a href="#Pathier.copy-441"><span class="linenos">441</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-442"><a href="#Pathier.copy-442"><span class="linenos">442</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.copy-443"><a href="#Pathier.copy-443"><span class="linenos">443</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.copy-444"><a href="#Pathier.copy-444"><span class="linenos">444</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
-</span><span id="Pathier.copy-445"><a href="#Pathier.copy-445"><span class="linenos">445</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Pathier.copy-446"><a href="#Pathier.copy-446"><span class="linenos">446</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="Pathier.copy-447"><a href="#Pathier.copy-447"><span class="linenos">447</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-448"><a href="#Pathier.copy-448"><span class="linenos">448</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
-</span><span id="Pathier.copy-449"><a href="#Pathier.copy-449"><span class="linenos">449</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.copy-450"><a href="#Pathier.copy-450"><span class="linenos">450</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-451"><a href="#Pathier.copy-451"><span class="linenos">451</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier.copy-452"><a href="#Pathier.copy-452"><span class="linenos">452</span></a>        <span class="k">return</span> <span class="n">new_path</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.copy-429"><a href="#Pathier.copy-429"><span class="linenos">429</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
+</span><span id="Pathier.copy-430"><a href="#Pathier.copy-430"><span class="linenos">430</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Pathier.copy-431"><a href="#Pathier.copy-431"><span class="linenos">431</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.copy-432"><a href="#Pathier.copy-432"><span class="linenos">432</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
+</span><span id="Pathier.copy-433"><a href="#Pathier.copy-433"><span class="linenos">433</span></a><span class="sd">        to the instance pointed to by `new_path` using `shutil.copyfile`</span>
+</span><span id="Pathier.copy-434"><a href="#Pathier.copy-434"><span class="linenos">434</span></a><span class="sd">        or `shutil.copytree`.</span>
+</span><span id="Pathier.copy-435"><a href="#Pathier.copy-435"><span class="linenos">435</span></a>
+</span><span id="Pathier.copy-436"><a href="#Pathier.copy-436"><span class="linenos">436</span></a><span class="sd">        Returns the new path.</span>
+</span><span id="Pathier.copy-437"><a href="#Pathier.copy-437"><span class="linenos">437</span></a>
+</span><span id="Pathier.copy-438"><a href="#Pathier.copy-438"><span class="linenos">438</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.copy-439"><a href="#Pathier.copy-439"><span class="linenos">439</span></a>
+</span><span id="Pathier.copy-440"><a href="#Pathier.copy-440"><span class="linenos">440</span></a><span class="sd">        `new_path`: The copy destination.</span>
+</span><span id="Pathier.copy-441"><a href="#Pathier.copy-441"><span class="linenos">441</span></a>
+</span><span id="Pathier.copy-442"><a href="#Pathier.copy-442"><span class="linenos">442</span></a><span class="sd">        `overwrite`: If `True`, files already existing in `new_path` will be overwritten.</span>
+</span><span id="Pathier.copy-443"><a href="#Pathier.copy-443"><span class="linenos">443</span></a><span class="sd">        If `False`, only files that don&#39;t exist in `new_path` will be copied.&quot;&quot;&quot;</span>
+</span><span id="Pathier.copy-444"><a href="#Pathier.copy-444"><span class="linenos">444</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier.copy-445"><a href="#Pathier.copy-445"><span class="linenos">445</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier.copy-446"><a href="#Pathier.copy-446"><span class="linenos">446</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-447"><a href="#Pathier.copy-447"><span class="linenos">447</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.copy-448"><a href="#Pathier.copy-448"><span class="linenos">448</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.copy-449"><a href="#Pathier.copy-449"><span class="linenos">449</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
+</span><span id="Pathier.copy-450"><a href="#Pathier.copy-450"><span class="linenos">450</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Pathier.copy-451"><a href="#Pathier.copy-451"><span class="linenos">451</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="Pathier.copy-452"><a href="#Pathier.copy-452"><span class="linenos">452</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-453"><a href="#Pathier.copy-453"><span class="linenos">453</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
+</span><span id="Pathier.copy-454"><a href="#Pathier.copy-454"><span class="linenos">454</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier.copy-455"><a href="#Pathier.copy-455"><span class="linenos">455</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-456"><a href="#Pathier.copy-456"><span class="linenos">456</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier.copy-457"><a href="#Pathier.copy-457"><span class="linenos">457</span></a>        <span class="k">return</span> <span class="n">new_path</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Copy the path pointed to by this instance
 to the instance pointed to by <code>new_path</code> using <code>shutil.copyfile</code>
 or <code>shutil.copytree</code>.</p>
 
@@ -1765,38 +1786,38 @@
         <span class="def">def</span>
         <span class="name">backup</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Optional</span><span class="p">[</span><span class="n">Self</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.backup-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.backup"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.backup-454"><a href="#Pathier.backup-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier.backup-455"><a href="#Pathier.backup-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
-</span><span id="Pathier.backup-456"><a href="#Pathier.backup-456"><span class="linenos">456</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
-</span><span id="Pathier.backup-457"><a href="#Pathier.backup-457"><span class="linenos">457</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
-</span><span id="Pathier.backup-458"><a href="#Pathier.backup-458"><span class="linenos">458</span></a>
-</span><span id="Pathier.backup-459"><a href="#Pathier.backup-459"><span class="linenos">459</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.backup-460"><a href="#Pathier.backup-460"><span class="linenos">460</span></a>
-</span><span id="Pathier.backup-461"><a href="#Pathier.backup-461"><span class="linenos">461</span></a><span class="sd">        `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
-</span><span id="Pathier.backup-462"><a href="#Pathier.backup-462"><span class="linenos">462</span></a>
-</span><span id="Pathier.backup-463"><a href="#Pathier.backup-463"><span class="linenos">463</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
-</span><span id="Pathier.backup-464"><a href="#Pathier.backup-464"><span class="linenos">464</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
-</span><span id="Pathier.backup-465"><a href="#Pathier.backup-465"><span class="linenos">465</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier.backup-466"><a href="#Pathier.backup-466"><span class="linenos">466</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
-</span><span id="Pathier.backup-467"><a href="#Pathier.backup-467"><span class="linenos">467</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
-</span><span id="Pathier.backup-468"><a href="#Pathier.backup-468"><span class="linenos">468</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier.backup-469"><a href="#Pathier.backup-469"><span class="linenos">469</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
-</span><span id="Pathier.backup-470"><a href="#Pathier.backup-470"><span class="linenos">470</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.backup-471"><a href="#Pathier.backup-471"><span class="linenos">471</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier.backup-472"><a href="#Pathier.backup-472"><span class="linenos">472</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
-</span><span id="Pathier.backup-473"><a href="#Pathier.backup-473"><span class="linenos">473</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
-</span><span id="Pathier.backup-474"><a href="#Pathier.backup-474"><span class="linenos">474</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Pathier.backup-475"><a href="#Pathier.backup-475"><span class="linenos">475</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
-</span><span id="Pathier.backup-476"><a href="#Pathier.backup-476"><span class="linenos">476</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.backup-477"><a href="#Pathier.backup-477"><span class="linenos">477</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.backup-459"><a href="#Pathier.backup-459"><span class="linenos">459</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier.backup-460"><a href="#Pathier.backup-460"><span class="linenos">460</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
+</span><span id="Pathier.backup-461"><a href="#Pathier.backup-461"><span class="linenos">461</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
+</span><span id="Pathier.backup-462"><a href="#Pathier.backup-462"><span class="linenos">462</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
+</span><span id="Pathier.backup-463"><a href="#Pathier.backup-463"><span class="linenos">463</span></a>
+</span><span id="Pathier.backup-464"><a href="#Pathier.backup-464"><span class="linenos">464</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.backup-465"><a href="#Pathier.backup-465"><span class="linenos">465</span></a>
+</span><span id="Pathier.backup-466"><a href="#Pathier.backup-466"><span class="linenos">466</span></a><span class="sd">        `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
+</span><span id="Pathier.backup-467"><a href="#Pathier.backup-467"><span class="linenos">467</span></a>
+</span><span id="Pathier.backup-468"><a href="#Pathier.backup-468"><span class="linenos">468</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
+</span><span id="Pathier.backup-469"><a href="#Pathier.backup-469"><span class="linenos">469</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
+</span><span id="Pathier.backup-470"><a href="#Pathier.backup-470"><span class="linenos">470</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier.backup-471"><a href="#Pathier.backup-471"><span class="linenos">471</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
+</span><span id="Pathier.backup-472"><a href="#Pathier.backup-472"><span class="linenos">472</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
+</span><span id="Pathier.backup-473"><a href="#Pathier.backup-473"><span class="linenos">473</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier.backup-474"><a href="#Pathier.backup-474"><span class="linenos">474</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
+</span><span id="Pathier.backup-475"><a href="#Pathier.backup-475"><span class="linenos">475</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.backup-476"><a href="#Pathier.backup-476"><span class="linenos">476</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier.backup-477"><a href="#Pathier.backup-477"><span class="linenos">477</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
+</span><span id="Pathier.backup-478"><a href="#Pathier.backup-478"><span class="linenos">478</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
+</span><span id="Pathier.backup-479"><a href="#Pathier.backup-479"><span class="linenos">479</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Pathier.backup-480"><a href="#Pathier.backup-480"><span class="linenos">480</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
+</span><span id="Pathier.backup-481"><a href="#Pathier.backup-481"><span class="linenos">481</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.backup-482"><a href="#Pathier.backup-482"><span class="linenos">482</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a copy of this file or directory with <code>_backup</code> appended to the path stem.
 If the path to be backed up doesn't exist, <code>None</code> is returned.
 Otherwise a <code><a href="#Pathier">Pathier</a></code> object for the backup is returned.</p>
 
@@ -1825,32 +1846,32 @@
         <span class="def">def</span>
         <span class="name">execute</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.execute-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.execute"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.execute-479"><a href="#Pathier.execute-479"><span class="linenos">479</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Pathier.execute-480"><a href="#Pathier.execute-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Make a call to `os.system` using the path pointed to by this Pathier object.</span>
-</span><span id="Pathier.execute-481"><a href="#Pathier.execute-481"><span class="linenos">481</span></a>
-</span><span id="Pathier.execute-482"><a href="#Pathier.execute-482"><span class="linenos">482</span></a><span class="sd">        #### :params:</span>
-</span><span id="Pathier.execute-483"><a href="#Pathier.execute-483"><span class="linenos">483</span></a>
-</span><span id="Pathier.execute-484"><a href="#Pathier.execute-484"><span class="linenos">484</span></a><span class="sd">        `command`: Program/command to precede the path with.</span>
-</span><span id="Pathier.execute-485"><a href="#Pathier.execute-485"><span class="linenos">485</span></a>
-</span><span id="Pathier.execute-486"><a href="#Pathier.execute-486"><span class="linenos">486</span></a><span class="sd">        `args`: Any arguments that should come after the path.</span>
-</span><span id="Pathier.execute-487"><a href="#Pathier.execute-487"><span class="linenos">487</span></a>
-</span><span id="Pathier.execute-488"><a href="#Pathier.execute-488"><span class="linenos">488</span></a><span class="sd">        :returns: The integer output of `os.system`.</span>
-</span><span id="Pathier.execute-489"><a href="#Pathier.execute-489"><span class="linenos">489</span></a>
-</span><span id="Pathier.execute-490"><a href="#Pathier.execute-490"><span class="linenos">490</span></a><span class="sd">        e.g.</span>
-</span><span id="Pathier.execute-491"><a href="#Pathier.execute-491"><span class="linenos">491</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;mydirectory&quot;) / &quot;myscript.py&quot;</span>
-</span><span id="Pathier.execute-492"><a href="#Pathier.execute-492"><span class="linenos">492</span></a><span class="sd">        then</span>
-</span><span id="Pathier.execute-493"><a href="#Pathier.execute-493"><span class="linenos">493</span></a><span class="sd">        &gt;&gt;&gt; path.execute(&quot;py&quot;, &quot;--iterations 10&quot;)</span>
-</span><span id="Pathier.execute-494"><a href="#Pathier.execute-494"><span class="linenos">494</span></a><span class="sd">        equivalent to</span>
-</span><span id="Pathier.execute-495"><a href="#Pathier.execute-495"><span class="linenos">495</span></a><span class="sd">        &gt;&gt;&gt; os.system(f&quot;py {path} --iterations 10&quot;)&quot;&quot;&quot;</span>
-</span><span id="Pathier.execute-496"><a href="#Pathier.execute-496"><span class="linenos">496</span></a>        <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.execute-484"><a href="#Pathier.execute-484"><span class="linenos">484</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Pathier.execute-485"><a href="#Pathier.execute-485"><span class="linenos">485</span></a>        <span class="sd">&quot;&quot;&quot;Make a call to `os.system` using the path pointed to by this Pathier object.</span>
+</span><span id="Pathier.execute-486"><a href="#Pathier.execute-486"><span class="linenos">486</span></a>
+</span><span id="Pathier.execute-487"><a href="#Pathier.execute-487"><span class="linenos">487</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.execute-488"><a href="#Pathier.execute-488"><span class="linenos">488</span></a>
+</span><span id="Pathier.execute-489"><a href="#Pathier.execute-489"><span class="linenos">489</span></a><span class="sd">        `command`: Program/command to precede the path with.</span>
+</span><span id="Pathier.execute-490"><a href="#Pathier.execute-490"><span class="linenos">490</span></a>
+</span><span id="Pathier.execute-491"><a href="#Pathier.execute-491"><span class="linenos">491</span></a><span class="sd">        `args`: Any arguments that should come after the path.</span>
+</span><span id="Pathier.execute-492"><a href="#Pathier.execute-492"><span class="linenos">492</span></a>
+</span><span id="Pathier.execute-493"><a href="#Pathier.execute-493"><span class="linenos">493</span></a><span class="sd">        :returns: The integer output of `os.system`.</span>
+</span><span id="Pathier.execute-494"><a href="#Pathier.execute-494"><span class="linenos">494</span></a>
+</span><span id="Pathier.execute-495"><a href="#Pathier.execute-495"><span class="linenos">495</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier.execute-496"><a href="#Pathier.execute-496"><span class="linenos">496</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;mydirectory&quot;) / &quot;myscript.py&quot;</span>
+</span><span id="Pathier.execute-497"><a href="#Pathier.execute-497"><span class="linenos">497</span></a><span class="sd">        then</span>
+</span><span id="Pathier.execute-498"><a href="#Pathier.execute-498"><span class="linenos">498</span></a><span class="sd">        &gt;&gt;&gt; path.execute(&quot;py&quot;, &quot;--iterations 10&quot;)</span>
+</span><span id="Pathier.execute-499"><a href="#Pathier.execute-499"><span class="linenos">499</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier.execute-500"><a href="#Pathier.execute-500"><span class="linenos">500</span></a><span class="sd">        &gt;&gt;&gt; os.system(f&quot;py {path} --iterations 10&quot;)&quot;&quot;&quot;</span>
+</span><span id="Pathier.execute-501"><a href="#Pathier.execute-501"><span class="linenos">501</span></a>        <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make a call to <code>os.system</code> using the path pointed to by this Pathier object.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -7,14 +7,15 @@
           o dob
           o age
           o mod_date
           o mod_delta
           o last_read_time
           o modified_since_last_read
           o size
+          o formatted_size
           o format_bytes
           o is_larger
           o is_older
           o modified_more_recently
           o mkcwd
           o in_PATH
           o add_to_PATH
@@ -150,454 +151,460 @@
 _95            return 0
 _96        elif self.is_file():
 _97            return self.stat().st_size
 _98        elif self.is_dir():
 _99            return sum(file.stat().st_size for file in self.rglob("*.*"))
 100        return 0
 101
-102    @staticmethod
-103    def format_bytes(size: int) -> str:
-104        """Format `size` with common file size abbreviations and rounded to
+102    @property
+103    def formatted_size(self) -> str:
+104        """The size of this file or directory formatted with
+`self.format_bytes()`."""
+105        return self.format_bytes(self.size)
+106
+107    @staticmethod
+108    def format_bytes(size: int) -> str:
+109        """Format `size` with common file size abbreviations and rounded to
 two decimal places.
-105        >>> 1234 -> "1.23 kb" """
-106        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
-107            if unit != "bytes":
-108                size *= 0.001
-109            if size < 1000 or unit == "pb":
-110                return f"{round(size, 2)} {unit}"
-111
-112    def is_larger(self, path: Self) -> bool:
-113        """Returns whether this file or folder is larger than the one
+110        >>> 1234 -> "1.23 kb" """
+111        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
+112            if unit != "bytes":
+113                size *= 0.001
+114            if size < 1000 or unit == "pb":
+115                return f"{round(size, 2)} {unit}"
+116
+117    def is_larger(self, path: Self) -> bool:
+118        """Returns whether this file or folder is larger than the one
 pointed to by `path`."""
-114        return self.size > path.size
-115
-116    def is_older(self, path: Self) -> bool:
-117        """Returns whether this file or folder is older than the one pointed
+119        return self.size > path.size
+120
+121    def is_older(self, path: Self) -> bool:
+122        """Returns whether this file or folder is older than the one pointed
 to by `path`."""
-118        return self.dob < path.dob
-119
-120    def modified_more_recently(self, path: Self) -> bool:
-121        """Returns whether this file or folder was modified more recently
+123        return self.dob < path.dob
+124
+125    def modified_more_recently(self, path: Self) -> bool:
+126        """Returns whether this file or folder was modified more recently
 than the one pointed to by `path`."""
-122        return self.mod_date > path.mod_date
-123
-124    #
-===============================================navigation===============================================
-125    def mkcwd(self):
-126        """Make this path your current working directory."""
-127        os.chdir(self)
+127        return self.mod_date > path.mod_date
 128
-129    @property
-130    def in_PATH(self) -> bool:
-131        """Return `True` if this path is in `sys.path`."""
-132        return str(self) in sys.path
+129    #
+===============================================navigation===============================================
+130    def mkcwd(self):
+131        """Make this path your current working directory."""
+132        os.chdir(self)
 133
-134    def add_to_PATH(self, index: int = 0):
-135        """Insert this path into `sys.path` if it isn't already there.
-136
-137        #### :params:
+134    @property
+135    def in_PATH(self) -> bool:
+136        """Return `True` if this path is in `sys.path`."""
+137        return str(self) in sys.path
 138
-139        `index`: The index of `sys.path` to insert this path at."""
-140        path = str(self)
-141        if not self.in_PATH:
-142            sys.path.insert(index, path)
+139    def add_to_PATH(self, index: int = 0):
+140        """Insert this path into `sys.path` if it isn't already there.
+141
+142        #### :params:
 143
-144    def append_to_PATH(self):
-145        """Append this path to `sys.path` if it isn't already there."""
-146        path = str(self)
-147        if not self.in_PATH:
-148            sys.path.append(path)
-149
-150    def remove_from_PATH(self):
-151        """Remove this path from `sys.path` if it's in `sys.path`."""
-152        if self.in_PATH:
-153            sys.path.remove(str(self))
+144        `index`: The index of `sys.path` to insert this path at."""
+145        path = str(self)
+146        if not self.in_PATH:
+147            sys.path.insert(index, path)
+148
+149    def append_to_PATH(self):
+150        """Append this path to `sys.path` if it isn't already there."""
+151        path = str(self)
+152        if not self.in_PATH:
+153            sys.path.append(path)
 154
-155    def moveup(self, name: str) -> Self:
-156        """Return a new `Pathier` object that is a parent of this instance.
-157
-158        `name` is case-sensitive and raises an exception if it isn't in
+155    def remove_from_PATH(self):
+156        """Remove this path from `sys.path` if it's in `sys.path`."""
+157        if self.in_PATH:
+158            sys.path.remove(str(self))
+159
+160    def moveup(self, name: str) -> Self:
+161        """Return a new `Pathier` object that is a parent of this instance.
+162
+163        `name` is case-sensitive and raises an exception if it isn't in
 `self.parts`.
-159        >>> p = Pathier("C:\some\directory\in\your\system")
-160        >>> print(p.moveup("directory"))
-161        >>> "C:\some\directory"
-162        >>> print(p.moveup("yeet"))
-163        >>> "Exception: yeet is not a parent of C:
+164        >>> p = Pathier("C:\some\directory\in\your\system")
+165        >>> print(p.moveup("directory"))
+166        >>> "C:\some\directory"
+167        >>> print(p.moveup("yeet"))
+168        >>> "Exception: yeet is not a parent of C:
 \some\directory\in\your\system" """
-164        if name not in self.parts:
-165            raise Exception(f"{name} is not a parent of {self}")
-166        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
-167
-168    def __sub__(self, levels: int) -> Self:
-169        """Return a new `Pathier` object moved up `levels` number of parents
+169        if name not in self.parts:
+170            raise Exception(f"{name} is not a parent of {self}")
+171        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
+172
+173    def __sub__(self, levels: int) -> Self:
+174        """Return a new `Pathier` object moved up `levels` number of parents
 from the current path.
-170        >>> p = Pathier("C:\some\directory\in\your\system")
-171        >>> new_p = p - 3
-172        >>> print(new_p)
-173        >>> "C:\some\directory" """
-174        path = self
-175        for _ in range(levels):
-176            path = path.parent
-177        return path
-178
-179    def move_under(self, name: str) -> Self:
-180        """Return a new `Pathier` object such that the stem is one level
+175        >>> p = Pathier("C:\some\directory\in\your\system")
+176        >>> new_p = p - 3
+177        >>> print(new_p)
+178        >>> "C:\some\directory" """
+179        path = self
+180        for _ in range(levels):
+181            path = path.parent
+182        return path
+183
+184    def move_under(self, name: str) -> Self:
+185        """Return a new `Pathier` object such that the stem is one level
 below the given folder `name`.
-181
-182        `name` is case-sensitive and raises an exception if it isn't in
+186
+187        `name` is case-sensitive and raises an exception if it isn't in
 `self.parts`.
-183        >>> p = Pathier("a/b/c/d/e/f/g")
-184        >>> print(p.move_under("c"))
-185        >>> 'a/b/c/d'"""
-186        if name not in self.parts:
-187            raise Exception(f"{name} is not a parent of {self}")
-188        return self - (len(self.parts) - self.parts.index(name) - 2)
-189
-190    def separate(self, name: str, keep_name: bool = False) -> Self:
-191        """Return a new `Pathier` object that is the relative child path
+188        >>> p = Pathier("a/b/c/d/e/f/g")
+189        >>> print(p.move_under("c"))
+190        >>> 'a/b/c/d'"""
+191        if name not in self.parts:
+192            raise Exception(f"{name} is not a parent of {self}")
+193        return self - (len(self.parts) - self.parts.index(name) - 2)
+194
+195    def separate(self, name: str, keep_name: bool = False) -> Self:
+196        """Return a new `Pathier` object that is the relative child path
 after `name`.
-192
-193        `name` is case-sensitive and raises an exception if it isn't in
+197
+198        `name` is case-sensitive and raises an exception if it isn't in
 `self.parts`.
-194
-195        #### :params:
-196
-197        `keep_name`: If `True`, the returned path will start with `name`.
-198        >>> p = Pathier("a/b/c/d/e/f/g")
-199        >>> print(p.separate("c"))
-200        >>> 'd/e/f/g'
-201        >>> print(p.separate("c", True))
-202        >>> 'c/d/e/f/g'"""
-203        if name not in self.parts:
-204            raise Exception(f"{name} is not a parent of {self}")
-205        if keep_name:
-206            return Pathier(*self.parts[self.parts.index(name) :])
-207        return Pathier(*self.parts[self.parts.index(name) + 1 :])
-208
-209    # ============================================write and
+199
+200        #### :params:
+201
+202        `keep_name`: If `True`, the returned path will start with `name`.
+203        >>> p = Pathier("a/b/c/d/e/f/g")
+204        >>> print(p.separate("c"))
+205        >>> 'd/e/f/g'
+206        >>> print(p.separate("c", True))
+207        >>> 'c/d/e/f/g'"""
+208        if name not in self.parts:
+209            raise Exception(f"{name} is not a parent of {self}")
+210        if keep_name:
+211            return Pathier(*self.parts[self.parts.index(name) :])
+212        return Pathier(*self.parts[self.parts.index(name) + 1 :])
+213
+214    # ============================================write and
 read============================================
-210    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
+215    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
 True):
-211        """Create this directory.
-212
-213        Same as `Path().mkdir()` except `parents` and `exist_ok` default to
+216        """Create this directory.
+217
+218        Same as `Path().mkdir()` except `parents` and `exist_ok` default to
 `True` instead of `False`."""
-214        super().mkdir(mode, parents, exist_ok)
-215
-216    def touch(self):
-217        """Create file (and parents if necessary)."""
-218        self.parent.mkdir()
-219        super().touch()
+219        super().mkdir(mode, parents, exist_ok)
 220
-221    def open(self, mode="r", buffering=-1, encoding=None, errors=None,
+221    def touch(self):
+222        """Create file (and parents if necessary)."""
+223        self.parent.mkdir()
+224        super().touch()
+225
+226    def open(self, mode="r", buffering=-1, encoding=None, errors=None,
 newline=None):
-222        """
-223        Open the file pointed by this path and return a file object, as
-224        the built-in open() function does.
-225        """
-226        stream = super().open(mode, buffering, encoding, errors, newline)
-227        if "r" in mode:
-228            self._last_read_time = time.time()
-229        return stream
-230
-231    def write_text(
-232        self,
-233        data: Any,
-234        encoding: Any | None = None,
-235        errors: Any | None = None,
-236        newline: Any | None = None,
-237        parents: bool = True,
-238    ):
-239        """Write data to file.
-240
-241        If a `TypeError` is raised, the function  will attempt to cast
+227        """
+228        Open the file pointed by this path and return a file object, as
+229        the built-in open() function does.
+230        """
+231        stream = super().open(mode, buffering, encoding, errors, newline)
+232        if "r" in mode:
+233            self._last_read_time = time.time()
+234        return stream
+235
+236    def write_text(
+237        self,
+238        data: Any,
+239        encoding: Any | None = None,
+240        errors: Any | None = None,
+241        newline: Any | None = None,
+242        parents: bool = True,
+243    ):
+244        """Write data to file.
+245
+246        If a `TypeError` is raised, the function  will attempt to cast
 `data` to a `str` and try the write again.
-242
-243        If a `FileNotFoundError` is raised and `parents = True`,
+247
+248        If a `FileNotFoundError` is raised and `parents = True`,
 `self.parent` will be created."""
-244        write = functools.partial(
-245            super().write_text,
-246            encoding=encoding,
-247            errors=errors,
-248            newline=newline,
-249        )
-250        try:
-251            write(data)
-252        except TypeError:
-253            data = str(data)
-254            write(data)
-255        except FileNotFoundError:
-256            if parents:
-257                self.parent.mkdir(parents=True)
-258                write(data)
-259            else:
-260                raise
-261        except Exception as e:
-262            raise
-263
-264    def write_bytes(self, data: bytes, parents: bool = True):
-265        """Write bytes to file.
-266
-267        #### :params:
+249        write = functools.partial(
+250            super().write_text,
+251            encoding=encoding,
+252            errors=errors,
+253            newline=newline,
+254        )
+255        try:
+256            write(data)
+257        except TypeError:
+258            data = str(data)
+259            write(data)
+260        except FileNotFoundError:
+261            if parents:
+262                self.parent.mkdir(parents=True)
+263                write(data)
+264            else:
+265                raise
+266        except Exception as e:
+267            raise
 268
-269        `parents`: If `True` and the write operation fails with a
+269    def write_bytes(self, data: bytes, parents: bool = True):
+270        """Write bytes to file.
+271
+272        #### :params:
+273
+274        `parents`: If `True` and the write operation fails with a
 `FileNotFoundError`,
-270        make the parent directory and retry the write."""
-271        try:
-272            super().write_bytes(data)
-273        except FileNotFoundError:
-274            if parents:
-275                self.parent.mkdir(parents=True)
-276                super().write_bytes(data)
-277            else:
-278                raise
-279        except Exception as e:
-280            raise
-281
-282    def append(self, data: str, new_line: bool = True, encoding: Any | None
-= None):
-283        """Append `data` to the file pointed to by this `Pathier` object.
-284
-285        #### :params:
+275        make the parent directory and retry the write."""
+276        try:
+277            super().write_bytes(data)
+278        except FileNotFoundError:
+279            if parents:
+280                self.parent.mkdir(parents=True)
+281                super().write_bytes(data)
+282            else:
+283                raise
+284        except Exception as e:
+285            raise
 286
-287        `new_line`: If `True`, add `\\n` to `data`.
-288
-289        `encoding`: The file encoding to use."""
-290        if new_line:
-291            data += "\n"
-292        with self.open("a", encoding=encoding) as file:
-293            file.write(data)
-294
-295    def replace(
-296        self,
-297        substitutions: list[tuple[str, str]],
-298        count: int = -1,
-299        encoding: Any | None = None,
-300    ):
-301        """For each pair in `substitutions`, replace the first string with
+287    def append(self, data: str, new_line: bool = True, encoding: Any | None
+= None):
+288        """Append `data` to the file pointed to by this `Pathier` object.
+289
+290        #### :params:
+291
+292        `new_line`: If `True`, add `\\n` to `data`.
+293
+294        `encoding`: The file encoding to use."""
+295        if new_line:
+296            data += "\n"
+297        with self.open("a", encoding=encoding) as file:
+298            file.write(data)
+299
+300    def replace(
+301        self,
+302        substitutions: list[tuple[str, str]],
+303        count: int = -1,
+304        encoding: Any | None = None,
+305    ):
+306        """For each pair in `substitutions`, replace the first string with
 the second string.
-302
-303        #### :params:
-304
-305        `count`: Only replace this many occurences of each pair.
-306        By default (`-1`), all occurences are replaced.
 307
-308        `encoding`: The file encoding to use.
+308        #### :params:
 309
-310        e.g.
-311        >>> path = Pathier("somefile.txt")
-312        >>>
-313        >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
-314        equivalent to
-315        >>> path.write_text(path.read_text().replace("hello",
+310        `count`: Only replace this many occurences of each pair.
+311        By default (`-1`), all occurences are replaced.
+312
+313        `encoding`: The file encoding to use.
+314
+315        e.g.
+316        >>> path = Pathier("somefile.txt")
+317        >>>
+318        >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
+319        equivalent to
+320        >>> path.write_text(path.read_text().replace("hello",
 "yeet").replace("goodbye", "yeehaw"))"""
-316        text = self.read_text(encoding)
-317        for sub in substitutions:
-318            text = text.replace(sub[0], sub[1], count)
-319        self.write_text(text, encoding=encoding)
-320
-321    def join(self, data: list[str], encoding: Any | None = None, sep: str =
+321        text = self.read_text(encoding)
+322        for sub in substitutions:
+323            text = text.replace(sub[0], sub[1], count)
+324        self.write_text(text, encoding=encoding)
+325
+326    def join(self, data: list[str], encoding: Any | None = None, sep: str =
 "\n"):
-322        """Write a list of strings, joined by `sep`, to the file pointed at
+327        """Write a list of strings, joined by `sep`, to the file pointed at
 by this instance.
-323
-324        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
+328
+329        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
 encoding=encoding)`
-325
-326        #### :params:
-327
-328        `encoding`: The file encoding to use.
-329
-330        `sep`: The separator to use when joining `data`."""
-331        self.write_text(sep.join(data), encoding=encoding)
+330
+331        #### :params:
 332
-333    def split(self, encoding: Any | None = None, keepends: bool = False) -
+333        `encoding`: The file encoding to use.
+334
+335        `sep`: The separator to use when joining `data`."""
+336        self.write_text(sep.join(data), encoding=encoding)
+337
+338    def split(self, encoding: Any | None = None, keepends: bool = False) -
 > list[str]:
-334        """Returns the content of the pointed at file as a list of strings,
+339        """Returns the content of the pointed at file as a list of strings,
 splitting at new line characters.
-335
-336        Equivalent to `Pathier("somefile.txt").read_text
+340
+341        Equivalent to `Pathier("somefile.txt").read_text
 (encoding=encoding).splitlines()`
-337
-338        #### :params:
-339
-340        `encoding`: The file encoding to use.
-341
-342        `keepend`: If `True`, line breaks will be included in returned
-strings."""
-343        return self.read_text(encoding=encoding).splitlines(keepends)
+342
+343        #### :params:
 344
-345    def json_loads(self, encoding: Any | None = None, errors: Any | None =
+345        `encoding`: The file encoding to use.
+346
+347        `keepend`: If `True`, line breaks will be included in returned
+strings."""
+348        return self.read_text(encoding=encoding).splitlines(keepends)
+349
+350    def json_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-346        """Load json file."""
-347        return json.loads(self.read_text(encoding, errors))
-348
-349    def json_dumps(
-350        self,
-351        data: Any,
-352        encoding: Any | None = None,
-353        errors: Any | None = None,
-354        newline: Any | None = None,
-355        sort_keys: bool = False,
-356        indent: Any | None = None,
-357        default: Any | None = None,
-358        parents: bool = True,
-359    ) -> Any:
-360        """Dump `data` to json file."""
-361        self.write_text(
-362            json.dumps(data, indent=indent, default=default,
+351        """Load json file."""
+352        return json.loads(self.read_text(encoding, errors))
+353
+354    def json_dumps(
+355        self,
+356        data: Any,
+357        encoding: Any | None = None,
+358        errors: Any | None = None,
+359        newline: Any | None = None,
+360        sort_keys: bool = False,
+361        indent: Any | None = None,
+362        default: Any | None = None,
+363        parents: bool = True,
+364    ) -> Any:
+365        """Dump `data` to json file."""
+366        self.write_text(
+367            json.dumps(data, indent=indent, default=default,
 sort_keys=sort_keys),
-363            encoding,
-364            errors,
-365            newline,
-366            parents,
-367        )
-368
-369    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
+368            encoding,
+369            errors,
+370            newline,
+371            parents,
+372        )
+373
+374    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-370        """Load toml file."""
-371        return tomlkit.loads(self.read_text(encoding, errors)).unwrap()
-372
-373    def toml_dumps(
-374        self,
-375        data: Any,
-376        encoding: Any | None = None,
-377        errors: Any | None = None,
-378        newline: Any | None = None,
-379        sort_keys: bool = False,
-380        parents: bool = True,
-381    ):
-382        """Dump `data` to toml file."""
-383        self.write_text(
-384            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
+375        """Load toml file."""
+376        return tomlkit.loads(self.read_text(encoding, errors)).unwrap()
+377
+378    def toml_dumps(
+379        self,
+380        data: Any,
+381        encoding: Any | None = None,
+382        errors: Any | None = None,
+383        newline: Any | None = None,
+384        sort_keys: bool = False,
+385        parents: bool = True,
+386    ):
+387        """Dump `data` to toml file."""
+388        self.write_text(
+389            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
 parents
-385        )
-386
-387    def loads(self, encoding: Any | None = None, errors: Any | None = None)
+390        )
+391
+392    def loads(self, encoding: Any | None = None, errors: Any | None = None)
 -> Any:
-388        """Load a json or toml file based off this instance's suffix."""
-389        match self.suffix:
-390            case ".json":
-391                return self.json_loads(encoding, errors)
-392            case ".toml":
-393                return self.toml_loads(encoding, errors)
-394
-395    def dumps(
-396        self,
-397        data: Any,
-398        encoding: Any | None = None,
-399        errors: Any | None = None,
-400        newline: Any | None = None,
-401        sort_keys: bool = False,
-402        indent: Any | None = None,
-403        default: Any | None = None,
-404        parents: bool = True,
-405    ):
-406        """Dump `data` to a json or toml file based off this instance's
+393        """Load a json or toml file based off this instance's suffix."""
+394        match self.suffix:
+395            case ".json":
+396                return self.json_loads(encoding, errors)
+397            case ".toml":
+398                return self.toml_loads(encoding, errors)
+399
+400    def dumps(
+401        self,
+402        data: Any,
+403        encoding: Any | None = None,
+404        errors: Any | None = None,
+405        newline: Any | None = None,
+406        sort_keys: bool = False,
+407        indent: Any | None = None,
+408        default: Any | None = None,
+409        parents: bool = True,
+410    ):
+411        """Dump `data` to a json or toml file based off this instance's
 suffix."""
-407        match self.suffix:
-408            case ".json":
-409                self.json_dumps(
-410                    data, encoding, errors, newline, sort_keys, indent,
+412        match self.suffix:
+413            case ".json":
+414                self.json_dumps(
+415                    data, encoding, errors, newline, sort_keys, indent,
 default, parents
-411                )
-412            case ".toml":
-413                self.toml_dumps(data, encoding, errors, newline, sort_keys,
+416                )
+417            case ".toml":
+418                self.toml_dumps(data, encoding, errors, newline, sort_keys,
 parents)
-414
-415    def delete(self, missing_ok: bool = True):
-416        """Delete the file or folder pointed to by this instance.
-417
-418        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a
+419
+420    def delete(self, missing_ok: bool = True):
+421        """Delete the file or folder pointed to by this instance.
+422
+423        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a
 directory."""
-419        if self.is_file():
-420            self.unlink(missing_ok)
-421        elif self.is_dir():
-422            shutil.rmtree(self)
-423
-424    def copy(
-425        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
-426    ) -> Self:
-427        """Copy the path pointed to by this instance
-428        to the instance pointed to by `new_path` using `shutil.copyfile`
-429        or `shutil.copytree`.
-430
-431        Returns the new path.
-432
-433        #### :params:
-434
-435        `new_path`: The copy destination.
-436
-437        `overwrite`: If `True`, files already existing in `new_path` will be
+424        if self.is_file():
+425            self.unlink(missing_ok)
+426        elif self.is_dir():
+427            shutil.rmtree(self)
+428
+429    def copy(
+430        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
+431    ) -> Self:
+432        """Copy the path pointed to by this instance
+433        to the instance pointed to by `new_path` using `shutil.copyfile`
+434        or `shutil.copytree`.
+435
+436        Returns the new path.
+437
+438        #### :params:
+439
+440        `new_path`: The copy destination.
+441
+442        `overwrite`: If `True`, files already existing in `new_path` will be
 overwritten.
-438        If `False`, only files that don't exist in `new_path` will be
+443        If `False`, only files that don't exist in `new_path` will be
 copied."""
-439        new_path = Pathier(new_path)
-440        if self.is_dir():
-441            if overwrite or not new_path.exists():
-442                shutil.copytree(self, new_path, dirs_exist_ok=True)
-443            else:
-444                files = self.rglob("*.*")
-445                for file in files:
-446                    dst = new_path.with_name(file.name)
-447                    if not dst.exists():
-448                        shutil.copyfile(file, dst)
-449        elif self.is_file():
-450            if overwrite or not new_path.exists():
-451                shutil.copyfile(self, new_path)
-452        return new_path
-453
-454    def backup(self, timestamp: bool = False) -> Self | None:
-455        """Create a copy of this file or directory with `_backup` appended
-to the path stem.
-456        If the path to be backed up doesn't exist, `None` is returned.
-457        Otherwise a `Pathier` object for the backup is returned.
+444        new_path = Pathier(new_path)
+445        if self.is_dir():
+446            if overwrite or not new_path.exists():
+447                shutil.copytree(self, new_path, dirs_exist_ok=True)
+448            else:
+449                files = self.rglob("*.*")
+450                for file in files:
+451                    dst = new_path.with_name(file.name)
+452                    if not dst.exists():
+453                        shutil.copyfile(file, dst)
+454        elif self.is_file():
+455            if overwrite or not new_path.exists():
+456                shutil.copyfile(self, new_path)
+457        return new_path
 458
-459        #### :params:
-460
-461        `timestamp`: Add a timestamp to the backup name to prevent
+459    def backup(self, timestamp: bool = False) -> Self | None:
+460        """Create a copy of this file or directory with `_backup` appended
+to the path stem.
+461        If the path to be backed up doesn't exist, `None` is returned.
+462        Otherwise a `Pathier` object for the backup is returned.
+463
+464        #### :params:
+465
+466        `timestamp`: Add a timestamp to the backup name to prevent
 overriding previous backups.
-462
-463        >>> path = Pathier("some_file.txt")
-464        >>> path.backup()
-465        >>> list(path.iterdir())
-466        >>> ['some_file.txt', 'some_file_backup.txt']
-467        >>> path.backup(True)
-468        >>> list(path.iterdir())
-469        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
+467
+468        >>> path = Pathier("some_file.txt")
+469        >>> path.backup()
+470        >>> list(path.iterdir())
+471        >>> ['some_file.txt', 'some_file_backup.txt']
+472        >>> path.backup(True)
+473        >>> list(path.iterdir())
+474        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
 28-2023-06_25_52_PM.txt']"""
-470        if not self.exists():
-471            return None
-472        backup_stem = f"{self.stem}_backup"
-473        if timestamp:
-474            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
+475        if not self.exists():
+476            return None
+477        backup_stem = f"{self.stem}_backup"
+478        if timestamp:
+479            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
 ('%m-%d-%Y-%I_%M_%S_%p')}"
-475        backup_path = self.with_stem(backup_stem)
-476        self.copy(backup_path, True)
-477        return backup_path
-478
-479    def execute(self, command: str = "", args: str = "") -> int:
-480        """Make a call to `os.system` using the path pointed to by this
-Pathier object.
-481
-482        #### :params:
+480        backup_path = self.with_stem(backup_stem)
+481        self.copy(backup_path, True)
+482        return backup_path
 483
-484        `command`: Program/command to precede the path with.
-485
-486        `args`: Any arguments that should come after the path.
-487
-488        :returns: The integer output of `os.system`.
-489
-490        e.g.
-491        >>> path = Pathier("mydirectory") / "myscript.py"
-492        then
-493        >>> path.execute("py", "--iterations 10")
-494        equivalent to
-495        >>> os.system(f"py {path} --iterations 10")"""
-496        return os.system(f"{command} {self} {args}")
+484    def execute(self, command: str = "", args: str = "") -> int:
+485        """Make a call to `os.system` using the path pointed to by this
+Pathier object.
+486
+487        #### :params:
+488
+489        `command`: Program/command to precede the path with.
+490
+491        `args`: Any arguments that should come after the path.
+492
+493        :returns: The integer output of `os.system`.
+494
+495        e.g.
+496        >>> path = Pathier("mydirectory") / "myscript.py"
+497        then
+498        >>> path.execute("py", "--iterations 10")
+499        equivalent to
+500        >>> os.system(f"py {path} --iterations 10")"""
+501        return os.system(f"{command} {self} {args}")
 Subclasses the standard library pathlib.Path class.
 Pathier()
 dob: datetime.datetime | None
 Returns the creation date of this file or directory as a dateime.datetime
 object.
 age: float | None
 Returns the age in seconds of this file or directory.
@@ -624,330 +631,332 @@
 May not be accurate if the file was modified within a couple of seconds of
 checking this property. (For instance, on my machine self.mod_date is
 consistently 1-1.5s in the future from when self.write_text() was called
 according to time.time().)
 size: int
 Returns the size in bytes of this file or directory.
 If this path doesn't exist, 0 will be returned.
+formatted_size: str
+The size of this file or directory formatted with self.format_bytes().
 ⁰
 @staticmethod
 def format_bytes(size: int) -> str: View Source
-102    @staticmethod
-103    def format_bytes(size: int) -> str:
-104        """Format `size` with common file size abbreviations and rounded to
+107    @staticmethod
+108    def format_bytes(size: int) -> str:
+109        """Format `size` with common file size abbreviations and rounded to
 two decimal places.
-105        >>> 1234 -> "1.23 kb" """
-106        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
-107            if unit != "bytes":
-108                size *= 0.001
-109            if size < 1000 or unit == "pb":
-110                return f"{round(size, 2)} {unit}"
+110        >>> 1234 -> "1.23 kb" """
+111        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
+112            if unit != "bytes":
+113                size *= 0.001
+114            if size < 1000 or unit == "pb":
+115                return f"{round(size, 2)} {unit}"
 Format size with common file size abbreviations and rounded to two decimal
 places.
 >>> 1234 -> "1.23 kb"
 ⁰
 def is_larger(self, path: Self) -> bool: View Source
-112    def is_larger(self, path: Self) -> bool:
-113        """Returns whether this file or folder is larger than the one
+117    def is_larger(self, path: Self) -> bool:
+118        """Returns whether this file or folder is larger than the one
 pointed to by `path`."""
-114        return self.size > path.size
+119        return self.size > path.size
 Returns whether this file or folder is larger than the one pointed to by path.
 ⁰
 def is_older(self, path: Self) -> bool: View Source
-116    def is_older(self, path: Self) -> bool:
-117        """Returns whether this file or folder is older than the one pointed
+121    def is_older(self, path: Self) -> bool:
+122        """Returns whether this file or folder is older than the one pointed
 to by `path`."""
-118        return self.dob < path.dob
+123        return self.dob < path.dob
 Returns whether this file or folder is older than the one pointed to by path.
 ⁰
 def modified_more_recently(self, path: Self) -> bool: View Source
-120    def modified_more_recently(self, path: Self) -> bool:
-121        """Returns whether this file or folder was modified more recently
+125    def modified_more_recently(self, path: Self) -> bool:
+126        """Returns whether this file or folder was modified more recently
 than the one pointed to by `path`."""
-122        return self.mod_date > path.mod_date
+127        return self.mod_date > path.mod_date
 Returns whether this file or folder was modified more recently than the one
 pointed to by path.
 ⁰
 def mkcwd(self): View Source
-125    def mkcwd(self):
-126        """Make this path your current working directory."""
-127        os.chdir(self)
+130    def mkcwd(self):
+131        """Make this path your current working directory."""
+132        os.chdir(self)
 Make this path your current working directory.
 in_PATH: bool
 Return True if this path is in sys.path.
 ⁰
 def add_to_PATH(self, index: int = 0): View Source
-134    def add_to_PATH(self, index: int = 0):
-135        """Insert this path into `sys.path` if it isn't already there.
-136
-137        #### :params:
-138
-139        `index`: The index of `sys.path` to insert this path at."""
-140        path = str(self)
-141        if not self.in_PATH:
-142            sys.path.insert(index, path)
+139    def add_to_PATH(self, index: int = 0):
+140        """Insert this path into `sys.path` if it isn't already there.
+141
+142        #### :params:
+143
+144        `index`: The index of `sys.path` to insert this path at."""
+145        path = str(self)
+146        if not self.in_PATH:
+147            sys.path.insert(index, path)
 Insert this path into sys.path if it isn't already there.
 *** :params: ***
 index: The index of sys.path to insert this path at.
 ⁰
 def append_to_PATH(self): View Source
-144    def append_to_PATH(self):
-145        """Append this path to `sys.path` if it isn't already there."""
-146        path = str(self)
-147        if not self.in_PATH:
-148            sys.path.append(path)
+149    def append_to_PATH(self):
+150        """Append this path to `sys.path` if it isn't already there."""
+151        path = str(self)
+152        if not self.in_PATH:
+153            sys.path.append(path)
 Append this path to sys.path if it isn't already there.
 ⁰
 def remove_from_PATH(self): View Source
-150    def remove_from_PATH(self):
-151        """Remove this path from `sys.path` if it's in `sys.path`."""
-152        if self.in_PATH:
-153            sys.path.remove(str(self))
+155    def remove_from_PATH(self):
+156        """Remove this path from `sys.path` if it's in `sys.path`."""
+157        if self.in_PATH:
+158            sys.path.remove(str(self))
 Remove this path from sys.path if it's in sys.path.
 ⁰
 def moveup(self, name: str) -> Self: View Source
-155    def moveup(self, name: str) -> Self:
-156        """Return a new `Pathier` object that is a parent of this instance.
-157
-158        `name` is case-sensitive and raises an exception if it isn't in
+160    def moveup(self, name: str) -> Self:
+161        """Return a new `Pathier` object that is a parent of this instance.
+162
+163        `name` is case-sensitive and raises an exception if it isn't in
 `self.parts`.
-159        >>> p = Pathier("C:\some\directory\in\your\system")
-160        >>> print(p.moveup("directory"))
-161        >>> "C:\some\directory"
-162        >>> print(p.moveup("yeet"))
-163        >>> "Exception: yeet is not a parent of C:
+164        >>> p = Pathier("C:\some\directory\in\your\system")
+165        >>> print(p.moveup("directory"))
+166        >>> "C:\some\directory"
+167        >>> print(p.moveup("yeet"))
+168        >>> "Exception: yeet is not a parent of C:
 \some\directory\in\your\system" """
-164        if name not in self.parts:
-165            raise Exception(f"{name} is not a parent of {self}")
-166        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
+169        if name not in self.parts:
+170            raise Exception(f"{name} is not a parent of {self}")
+171        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
 Return a new Pathier object that is a parent of this instance.
 name is case-sensitive and raises an exception if it isn't in self.parts.
 >>> p = Pathier("C:\some\directory\in\your\system")
 >>> print(p.moveup("directory"))
 >>> "C:\some\directory"
 >>> print(p.moveup("yeet"))
 >>> "Exception: yeet is not a parent of C:\some\directory\in\your\system"
 ⁰
 def move_under(self, name: str) -> Self: View Source
-179    def move_under(self, name: str) -> Self:
-180        """Return a new `Pathier` object such that the stem is one level
+184    def move_under(self, name: str) -> Self:
+185        """Return a new `Pathier` object such that the stem is one level
 below the given folder `name`.
-181
-182        `name` is case-sensitive and raises an exception if it isn't in
+186
+187        `name` is case-sensitive and raises an exception if it isn't in
 `self.parts`.
-183        >>> p = Pathier("a/b/c/d/e/f/g")
-184        >>> print(p.move_under("c"))
-185        >>> 'a/b/c/d'"""
-186        if name not in self.parts:
-187            raise Exception(f"{name} is not a parent of {self}")
-188        return self - (len(self.parts) - self.parts.index(name) - 2)
+188        >>> p = Pathier("a/b/c/d/e/f/g")
+189        >>> print(p.move_under("c"))
+190        >>> 'a/b/c/d'"""
+191        if name not in self.parts:
+192            raise Exception(f"{name} is not a parent of {self}")
+193        return self - (len(self.parts) - self.parts.index(name) - 2)
 Return a new Pathier object such that the stem is one level below the given
 folder name.
 name is case-sensitive and raises an exception if it isn't in self.parts.
 >>> p = Pathier("a/b/c/d/e/f/g")
 >>> print(p.move_under("c"))
 >>> 'a/b/c/d'
 ⁰
 def separate(self, name: str, keep_name: bool = False) -> Self: View Source
-190    def separate(self, name: str, keep_name: bool = False) -> Self:
-191        """Return a new `Pathier` object that is the relative child path
+195    def separate(self, name: str, keep_name: bool = False) -> Self:
+196        """Return a new `Pathier` object that is the relative child path
 after `name`.
-192
-193        `name` is case-sensitive and raises an exception if it isn't in
+197
+198        `name` is case-sensitive and raises an exception if it isn't in
 `self.parts`.
-194
-195        #### :params:
-196
-197        `keep_name`: If `True`, the returned path will start with `name`.
-198        >>> p = Pathier("a/b/c/d/e/f/g")
-199        >>> print(p.separate("c"))
-200        >>> 'd/e/f/g'
-201        >>> print(p.separate("c", True))
-202        >>> 'c/d/e/f/g'"""
-203        if name not in self.parts:
-204            raise Exception(f"{name} is not a parent of {self}")
-205        if keep_name:
-206            return Pathier(*self.parts[self.parts.index(name) :])
-207        return Pathier(*self.parts[self.parts.index(name) + 1 :])
+199
+200        #### :params:
+201
+202        `keep_name`: If `True`, the returned path will start with `name`.
+203        >>> p = Pathier("a/b/c/d/e/f/g")
+204        >>> print(p.separate("c"))
+205        >>> 'd/e/f/g'
+206        >>> print(p.separate("c", True))
+207        >>> 'c/d/e/f/g'"""
+208        if name not in self.parts:
+209            raise Exception(f"{name} is not a parent of {self}")
+210        if keep_name:
+211            return Pathier(*self.parts[self.parts.index(name) :])
+212        return Pathier(*self.parts[self.parts.index(name) + 1 :])
 Return a new Pathier object that is the relative child path after name.
 name is case-sensitive and raises an exception if it isn't in self.parts.
 *** :params: ***
 keep_name: If True, the returned path will start with name.
 >>> p = Pathier("a/b/c/d/e/f/g")
 >>> print(p.separate("c"))
 >>> 'd/e/f/g'
 >>> print(p.separate("c", True))
 >>> 'c/d/e/f/g'
 ⁰
 def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool = True):
 View Source
-210    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
+215    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
 True):
-211        """Create this directory.
-212
-213        Same as `Path().mkdir()` except `parents` and `exist_ok` default to
+216        """Create this directory.
+217
+218        Same as `Path().mkdir()` except `parents` and `exist_ok` default to
 `True` instead of `False`."""
-214        super().mkdir(mode, parents, exist_ok)
+219        super().mkdir(mode, parents, exist_ok)
 Create this directory.
 Same as Path().mkdir() except parents and exist_ok default to True instead of
 False.
 ⁰
 def touch(self): View Source
-216    def touch(self):
-217        """Create file (and parents if necessary)."""
-218        self.parent.mkdir()
-219        super().touch()
+221    def touch(self):
+222        """Create file (and parents if necessary)."""
+223        self.parent.mkdir()
+224        super().touch()
 Create file (and parents if necessary).
 ⁰
 def open(
 self,
 mode='r',
 buffering=-1,
 encoding=None,
 errors=None,
 newline=None): View Source
-221    def open(self, mode="r", buffering=-1, encoding=None, errors=None,
+226    def open(self, mode="r", buffering=-1, encoding=None, errors=None,
 newline=None):
-222        """
-223        Open the file pointed by this path and return a file object, as
-224        the built-in open() function does.
-225        """
-226        stream = super().open(mode, buffering, encoding, errors, newline)
-227        if "r" in mode:
-228            self._last_read_time = time.time()
-229        return stream
+227        """
+228        Open the file pointed by this path and return a file object, as
+229        the built-in open() function does.
+230        """
+231        stream = super().open(mode, buffering, encoding, errors, newline)
+232        if "r" in mode:
+233            self._last_read_time = time.time()
+234        return stream
 Open the file pointed by this path and return a file object, as the built-in
 open() function does.
 ⁰
 def write_text(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 parents: bool = True): View Source
-231    def write_text(
-232        self,
-233        data: Any,
-234        encoding: Any | None = None,
-235        errors: Any | None = None,
-236        newline: Any | None = None,
-237        parents: bool = True,
-238    ):
-239        """Write data to file.
-240
-241        If a `TypeError` is raised, the function  will attempt to cast
+236    def write_text(
+237        self,
+238        data: Any,
+239        encoding: Any | None = None,
+240        errors: Any | None = None,
+241        newline: Any | None = None,
+242        parents: bool = True,
+243    ):
+244        """Write data to file.
+245
+246        If a `TypeError` is raised, the function  will attempt to cast
 `data` to a `str` and try the write again.
-242
-243        If a `FileNotFoundError` is raised and `parents = True`,
+247
+248        If a `FileNotFoundError` is raised and `parents = True`,
 `self.parent` will be created."""
-244        write = functools.partial(
-245            super().write_text,
-246            encoding=encoding,
-247            errors=errors,
-248            newline=newline,
-249        )
-250        try:
-251            write(data)
-252        except TypeError:
-253            data = str(data)
-254            write(data)
-255        except FileNotFoundError:
-256            if parents:
-257                self.parent.mkdir(parents=True)
-258                write(data)
-259            else:
-260                raise
-261        except Exception as e:
-262            raise
+249        write = functools.partial(
+250            super().write_text,
+251            encoding=encoding,
+252            errors=errors,
+253            newline=newline,
+254        )
+255        try:
+256            write(data)
+257        except TypeError:
+258            data = str(data)
+259            write(data)
+260        except FileNotFoundError:
+261            if parents:
+262                self.parent.mkdir(parents=True)
+263                write(data)
+264            else:
+265                raise
+266        except Exception as e:
+267            raise
 Write data to file.
 If a TypeError is raised, the function will attempt to cast data to a str and
 try the write again.
 If a FileNotFoundError is raised and parents = True, self.parent will be
 created.
 ⁰
 def write_bytes(self, data: bytes, parents: bool = True): View Source
-264    def write_bytes(self, data: bytes, parents: bool = True):
-265        """Write bytes to file.
-266
-267        #### :params:
-268
-269        `parents`: If `True` and the write operation fails with a
+269    def write_bytes(self, data: bytes, parents: bool = True):
+270        """Write bytes to file.
+271
+272        #### :params:
+273
+274        `parents`: If `True` and the write operation fails with a
 `FileNotFoundError`,
-270        make the parent directory and retry the write."""
-271        try:
-272            super().write_bytes(data)
-273        except FileNotFoundError:
-274            if parents:
-275                self.parent.mkdir(parents=True)
-276                super().write_bytes(data)
-277            else:
-278                raise
-279        except Exception as e:
-280            raise
+275        make the parent directory and retry the write."""
+276        try:
+277            super().write_bytes(data)
+278        except FileNotFoundError:
+279            if parents:
+280                self.parent.mkdir(parents=True)
+281                super().write_bytes(data)
+282            else:
+283                raise
+284        except Exception as e:
+285            raise
 Write bytes to file.
 *** :params: ***
 parents: If True and the write operation fails with a FileNotFoundError, make
 the parent directory and retry the write.
 ⁰
 def append(
 self,
 data: str,
 new_line: bool = True,
 encoding: typing.Any | None = None): View Source
-282    def append(self, data: str, new_line: bool = True, encoding: Any | None
+287    def append(self, data: str, new_line: bool = True, encoding: Any | None
 = None):
-283        """Append `data` to the file pointed to by this `Pathier` object.
-284
-285        #### :params:
-286
-287        `new_line`: If `True`, add `\\n` to `data`.
-288
-289        `encoding`: The file encoding to use."""
-290        if new_line:
-291            data += "\n"
-292        with self.open("a", encoding=encoding) as file:
-293            file.write(data)
+288        """Append `data` to the file pointed to by this `Pathier` object.
+289
+290        #### :params:
+291
+292        `new_line`: If `True`, add `\\n` to `data`.
+293
+294        `encoding`: The file encoding to use."""
+295        if new_line:
+296            data += "\n"
+297        with self.open("a", encoding=encoding) as file:
+298            file.write(data)
 Append data to the file pointed to by this Pathier object.
 *** :params: ***
 new_line: If True, add \n to data.
 encoding: The file encoding to use.
 ⁰
 def replace(
 self,
 substitutions: list[tuple[str, str]],
 count: int = -1,
 encoding: typing.Any | None = None): View Source
-295    def replace(
-296        self,
-297        substitutions: list[tuple[str, str]],
-298        count: int = -1,
-299        encoding: Any | None = None,
-300    ):
-301        """For each pair in `substitutions`, replace the first string with
+300    def replace(
+301        self,
+302        substitutions: list[tuple[str, str]],
+303        count: int = -1,
+304        encoding: Any | None = None,
+305    ):
+306        """For each pair in `substitutions`, replace the first string with
 the second string.
-302
-303        #### :params:
-304
-305        `count`: Only replace this many occurences of each pair.
-306        By default (`-1`), all occurences are replaced.
 307
-308        `encoding`: The file encoding to use.
+308        #### :params:
 309
-310        e.g.
-311        >>> path = Pathier("somefile.txt")
-312        >>>
-313        >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
-314        equivalent to
-315        >>> path.write_text(path.read_text().replace("hello",
+310        `count`: Only replace this many occurences of each pair.
+311        By default (`-1`), all occurences are replaced.
+312
+313        `encoding`: The file encoding to use.
+314
+315        e.g.
+316        >>> path = Pathier("somefile.txt")
+317        >>>
+318        >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
+319        equivalent to
+320        >>> path.write_text(path.read_text().replace("hello",
 "yeet").replace("goodbye", "yeehaw"))"""
-316        text = self.read_text(encoding)
-317        for sub in substitutions:
-318            text = text.replace(sub[0], sub[1], count)
-319        self.write_text(text, encoding=encoding)
+321        text = self.read_text(encoding)
+322        for sub in substitutions:
+323            text = text.replace(sub[0], sub[1], count)
+324        self.write_text(text, encoding=encoding)
 For each pair in substitutions, replace the first string with the second
 string.
 *** :params: ***
 count: Only replace this many occurences of each pair. By default (-1), all
 occurences are replaced.
 encoding: The file encoding to use.
 e.g.
@@ -959,271 +968,271 @@
 ("goodbye", "yeehaw"))
 ⁰
 def join(
 self,
 data: list[str],
 encoding: typing.Any | None = None,
 sep: str = '\n'): View Source
-321    def join(self, data: list[str], encoding: Any | None = None, sep: str =
+326    def join(self, data: list[str], encoding: Any | None = None, sep: str =
 "\n"):
-322        """Write a list of strings, joined by `sep`, to the file pointed at
+327        """Write a list of strings, joined by `sep`, to the file pointed at
 by this instance.
-323
-324        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
+328
+329        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
 encoding=encoding)`
-325
-326        #### :params:
-327
-328        `encoding`: The file encoding to use.
-329
-330        `sep`: The separator to use when joining `data`."""
-331        self.write_text(sep.join(data), encoding=encoding)
+330
+331        #### :params:
+332
+333        `encoding`: The file encoding to use.
+334
+335        `sep`: The separator to use when joining `data`."""
+336        self.write_text(sep.join(data), encoding=encoding)
 Write a list of strings, joined by sep, to the file pointed at by this
 instance.
 Equivalent to Pathier("somefile.txt").write_text(sep.join(data),
 encoding=encoding)
 *** :params: ***
 encoding: The file encoding to use.
 sep: The separator to use when joining data.
 ⁰
 def split(
 self,
 encoding: typing.Any | None = None,
 keepends: bool = False) -> list[str]: View Source
-333    def split(self, encoding: Any | None = None, keepends: bool = False) -
+338    def split(self, encoding: Any | None = None, keepends: bool = False) -
 > list[str]:
-334        """Returns the content of the pointed at file as a list of strings,
+339        """Returns the content of the pointed at file as a list of strings,
 splitting at new line characters.
-335
-336        Equivalent to `Pathier("somefile.txt").read_text
+340
+341        Equivalent to `Pathier("somefile.txt").read_text
 (encoding=encoding).splitlines()`
-337
-338        #### :params:
-339
-340        `encoding`: The file encoding to use.
-341
-342        `keepend`: If `True`, line breaks will be included in returned
+342
+343        #### :params:
+344
+345        `encoding`: The file encoding to use.
+346
+347        `keepend`: If `True`, line breaks will be included in returned
 strings."""
-343        return self.read_text(encoding=encoding).splitlines(keepends)
+348        return self.read_text(encoding=encoding).splitlines(keepends)
 Returns the content of the pointed at file as a list of strings, splitting at
 new line characters.
 Equivalent to Pathier("somefile.txt").read_text(encoding=encoding).splitlines()
 *** :params: ***
 encoding: The file encoding to use.
 keepend: If True, line breaks will be included in returned strings.
 ⁰
 def json_loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-345    def json_loads(self, encoding: Any | None = None, errors: Any | None =
+350    def json_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-346        """Load json file."""
-347        return json.loads(self.read_text(encoding, errors))
+351        """Load json file."""
+352        return json.loads(self.read_text(encoding, errors))
 Load json file.
 ⁰
 def json_dumps(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 sort_keys: bool = False,
 indent: typing.Any | None = None,
 default: typing.Any | None = None,
 parents: bool = True) -> Any: View Source
-349    def json_dumps(
-350        self,
-351        data: Any,
-352        encoding: Any | None = None,
-353        errors: Any | None = None,
-354        newline: Any | None = None,
-355        sort_keys: bool = False,
-356        indent: Any | None = None,
-357        default: Any | None = None,
-358        parents: bool = True,
-359    ) -> Any:
-360        """Dump `data` to json file."""
-361        self.write_text(
-362            json.dumps(data, indent=indent, default=default,
+354    def json_dumps(
+355        self,
+356        data: Any,
+357        encoding: Any | None = None,
+358        errors: Any | None = None,
+359        newline: Any | None = None,
+360        sort_keys: bool = False,
+361        indent: Any | None = None,
+362        default: Any | None = None,
+363        parents: bool = True,
+364    ) -> Any:
+365        """Dump `data` to json file."""
+366        self.write_text(
+367            json.dumps(data, indent=indent, default=default,
 sort_keys=sort_keys),
-363            encoding,
-364            errors,
-365            newline,
-366            parents,
-367        )
+368            encoding,
+369            errors,
+370            newline,
+371            parents,
+372        )
 Dump data to json file.
 ⁰
 def toml_loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-369    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
+374    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-370        """Load toml file."""
-371        return tomlkit.loads(self.read_text(encoding, errors)).unwrap()
+375        """Load toml file."""
+376        return tomlkit.loads(self.read_text(encoding, errors)).unwrap()
 Load toml file.
 ⁰
 def toml_dumps(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 sort_keys: bool = False,
 parents: bool = True): View Source
-373    def toml_dumps(
-374        self,
-375        data: Any,
-376        encoding: Any | None = None,
-377        errors: Any | None = None,
-378        newline: Any | None = None,
-379        sort_keys: bool = False,
-380        parents: bool = True,
-381    ):
-382        """Dump `data` to toml file."""
-383        self.write_text(
-384            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
+378    def toml_dumps(
+379        self,
+380        data: Any,
+381        encoding: Any | None = None,
+382        errors: Any | None = None,
+383        newline: Any | None = None,
+384        sort_keys: bool = False,
+385        parents: bool = True,
+386    ):
+387        """Dump `data` to toml file."""
+388        self.write_text(
+389            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
 parents
-385        )
+390        )
 Dump data to toml file.
 ⁰
 def loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-387    def loads(self, encoding: Any | None = None, errors: Any | None = None)
+392    def loads(self, encoding: Any | None = None, errors: Any | None = None)
 -> Any:
-388        """Load a json or toml file based off this instance's suffix."""
-389        match self.suffix:
-390            case ".json":
-391                return self.json_loads(encoding, errors)
-392            case ".toml":
-393                return self.toml_loads(encoding, errors)
+393        """Load a json or toml file based off this instance's suffix."""
+394        match self.suffix:
+395            case ".json":
+396                return self.json_loads(encoding, errors)
+397            case ".toml":
+398                return self.toml_loads(encoding, errors)
 Load a json or toml file based off this instance's suffix.
 ⁰
 def dumps(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 sort_keys: bool = False,
 indent: typing.Any | None = None,
 default: typing.Any | None = None,
 parents: bool = True): View Source
-395    def dumps(
-396        self,
-397        data: Any,
-398        encoding: Any | None = None,
-399        errors: Any | None = None,
-400        newline: Any | None = None,
-401        sort_keys: bool = False,
-402        indent: Any | None = None,
-403        default: Any | None = None,
-404        parents: bool = True,
-405    ):
-406        """Dump `data` to a json or toml file based off this instance's
+400    def dumps(
+401        self,
+402        data: Any,
+403        encoding: Any | None = None,
+404        errors: Any | None = None,
+405        newline: Any | None = None,
+406        sort_keys: bool = False,
+407        indent: Any | None = None,
+408        default: Any | None = None,
+409        parents: bool = True,
+410    ):
+411        """Dump `data` to a json or toml file based off this instance's
 suffix."""
-407        match self.suffix:
-408            case ".json":
-409                self.json_dumps(
-410                    data, encoding, errors, newline, sort_keys, indent,
+412        match self.suffix:
+413            case ".json":
+414                self.json_dumps(
+415                    data, encoding, errors, newline, sort_keys, indent,
 default, parents
-411                )
-412            case ".toml":
-413                self.toml_dumps(data, encoding, errors, newline, sort_keys,
+416                )
+417            case ".toml":
+418                self.toml_dumps(data, encoding, errors, newline, sort_keys,
 parents)
 Dump data to a json or toml file based off this instance's suffix.
 ⁰
 def delete(self, missing_ok: bool = True): View Source
-415    def delete(self, missing_ok: bool = True):
-416        """Delete the file or folder pointed to by this instance.
-417
-418        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a
+420    def delete(self, missing_ok: bool = True):
+421        """Delete the file or folder pointed to by this instance.
+422
+423        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a
 directory."""
-419        if self.is_file():
-420            self.unlink(missing_ok)
-421        elif self.is_dir():
-422            shutil.rmtree(self)
+424        if self.is_file():
+425            self.unlink(missing_ok)
+426        elif self.is_dir():
+427            shutil.rmtree(self)
 Delete the file or folder pointed to by this instance.
 Uses self.unlink() if a file and uses shutil.rmtree() if a directory.
 ⁰
 def copy(
 self,
 new_path: Union[Self, pathlib.Path, str],
 overwrite: bool = False) -> Self: View Source
-424    def copy(
-425        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
-426    ) -> Self:
-427        """Copy the path pointed to by this instance
-428        to the instance pointed to by `new_path` using `shutil.copyfile`
-429        or `shutil.copytree`.
-430
-431        Returns the new path.
-432
-433        #### :params:
-434
-435        `new_path`: The copy destination.
-436
-437        `overwrite`: If `True`, files already existing in `new_path` will be
+429    def copy(
+430        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
+431    ) -> Self:
+432        """Copy the path pointed to by this instance
+433        to the instance pointed to by `new_path` using `shutil.copyfile`
+434        or `shutil.copytree`.
+435
+436        Returns the new path.
+437
+438        #### :params:
+439
+440        `new_path`: The copy destination.
+441
+442        `overwrite`: If `True`, files already existing in `new_path` will be
 overwritten.
-438        If `False`, only files that don't exist in `new_path` will be
+443        If `False`, only files that don't exist in `new_path` will be
 copied."""
-439        new_path = Pathier(new_path)
-440        if self.is_dir():
-441            if overwrite or not new_path.exists():
-442                shutil.copytree(self, new_path, dirs_exist_ok=True)
-443            else:
-444                files = self.rglob("*.*")
-445                for file in files:
-446                    dst = new_path.with_name(file.name)
-447                    if not dst.exists():
-448                        shutil.copyfile(file, dst)
-449        elif self.is_file():
-450            if overwrite or not new_path.exists():
-451                shutil.copyfile(self, new_path)
-452        return new_path
+444        new_path = Pathier(new_path)
+445        if self.is_dir():
+446            if overwrite or not new_path.exists():
+447                shutil.copytree(self, new_path, dirs_exist_ok=True)
+448            else:
+449                files = self.rglob("*.*")
+450                for file in files:
+451                    dst = new_path.with_name(file.name)
+452                    if not dst.exists():
+453                        shutil.copyfile(file, dst)
+454        elif self.is_file():
+455            if overwrite or not new_path.exists():
+456                shutil.copyfile(self, new_path)
+457        return new_path
 Copy the path pointed to by this instance to the instance pointed to by
 new_path using shutil.copyfile or shutil.copytree.
 Returns the new path.
 *** :params: ***
 new_path: The copy destination.
 overwrite: If True, files already existing in new_path will be overwritten. If
 False, only files that don't exist in new_path will be copied.
 ⁰
 def backup(self, timestamp: bool = False) -> Optional[Self]: View Source
-454    def backup(self, timestamp: bool = False) -> Self | None:
-455        """Create a copy of this file or directory with `_backup` appended
+459    def backup(self, timestamp: bool = False) -> Self | None:
+460        """Create a copy of this file or directory with `_backup` appended
 to the path stem.
-456        If the path to be backed up doesn't exist, `None` is returned.
-457        Otherwise a `Pathier` object for the backup is returned.
-458
-459        #### :params:
-460
-461        `timestamp`: Add a timestamp to the backup name to prevent
+461        If the path to be backed up doesn't exist, `None` is returned.
+462        Otherwise a `Pathier` object for the backup is returned.
+463
+464        #### :params:
+465
+466        `timestamp`: Add a timestamp to the backup name to prevent
 overriding previous backups.
-462
-463        >>> path = Pathier("some_file.txt")
-464        >>> path.backup()
-465        >>> list(path.iterdir())
-466        >>> ['some_file.txt', 'some_file_backup.txt']
-467        >>> path.backup(True)
-468        >>> list(path.iterdir())
-469        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
+467
+468        >>> path = Pathier("some_file.txt")
+469        >>> path.backup()
+470        >>> list(path.iterdir())
+471        >>> ['some_file.txt', 'some_file_backup.txt']
+472        >>> path.backup(True)
+473        >>> list(path.iterdir())
+474        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
 28-2023-06_25_52_PM.txt']"""
-470        if not self.exists():
-471            return None
-472        backup_stem = f"{self.stem}_backup"
-473        if timestamp:
-474            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
+475        if not self.exists():
+476            return None
+477        backup_stem = f"{self.stem}_backup"
+478        if timestamp:
+479            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
 ('%m-%d-%Y-%I_%M_%S_%p')}"
-475        backup_path = self.with_stem(backup_stem)
-476        self.copy(backup_path, True)
-477        return backup_path
+480        backup_path = self.with_stem(backup_stem)
+481        self.copy(backup_path, True)
+482        return backup_path
 Create a copy of this file or directory with _backup appended to the path stem.
 If the path to be backed up doesn't exist, None is returned. Otherwise a
 Pathier object for the backup is returned.
 *** :params: ***
 timestamp: Add a timestamp to the backup name to prevent overriding previous
 backups.
 >>> path = Pathier("some_file.txt")
@@ -1232,33 +1241,33 @@
 >>> ['some_file.txt', 'some_file_backup.txt']
 >>> path.backup(True)
 >>> list(path.iterdir())
 >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-28-2023-
 06_25_52_PM.txt']
 ⁰
 def execute(self, command: str = '', args: str = '') -> int: View Source
-479    def execute(self, command: str = "", args: str = "") -> int:
-480        """Make a call to `os.system` using the path pointed to by this
+484    def execute(self, command: str = "", args: str = "") -> int:
+485        """Make a call to `os.system` using the path pointed to by this
 Pathier object.
-481
-482        #### :params:
-483
-484        `command`: Program/command to precede the path with.
-485
-486        `args`: Any arguments that should come after the path.
-487
-488        :returns: The integer output of `os.system`.
-489
-490        e.g.
-491        >>> path = Pathier("mydirectory") / "myscript.py"
-492        then
-493        >>> path.execute("py", "--iterations 10")
-494        equivalent to
-495        >>> os.system(f"py {path} --iterations 10")"""
-496        return os.system(f"{command} {self} {args}")
+486
+487        #### :params:
+488
+489        `command`: Program/command to precede the path with.
+490
+491        `args`: Any arguments that should come after the path.
+492
+493        :returns: The integer output of `os.system`.
+494
+495        e.g.
+496        >>> path = Pathier("mydirectory") / "myscript.py"
+497        then
+498        >>> path.execute("py", "--iterations 10")
+499        equivalent to
+500        >>> os.system(f"py {path} --iterations 10")"""
+501        return os.system(f"{command} {self} {args}")
 Make a call to os.system using the path pointed to by this Pathier object.
 *** :params: ***
 command: Program/command to precede the path with.
 args: Any arguments that should come after the path.
 :returns: The integer output of os.system.
 e.g.
 >>> path = Pathier("mydirectory") / "myscript.py"
```

### Comparing `pathier-1.0.0/docs/search.js` & `pathier-1.1.0/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -747,14 +747,21 @@
         "fullname": "pathier.Pathier.size",
         "modulename": "pathier",
         "qualname": "Pathier.size",
         "kind": "variable",
         "doc": "<p>Returns the size in bytes of this file or directory.</p>\n\n<p>If this path doesn't exist, <code>0</code> will be returned.</p>\n",
         "annotation": ": int"
     }, {
+        "fullname": "pathier.Pathier.formatted_size",
+        "modulename": "pathier",
+        "qualname": "Pathier.formatted_size",
+        "kind": "variable",
+        "doc": "<p>The size of this file or directory formatted with <code>self.format_bytes()</code>.</p>\n",
+        "annotation": ": str"
+    }, {
         "fullname": "pathier.Pathier.format_bytes",
         "modulename": "pathier",
         "qualname": "Pathier.format_bytes",
         "kind": "function",
         "doc": "<p>Format <code>size</code> with common file size abbreviations and rounded to two decimal places.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"mi\">1234</span> <span class=\"o\">-&gt;</span> <span class=\"s2\">&quot;1.23 kb&quot;</span>\n</code></pre>\n</div>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">size</span><span class=\"p\">:</span> <span class=\"nb\">int</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
```

### Comparing `pathier-1.0.0/src/pathier/pathier.py` & `pathier-1.1.0/src/pathier/pathier.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,19 @@
             return 0
         elif self.is_file():
             return self.stat().st_size
         elif self.is_dir():
             return sum(file.stat().st_size for file in self.rglob("*.*"))
         return 0
 
+    @property
+    def formatted_size(self) -> str:
+        """The size of this file or directory formatted with `self.format_bytes()`."""
+        return self.format_bytes(self.size)
+
     @staticmethod
     def format_bytes(size: int) -> str:
         """Format `size` with common file size abbreviations and rounded to two decimal places.
         >>> 1234 -> "1.23 kb" """
         for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
             if unit != "bytes":
                 size *= 0.001
```

### Comparing `pathier-1.0.0/LICENSE.txt` & `pathier-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathier-1.0.0/README.md` & `pathier-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,16 @@
 datetime.datetime(2023, 3, 31, 21, 7, 30)
 >>> p.mod_delta
 207.488857
 >>> p.size
 10744
 >>> p.format_bytes(p.size)
 '10.74 kb'
+>>> p.formatted_size
+'10.74 kb'
 >>> p.is_larger(i)
 True
 >>> p.is_older(i)
 False
 >>> p.modified_more_recently(i)
 True
 </pre>
```

### Comparing `pathier-1.0.0/pyproject.toml` & `pathier-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathier"
 description = "Extends the standard library pathlib.Path class."
-version = "1.0.0"
+version = "1.1.0"
 requires-python = ">=3.10"
 dependencies = ["tomlkit>=0.11.8", "pytest", "typing_extensions"]
 readme = "README.md"
 keywords = ["pathlib", "path", "json", "toml", "shutil", "extender", "extension"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 
 [[project.authors]]
```

### Comparing `pathier-1.0.0/PKG-INFO` & `pathier-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathier
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extends the standard library pathlib.Path class.
 Project-URL: Homepage, https://github.com/matt-manes/pathier
 Project-URL: Documentation, https://github.com/matt-manes/pathier/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/pathier/tree/main/src/pathier
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: extender,extension,json,path,pathlib,shutil,toml
@@ -133,14 +133,16 @@
 datetime.datetime(2023, 3, 31, 21, 7, 30)
 >>> p.mod_delta
 207.488857
 >>> p.size
 10744
 >>> p.format_bytes(p.size)
 '10.74 kb'
+>>> p.formatted_size
+'10.74 kb'
 >>> p.is_larger(i)
 True
 >>> p.is_older(i)
 False
 >>> p.modified_more_recently(i)
 True
 </pre>
```

