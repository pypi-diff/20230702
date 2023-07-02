# Comparing `tmp/packagelister-1.6.1.tar.gz` & `tmp/packagelister-1.6.2.tar.gz`

## Comparing `packagelister-1.6.1.tar` & `packagelister-1.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 packagelister-1.6.1/CHANGELOG.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/index.html
--rw-r--r--   0        0        0    34336 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister.html
--rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/search.js
--rw-r--r--   0        0        0    79722 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister/packagelister.html
--rw-r--r--   0        0        0    77472 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister/packagelister_cli.html
--rw-r--r--   0        0        0    56429 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister/whouses.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/__init__.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/packagelister.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/packagelister_cli.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/whouses.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.6.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.6.1/LICENSE.txt
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.6.1/README.md
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 packagelister-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 packagelister-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 packagelister-1.6.2/CHANGELOG.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.6.2/docs/index.html
+-rw-r--r--   0        0        0    34336 2020-02-02 00:00:00.000000 packagelister-1.6.2/docs/packagelister.html
+-rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 packagelister-1.6.2/docs/search.js
+-rw-r--r--   0        0        0    79722 2020-02-02 00:00:00.000000 packagelister-1.6.2/docs/packagelister/packagelister.html
+-rw-r--r--   0        0        0    77472 2020-02-02 00:00:00.000000 packagelister-1.6.2/docs/packagelister/packagelister_cli.html
+-rw-r--r--   0        0        0    63213 2020-02-02 00:00:00.000000 packagelister-1.6.2/docs/packagelister/whouses.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 packagelister-1.6.2/src/packagelister/__init__.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 packagelister-1.6.2/src/packagelister/packagelister.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 packagelister-1.6.2/src/packagelister/packagelister_cli.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 packagelister-1.6.2/src/packagelister/whouses.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.6.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.6.2/LICENSE.txt
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.6.2/README.md
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 packagelister-1.6.2/PKG-INFO
```

### Comparing `packagelister-1.6.1/CHANGELOG.md` & `packagelister-1.6.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v1.6.1 (2023-06-10)
+
+#### Fixes
+
+* cli no longer lists the package being scanned in the results
+#### Performance improvements
+
+* remove redundant list sort
+
+
 ## v1.6.0 (2023-06-10)
 
 #### New Features
 
 * replace package names with pip name when they don't match when generating requirements
 #### Fixes
```

### Comparing `packagelister-1.6.1/docs/packagelister.html` & `packagelister-1.6.2/docs/packagelister.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/docs/search.js` & `packagelister-1.6.2/docs/search.js`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/docs/packagelister/packagelister.html` & `packagelister-1.6.2/docs/packagelister/packagelister.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/docs/packagelister/packagelister_cli.html` & `packagelister-1.6.2/docs/packagelister/packagelister_cli.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/docs/packagelister/whouses.html` & `packagelister-1.6.2/docs/packagelister/whouses.html`

 * *Files 18% similar despite different names*

```diff
@@ -88,31 +88,45 @@
 </span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>
 </span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>    <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>
 </span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>
 </span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a><span class="k">def</span> <span class="nf">find</span><span class="p">(</span><span class="n">root</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">package</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">ignore</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="sd">&quot;&quot;&quot;Find what sub-folders of `root`, excluding those in `ignore`, have files that use `package`.&quot;&quot;&quot;</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">package_users</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="k">for</span> <span class="n">project</span> <span class="ow">in</span> <span class="n">root</span><span class="o">.</span><span class="n">iterdir</span><span class="p">():</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>        <span class="k">if</span> <span class="n">project</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()</span> <span class="ow">and</span> <span class="n">project</span><span class="o">.</span><span class="n">stem</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">ignore</span><span class="p">:</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>            <span class="k">if</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">scan</span><span class="p">(</span><span class="n">project</span><span class="p">):</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>                <span class="n">package_users</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">project</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>    <span class="k">return</span> <span class="n">package_users</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="n">package_users</span> <span class="o">=</span> <span class="n">find</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">(),</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">ignore</span><span class="p">)</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following folders have files that use </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">package_users</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>
-</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="n">scan_fails</span> <span class="o">=</span> <span class="p">{}</span>  <span class="c1"># Error message: [projects]</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="k">for</span> <span class="n">project</span> <span class="ow">in</span> <span class="n">root</span><span class="o">.</span><span class="n">iterdir</span><span class="p">():</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>        <span class="k">if</span> <span class="n">project</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()</span> <span class="ow">and</span> <span class="n">project</span><span class="o">.</span><span class="n">stem</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">ignore</span><span class="p">:</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>                <span class="k">if</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">scan</span><span class="p">(</span><span class="n">project</span><span class="p">):</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>                    <span class="n">package_users</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">project</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>                <span class="n">err</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>                <span class="k">if</span> <span class="n">err</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">scan_fails</span><span class="p">:</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>                    <span class="n">scan_fails</span><span class="p">[</span><span class="n">err</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">project</span><span class="p">]</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>                    <span class="n">scan_fails</span><span class="p">[</span><span class="n">err</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">project</span><span class="p">)</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following errors occured during the scan:&quot;</span><span class="p">)</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">scan_fails</span><span class="p">:</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">fail</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>        <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">scan_fails</span><span class="p">[</span><span class="n">fail</span><span class="p">],</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>    <span class="k">return</span> <span class="n">package_users</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a>
+</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>
+</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos">55</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos">56</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos">57</span></a>    <span class="n">package_users</span> <span class="o">=</span> <span class="n">find</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">(),</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">ignore</span><span class="p">)</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos">58</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following folders have files that use </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos">59</span></a>    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">package_users</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos">60</span></a>
+</span><span id="L-61"><a href="#L-61"><span class="linenos">61</span></a>
+</span><span id="L-62"><a href="#L-62"><span class="linenos">62</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos">63</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -160,19 +174,33 @@
                 <label class="view-source-button" for="find-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#find"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="find-31"><a href="#find-31"><span class="linenos">31</span></a><span class="k">def</span> <span class="nf">find</span><span class="p">(</span><span class="n">root</span><span class="p">:</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">package</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">ignore</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="find-32"><a href="#find-32"><span class="linenos">32</span></a>    <span class="sd">&quot;&quot;&quot;Find what sub-folders of `root`, excluding those in `ignore`, have files that use `package`.&quot;&quot;&quot;</span>
 </span><span id="find-33"><a href="#find-33"><span class="linenos">33</span></a>    <span class="n">package_users</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="find-34"><a href="#find-34"><span class="linenos">34</span></a>    <span class="k">for</span> <span class="n">project</span> <span class="ow">in</span> <span class="n">root</span><span class="o">.</span><span class="n">iterdir</span><span class="p">():</span>
-</span><span id="find-35"><a href="#find-35"><span class="linenos">35</span></a>        <span class="k">if</span> <span class="n">project</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()</span> <span class="ow">and</span> <span class="n">project</span><span class="o">.</span><span class="n">stem</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">ignore</span><span class="p">:</span>
-</span><span id="find-36"><a href="#find-36"><span class="linenos">36</span></a>            <span class="k">if</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">scan</span><span class="p">(</span><span class="n">project</span><span class="p">):</span>
-</span><span id="find-37"><a href="#find-37"><span class="linenos">37</span></a>                <span class="n">package_users</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">project</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="find-38"><a href="#find-38"><span class="linenos">38</span></a>    <span class="k">return</span> <span class="n">package_users</span>
+</span><span id="find-34"><a href="#find-34"><span class="linenos">34</span></a>    <span class="n">scan_fails</span> <span class="o">=</span> <span class="p">{}</span>  <span class="c1"># Error message: [projects]</span>
+</span><span id="find-35"><a href="#find-35"><span class="linenos">35</span></a>    <span class="k">for</span> <span class="n">project</span> <span class="ow">in</span> <span class="n">root</span><span class="o">.</span><span class="n">iterdir</span><span class="p">():</span>
+</span><span id="find-36"><a href="#find-36"><span class="linenos">36</span></a>        <span class="k">if</span> <span class="n">project</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()</span> <span class="ow">and</span> <span class="n">project</span><span class="o">.</span><span class="n">stem</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">ignore</span><span class="p">:</span>
+</span><span id="find-37"><a href="#find-37"><span class="linenos">37</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="find-38"><a href="#find-38"><span class="linenos">38</span></a>                <span class="k">if</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">scan</span><span class="p">(</span><span class="n">project</span><span class="p">):</span>
+</span><span id="find-39"><a href="#find-39"><span class="linenos">39</span></a>                    <span class="n">package_users</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">project</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="find-40"><a href="#find-40"><span class="linenos">40</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="find-41"><a href="#find-41"><span class="linenos">41</span></a>                <span class="n">err</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="find-42"><a href="#find-42"><span class="linenos">42</span></a>                <span class="k">if</span> <span class="n">err</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">scan_fails</span><span class="p">:</span>
+</span><span id="find-43"><a href="#find-43"><span class="linenos">43</span></a>                    <span class="n">scan_fails</span><span class="p">[</span><span class="n">err</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">project</span><span class="p">]</span>
+</span><span id="find-44"><a href="#find-44"><span class="linenos">44</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="find-45"><a href="#find-45"><span class="linenos">45</span></a>                    <span class="n">scan_fails</span><span class="p">[</span><span class="n">err</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">project</span><span class="p">)</span>
+</span><span id="find-46"><a href="#find-46"><span class="linenos">46</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="find-47"><a href="#find-47"><span class="linenos">47</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The following errors occured during the scan:&quot;</span><span class="p">)</span>
+</span><span id="find-48"><a href="#find-48"><span class="linenos">48</span></a>    <span class="k">for</span> <span class="n">fail</span> <span class="ow">in</span> <span class="n">scan_fails</span><span class="p">:</span>
+</span><span id="find-49"><a href="#find-49"><span class="linenos">49</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">fail</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="find-50"><a href="#find-50"><span class="linenos">50</span></a>        <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">scan_fails</span><span class="p">[</span><span class="n">fail</span><span class="p">],</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="find-51"><a href="#find-51"><span class="linenos">51</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="find-52"><a href="#find-52"><span class="linenos">52</span></a>    <span class="k">return</span> <span class="n">package_users</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Find what sub-folders of <code>root</code>, excluding those in <code>ignore</code>, have files that use <code>package</code>.</p>
 </div>
 
 
@@ -184,20 +212,20 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-41"><a href="#main-41"><span class="linenos">41</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-42"><a href="#main-42"><span class="linenos">42</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-43"><a href="#main-43"><span class="linenos">43</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a>    <span class="n">package_users</span> <span class="o">=</span> <span class="n">find</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">(),</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">ignore</span><span class="p">)</span>
-</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following folders have files that use </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
-</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">package_users</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-55"><a href="#main-55"><span class="linenos">55</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-56"><a href="#main-56"><span class="linenos">56</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-57"><a href="#main-57"><span class="linenos">57</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-58"><a href="#main-58"><span class="linenos">58</span></a>    <span class="n">package_users</span> <span class="o">=</span> <span class="n">find</span><span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">(),</span> <span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">ignore</span><span class="p">)</span>
+</span><span id="main-59"><a href="#main-59"><span class="linenos">59</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The following folders have files that use </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">package</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="main-60"><a href="#main-60"><span class="linenos">60</span></a>    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">package_users</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -40,31 +40,45 @@
 27    return args
 28
 29
 30def find(root: Pathier, package: str, ignore: list[str] = []) -> list[str]:
 31    """Find what sub-folders of `root`, excluding those in `ignore`, have
 files that use `package`."""
 32    package_users = []
-33    for project in root.iterdir():
-34        if project.is_dir() and project.stem not in ignore:
-35            if package in scan(project):
-36                package_users.append(project.stem)
-37    return package_users
-38
-39
-40def main(args: argparse.Namespace = None):
-41    if not args:
-42        args = get_args()
-43    package_users = find(Pathier.cwd(), args.package, args.ignore)
-44    print(f"The following folders have files that use {args.package}:")
-45    print(*package_users, sep="\n")
-46
-47
-48if __name__ == "__main__":
-49    main(get_args())
+33    scan_fails = {}  # Error message: [projects]
+34    for project in root.iterdir():
+35        if project.is_dir() and project.stem not in ignore:
+36            try:
+37                if package in scan(project):
+38                    package_users.append(project.stem)
+39            except Exception as e:
+40                err = str(e)
+41                if err not in scan_fails:
+42                    scan_fails[err] = [project]
+43                else:
+44                    scan_fails[err].append(project)
+45    print()
+46    print("The following errors occured during the scan:")
+47    for fail in scan_fails:
+48        print(f"ERROR: {fail}:")
+49        print(*scan_fails[fail], sep="\n")
+50        print()
+51    return package_users
+52
+53
+54def main(args: argparse.Namespace = None):
+55    if not args:
+56        args = get_args()
+57    package_users = find(Pathier.cwd(), args.package, args.ignore)
+58    print(f"The following folders have files that use {args.package}:")
+59    print(*package_users, sep="\n")
+60
+61
+62if __name__ == "__main__":
+63    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
 _9def get_args() -> argparse.Namespace:
 10    parser = argparse.ArgumentParser()
 11
 12    parser.add_argument(
 13        "package",
@@ -89,23 +103,37 @@
 root: pathier.pathier.Pathier,
 package: str,
 ignore: list[str] = []) -> list[str]: View Source
 31def find(root: Pathier, package: str, ignore: list[str] = []) -> list[str]:
 32    """Find what sub-folders of `root`, excluding those in `ignore`, have
 files that use `package`."""
 33    package_users = []
-34    for project in root.iterdir():
-35        if project.is_dir() and project.stem not in ignore:
-36            if package in scan(project):
-37                package_users.append(project.stem)
-38    return package_users
+34    scan_fails = {}  # Error message: [projects]
+35    for project in root.iterdir():
+36        if project.is_dir() and project.stem not in ignore:
+37            try:
+38                if package in scan(project):
+39                    package_users.append(project.stem)
+40            except Exception as e:
+41                err = str(e)
+42                if err not in scan_fails:
+43                    scan_fails[err] = [project]
+44                else:
+45                    scan_fails[err].append(project)
+46    print()
+47    print("The following errors occured during the scan:")
+48    for fail in scan_fails:
+49        print(f"ERROR: {fail}:")
+50        print(*scan_fails[fail], sep="\n")
+51        print()
+52    return package_users
 Find what sub-folders of root, excluding those in ignore, have files that use
 package.
   ⁰
 def main(args: argparse.Namespace = None): View Source
-41def main(args: argparse.Namespace = None):
-42    if not args:
-43        args = get_args()
-44    package_users = find(Pathier.cwd(), args.package, args.ignore)
-45    print(f"The following folders have files that use {args.package}:")
-46    print(*package_users, sep="\n")
+55def main(args: argparse.Namespace = None):
+56    if not args:
+57        args = get_args()
+58    package_users = find(Pathier.cwd(), args.package, args.ignore)
+59    print(f"The following folders have files that use {args.package}:")
+60    print(*package_users, sep="\n")
```

### Comparing `packagelister-1.6.1/src/packagelister/packagelister.py` & `packagelister-1.6.2/src/packagelister/packagelister.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/src/packagelister/packagelister_cli.py` & `packagelister-1.6.2/src/packagelister/packagelister_cli.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/src/packagelister/whouses.py` & `packagelister-1.6.2/src/packagelister/whouses.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,18 +26,32 @@
 
     return args
 
 
 def find(root: Pathier, package: str, ignore: list[str] = []) -> list[str]:
     """Find what sub-folders of `root`, excluding those in `ignore`, have files that use `package`."""
     package_users = []
+    scan_fails = {}  # Error message: [projects]
     for project in root.iterdir():
         if project.is_dir() and project.stem not in ignore:
-            if package in scan(project):
-                package_users.append(project.stem)
+            try:
+                if package in scan(project):
+                    package_users.append(project.stem)
+            except Exception as e:
+                err = str(e)
+                if err not in scan_fails:
+                    scan_fails[err] = [project]
+                else:
+                    scan_fails[err].append(project)
+    print()
+    print("The following errors occured during the scan:")
+    for fail in scan_fails:
+        print(f"ERROR: {fail}:")
+        print(*scan_fails[fail], sep="\n")
+        print()
     return package_users
 
 
 def main(args: argparse.Namespace = None):
     if not args:
         args = get_args()
     package_users = find(Pathier.cwd(), args.package, args.ignore)
```

### Comparing `packagelister-1.6.1/LICENSE.txt` & `packagelister-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/README.md` & `packagelister-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.1/PKG-INFO` & `packagelister-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagelister
-Version: 1.6.1
+Version: 1.6.2
 Summary: Determine what 3rd-party packages a project imports.
 Project-URL: Homepage, https://github.com/matt-manes/packagelister
 Project-URL: Documentation, https://github.com/matt-manes/packagelister/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/packagelister/tree/main/src/packagelister
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: import,module,package
```

