# Comparing `tmp/pathier-0.9.0.tar.gz` & `tmp/pathier-1.0.0.tar.gz`

## Comparing `pathier-0.9.0.tar` & `pathier-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 pathier-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-0.9.0/docs/index.html
--rw-r--r--   0        0        0   240044 2020-02-02 00:00:00.000000 pathier-0.9.0/docs/pathier.html
--rw-r--r--   0        0        0    48466 2020-02-02 00:00:00.000000 pathier-0.9.0/docs/search.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pathier-0.9.0/src/pathier/__init__.py
--rw-r--r--   0        0        0    14056 2020-02-02 00:00:00.000000 pathier-0.9.0/src/pathier/pathier.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-0.9.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pathier-0.9.0/README.md
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pathier-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 pathier-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 pathier-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-1.0.0/docs/index.html
+-rw-r--r--   0        0        0   299385 2020-02-02 00:00:00.000000 pathier-1.0.0/docs/pathier.html
+-rw-r--r--   0        0        0    61206 2020-02-02 00:00:00.000000 pathier-1.0.0/docs/search.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.0.0/src/pathier/__init__.py
+-rw-r--r--   0        0        0    18994 2020-02-02 00:00:00.000000 pathier-1.0.0/src/pathier/pathier.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 pathier-1.0.0/README.md
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pathier-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 pathier-1.0.0/PKG-INFO
```

### Comparing `pathier-0.9.0/CHANGELOG.md` & `pathier-1.0.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,90 @@
 # Changelog
 
-## 0.8.0 (2023-04-15)
+## v0.14.1 (2023-06-21)
+
+#### Performance improvements
+
+* toml files will have their datatypes converted to python types when loaded
+#### Others
+
+* specify minimum tomlkit version
+## v0.14.0 (2023-06-10)
+
+#### New Features
+
+* add type aliases for `Pathier | pathlib.Path` and `Pathier | pathlib.Path | str`
+## v0.13.0 (2023-06-01)
+
+#### Refactorings
+
+* size() returns 0 for non-existent files instead of None
+
+## v0.12.0 (2023-05-26)
+
+#### New Features
+
+* add `keepends` parameter to split function
+* add `sep` parameter to join function
+* add properties to track last read vs last modified times
+#### Others
+
+
+
+## v0.11.0 (2023-04-29)
+
+#### New Features
+
+* add join and split methods
+* add append method
+#### Docs
+
+* update readme
+
+
+## v0.10.0 (2023-04-29)
+
+#### New Features
+
+* add replace function
+* add execute function
+#### Docs
+
+* update readme
+* improve doc string formatting
+#### Others
+
+* build v0.10.0
+* update changelog
+* remove unused import
+
+
+## v0.9.0 (2023-04-28)
+
+#### New Features
+
+* add backup function
+#### Others
+
+* build v0.9.0
+* update changelog
+
+
+## v0.8.0 (2023-04-15)
 
 #### New Features
 
 * wrap importing typing.Self in try/except to accomodate python 3.10
 #### Refactorings
 
 * import Self from typing_extensions
 #### Others
 
+* build v0.8.0
+* update changelog
 * remove uneeded dependency
 * set requires-python to >=3.10
 * build v0.7.0
 * remove uneeded dependency
 
 
 ## v0.7.0 (2023-04-11)
```

### Comparing `pathier-0.9.0/docs/pathier.html` & `pathier-1.0.0/docs/pathier.html`

 * *Files 8% similar despite different names*

```diff
@@ -38,18 +38,24 @@
                         <li>
                                 <a class="variable" href="#Pathier.mod_date">mod_date</a>
                         </li>
                         <li>
                                 <a class="variable" href="#Pathier.mod_delta">mod_delta</a>
                         </li>
                         <li>
-                                <a class="function" href="#Pathier.size">size</a>
+                                <a class="variable" href="#Pathier.last_read_time">last_read_time</a>
                         </li>
                         <li>
-                                <a class="function" href="#Pathier.format_size">format_size</a>
+                                <a class="variable" href="#Pathier.modified_since_last_read">modified_since_last_read</a>
+                        </li>
+                        <li>
+                                <a class="variable" href="#Pathier.size">size</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#Pathier.format_bytes">format_bytes</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.is_larger">is_larger</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.is_older">is_older</a>
                         </li>
@@ -83,20 +89,35 @@
                         <li>
                                 <a class="function" href="#Pathier.mkdir">mkdir</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.touch">touch</a>
                         </li>
                         <li>
+                                <a class="function" href="#Pathier.open">open</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#Pathier.write_text">write_text</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.write_bytes">write_bytes</a>
                         </li>
                         <li>
+                                <a class="function" href="#Pathier.append">append</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#Pathier.replace">replace</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#Pathier.join">join</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#Pathier.split">split</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#Pathier.json_loads">json_loads</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.json_dumps">json_dumps</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.toml_loads">toml_loads</a>
@@ -115,17 +136,26 @@
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.copy">copy</a>
                         </li>
                         <li>
                                 <a class="function" href="#Pathier.backup">backup</a>
                         </li>
+                        <li>
+                                <a class="function" href="#Pathier.execute">execute</a>
+                        </li>
                 </ul>
 
             </li>
+            <li>
+                    <a class="variable" href="#Pathy">Pathy</a>
+            </li>
+            <li>
+                    <a class="variable" href="#Pathish">Pathish</a>
+            </li>
     </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
@@ -139,17 +169,17 @@
 pathier    </h1>
 
                 
                         <input id="mod-pathier-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-pathier-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">.pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">.pathier</span> <span class="kn">import</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">Pathish</span><span class="p">,</span> <span class="n">Pathy</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">2</span></a>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">3</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Pathier&quot;</span><span class="p">]</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">3</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Pathier&quot;</span><span class="p">,</span> <span class="s2">&quot;Pathy&quot;</span><span class="p">,</span> <span class="s2">&quot;Pathish&quot;</span><span class="p">]</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Pathier">
                             <input id="Pathier-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -173,362 +203,479 @@
 </span><span id="Pathier-25"><a href="#Pathier-25"><span class="linenos"> 25</span></a>                <span class="s2">&quot;cannot instantiate </span><span class="si">%r</span><span class="s2"> on your system&quot;</span> <span class="o">%</span> <span class="p">(</span><span class="bp">cls</span><span class="o">.</span><span class="vm">__name__</span><span class="p">,)</span>
 </span><span id="Pathier-26"><a href="#Pathier-26"><span class="linenos"> 26</span></a>            <span class="p">)</span>
 </span><span id="Pathier-27"><a href="#Pathier-27"><span class="linenos"> 27</span></a>        <span class="k">return</span> <span class="bp">self</span>
 </span><span id="Pathier-28"><a href="#Pathier-28"><span class="linenos"> 28</span></a>
 </span><span id="Pathier-29"><a href="#Pathier-29"><span class="linenos"> 29</span></a>    <span class="c1"># ===============================================stats===============================================</span>
 </span><span id="Pathier-30"><a href="#Pathier-30"><span class="linenos"> 30</span></a>    <span class="nd">@property</span>
 </span><span id="Pathier-31"><a href="#Pathier-31"><span class="linenos"> 31</span></a>    <span class="k">def</span> <span class="nf">dob</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-32"><a href="#Pathier-32"><span class="linenos"> 32</span></a>        <span class="sd">&quot;&quot;&quot;Returns the creation date of this file</span>
-</span><span id="Pathier-33"><a href="#Pathier-33"><span class="linenos"> 33</span></a><span class="sd">        or directory as a dateime.datetime object.&quot;&quot;&quot;</span>
-</span><span id="Pathier-34"><a href="#Pathier-34"><span class="linenos"> 34</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-35"><a href="#Pathier-35"><span class="linenos"> 35</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_ctime</span><span class="p">)</span>
-</span><span id="Pathier-36"><a href="#Pathier-36"><span class="linenos"> 36</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-37"><a href="#Pathier-37"><span class="linenos"> 37</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-38"><a href="#Pathier-38"><span class="linenos"> 38</span></a>
-</span><span id="Pathier-39"><a href="#Pathier-39"><span class="linenos"> 39</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-40"><a href="#Pathier-40"><span class="linenos"> 40</span></a>    <span class="k">def</span> <span class="nf">age</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-41"><a href="#Pathier-41"><span class="linenos"> 41</span></a>        <span class="sd">&quot;&quot;&quot;Returns the age in seconds of this file or directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-42"><a href="#Pathier-42"><span class="linenos"> 42</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-43"><a href="#Pathier-43"><span class="linenos"> 43</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Pathier-44"><a href="#Pathier-44"><span class="linenos"> 44</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-45"><a href="#Pathier-45"><span class="linenos"> 45</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-46"><a href="#Pathier-46"><span class="linenos"> 46</span></a>
-</span><span id="Pathier-47"><a href="#Pathier-47"><span class="linenos"> 47</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-48"><a href="#Pathier-48"><span class="linenos"> 48</span></a>    <span class="k">def</span> <span class="nf">mod_date</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-49"><a href="#Pathier-49"><span class="linenos"> 49</span></a>        <span class="sd">&quot;&quot;&quot;Returns the modification date of this file</span>
-</span><span id="Pathier-50"><a href="#Pathier-50"><span class="linenos"> 50</span></a><span class="sd">        or directory as a datetime.datetime object.&quot;&quot;&quot;</span>
-</span><span id="Pathier-51"><a href="#Pathier-51"><span class="linenos"> 51</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-52"><a href="#Pathier-52"><span class="linenos"> 52</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_mtime</span><span class="p">)</span>
-</span><span id="Pathier-53"><a href="#Pathier-53"><span class="linenos"> 53</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-54"><a href="#Pathier-54"><span class="linenos"> 54</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-55"><a href="#Pathier-55"><span class="linenos"> 55</span></a>
-</span><span id="Pathier-56"><a href="#Pathier-56"><span class="linenos"> 56</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-57"><a href="#Pathier-57"><span class="linenos"> 57</span></a>    <span class="k">def</span> <span class="nf">mod_delta</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-58"><a href="#Pathier-58"><span class="linenos"> 58</span></a>        <span class="sd">&quot;&quot;&quot;Returns how long ago in seconds this file</span>
-</span><span id="Pathier-59"><a href="#Pathier-59"><span class="linenos"> 59</span></a><span class="sd">        or directory was modified.&quot;&quot;&quot;</span>
-</span><span id="Pathier-60"><a href="#Pathier-60"><span class="linenos"> 60</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-61"><a href="#Pathier-61"><span class="linenos"> 61</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
-</span><span id="Pathier-62"><a href="#Pathier-62"><span class="linenos"> 62</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-63"><a href="#Pathier-63"><span class="linenos"> 63</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-64"><a href="#Pathier-64"><span class="linenos"> 64</span></a>
-</span><span id="Pathier-65"><a href="#Pathier-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-66"><a href="#Pathier-66"><span class="linenos"> 66</span></a>        <span class="sd">&quot;&quot;&quot;Returns the size in bytes of this file or directory.</span>
-</span><span id="Pathier-67"><a href="#Pathier-67"><span class="linenos"> 67</span></a><span class="sd">        Returns None if this path doesn&#39;t exist.</span>
-</span><span id="Pathier-68"><a href="#Pathier-68"><span class="linenos"> 68</span></a>
-</span><span id="Pathier-69"><a href="#Pathier-69"><span class="linenos"> 69</span></a><span class="sd">        :param format: If True, return value as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="Pathier-70"><a href="#Pathier-70"><span class="linenos"> 70</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-71"><a href="#Pathier-71"><span class="linenos"> 71</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-72"><a href="#Pathier-72"><span class="linenos"> 72</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-73"><a href="#Pathier-73"><span class="linenos"> 73</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
-</span><span id="Pathier-74"><a href="#Pathier-74"><span class="linenos"> 74</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-75"><a href="#Pathier-75"><span class="linenos"> 75</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="Pathier-76"><a href="#Pathier-76"><span class="linenos"> 76</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
-</span><span id="Pathier-77"><a href="#Pathier-77"><span class="linenos"> 77</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">)</span>
-</span><span id="Pathier-78"><a href="#Pathier-78"><span class="linenos"> 78</span></a>        <span class="k">return</span> <span class="n">size</span>
-</span><span id="Pathier-79"><a href="#Pathier-79"><span class="linenos"> 79</span></a>
-</span><span id="Pathier-80"><a href="#Pathier-80"><span class="linenos"> 80</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Pathier-81"><a href="#Pathier-81"><span class="linenos"> 81</span></a>    <span class="k">def</span> <span class="nf">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Pathier-82"><a href="#Pathier-82"><span class="linenos"> 82</span></a>        <span class="sd">&quot;&quot;&quot;Format &#39;size&#39; with common file size abbreviations</span>
-</span><span id="Pathier-83"><a href="#Pathier-83"><span class="linenos"> 83</span></a><span class="sd">        and rounded to two decimal places.</span>
-</span><span id="Pathier-84"><a href="#Pathier-84"><span class="linenos"> 84</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-85"><a href="#Pathier-85"><span class="linenos"> 85</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
-</span><span id="Pathier-86"><a href="#Pathier-86"><span class="linenos"> 86</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
-</span><span id="Pathier-87"><a href="#Pathier-87"><span class="linenos"> 87</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
-</span><span id="Pathier-88"><a href="#Pathier-88"><span class="linenos"> 88</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
-</span><span id="Pathier-89"><a href="#Pathier-89"><span class="linenos"> 89</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Pathier-90"><a href="#Pathier-90"><span class="linenos"> 90</span></a>
-</span><span id="Pathier-91"><a href="#Pathier-91"><span class="linenos"> 91</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-92"><a href="#Pathier-92"><span class="linenos"> 92</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than</span>
-</span><span id="Pathier-93"><a href="#Pathier-93"><span class="linenos"> 93</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier-94"><a href="#Pathier-94"><span class="linenos"> 94</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="Pathier-95"><a href="#Pathier-95"><span class="linenos"> 95</span></a>
-</span><span id="Pathier-96"><a href="#Pathier-96"><span class="linenos"> 96</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-97"><a href="#Pathier-97"><span class="linenos"> 97</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than</span>
-</span><span id="Pathier-98"><a href="#Pathier-98"><span class="linenos"> 98</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier-99"><a href="#Pathier-99"><span class="linenos"> 99</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
-</span><span id="Pathier-100"><a href="#Pathier-100"><span class="linenos">100</span></a>
-</span><span id="Pathier-101"><a href="#Pathier-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-102"><a href="#Pathier-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified</span>
-</span><span id="Pathier-103"><a href="#Pathier-103"><span class="linenos">103</span></a><span class="sd">        more recently than the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier-104"><a href="#Pathier-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
-</span><span id="Pathier-105"><a href="#Pathier-105"><span class="linenos">105</span></a>
-</span><span id="Pathier-106"><a href="#Pathier-106"><span class="linenos">106</span></a>    <span class="c1"># ===============================================navigation===============================================</span>
-</span><span id="Pathier-107"><a href="#Pathier-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-108"><a href="#Pathier-108"><span class="linenos">108</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-109"><a href="#Pathier-109"><span class="linenos">109</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-110"><a href="#Pathier-110"><span class="linenos">110</span></a>
-</span><span id="Pathier-111"><a href="#Pathier-111"><span class="linenos">111</span></a>    <span class="nd">@property</span>
-</span><span id="Pathier-112"><a href="#Pathier-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">in_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier-113"><a href="#Pathier-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Return True if this</span>
-</span><span id="Pathier-114"><a href="#Pathier-114"><span class="linenos">114</span></a><span class="sd">        path is in sys.path.&quot;&quot;&quot;</span>
-</span><span id="Pathier-115"><a href="#Pathier-115"><span class="linenos">115</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="ow">in</span> <span class="n">sys</span><span class="o">.</span><span class="n">path</span>
-</span><span id="Pathier-116"><a href="#Pathier-116"><span class="linenos">116</span></a>
-</span><span id="Pathier-117"><a href="#Pathier-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
-</span><span id="Pathier-118"><a href="#Pathier-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into sys.path</span>
-</span><span id="Pathier-119"><a href="#Pathier-119"><span class="linenos">119</span></a><span class="sd">        if it isn&#39;t already there.</span>
-</span><span id="Pathier-120"><a href="#Pathier-120"><span class="linenos">120</span></a>
-</span><span id="Pathier-121"><a href="#Pathier-121"><span class="linenos">121</span></a><span class="sd">        :param index: The index of sys.path</span>
-</span><span id="Pathier-122"><a href="#Pathier-122"><span class="linenos">122</span></a><span class="sd">        to insert this path at.&quot;&quot;&quot;</span>
-</span><span id="Pathier-123"><a href="#Pathier-123"><span class="linenos">123</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-124"><a href="#Pathier-124"><span class="linenos">124</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-125"><a href="#Pathier-125"><span class="linenos">125</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
-</span><span id="Pathier-126"><a href="#Pathier-126"><span class="linenos">126</span></a>
-</span><span id="Pathier-127"><a href="#Pathier-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-128"><a href="#Pathier-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to sys.path</span>
-</span><span id="Pathier-129"><a href="#Pathier-129"><span class="linenos">129</span></a><span class="sd">        if it isn&#39;t already there.&quot;&quot;&quot;</span>
-</span><span id="Pathier-130"><a href="#Pathier-130"><span class="linenos">130</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-131"><a href="#Pathier-131"><span class="linenos">131</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-132"><a href="#Pathier-132"><span class="linenos">132</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="Pathier-32"><a href="#Pathier-32"><span class="linenos"> 32</span></a>        <span class="sd">&quot;&quot;&quot;Returns the creation date of this file or directory as a `dateime.datetime` object.&quot;&quot;&quot;</span>
+</span><span id="Pathier-33"><a href="#Pathier-33"><span class="linenos"> 33</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-34"><a href="#Pathier-34"><span class="linenos"> 34</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_ctime</span><span class="p">)</span>
+</span><span id="Pathier-35"><a href="#Pathier-35"><span class="linenos"> 35</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-36"><a href="#Pathier-36"><span class="linenos"> 36</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-37"><a href="#Pathier-37"><span class="linenos"> 37</span></a>
+</span><span id="Pathier-38"><a href="#Pathier-38"><span class="linenos"> 38</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-39"><a href="#Pathier-39"><span class="linenos"> 39</span></a>    <span class="k">def</span> <span class="nf">age</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-40"><a href="#Pathier-40"><span class="linenos"> 40</span></a>        <span class="sd">&quot;&quot;&quot;Returns the age in seconds of this file or directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-41"><a href="#Pathier-41"><span class="linenos"> 41</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-42"><a href="#Pathier-42"><span class="linenos"> 42</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
+</span><span id="Pathier-43"><a href="#Pathier-43"><span class="linenos"> 43</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-44"><a href="#Pathier-44"><span class="linenos"> 44</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-45"><a href="#Pathier-45"><span class="linenos"> 45</span></a>
+</span><span id="Pathier-46"><a href="#Pathier-46"><span class="linenos"> 46</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-47"><a href="#Pathier-47"><span class="linenos"> 47</span></a>    <span class="k">def</span> <span class="nf">mod_date</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-48"><a href="#Pathier-48"><span class="linenos"> 48</span></a>        <span class="sd">&quot;&quot;&quot;Returns the modification date of this file or directory as a `datetime.datetime` object.&quot;&quot;&quot;</span>
+</span><span id="Pathier-49"><a href="#Pathier-49"><span class="linenos"> 49</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-50"><a href="#Pathier-50"><span class="linenos"> 50</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_mtime</span><span class="p">)</span>
+</span><span id="Pathier-51"><a href="#Pathier-51"><span class="linenos"> 51</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-52"><a href="#Pathier-52"><span class="linenos"> 52</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-53"><a href="#Pathier-53"><span class="linenos"> 53</span></a>
+</span><span id="Pathier-54"><a href="#Pathier-54"><span class="linenos"> 54</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-55"><a href="#Pathier-55"><span class="linenos"> 55</span></a>    <span class="k">def</span> <span class="nf">mod_delta</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-56"><a href="#Pathier-56"><span class="linenos"> 56</span></a>        <span class="sd">&quot;&quot;&quot;Returns how long ago in seconds this file or directory was modified.&quot;&quot;&quot;</span>
+</span><span id="Pathier-57"><a href="#Pathier-57"><span class="linenos"> 57</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-58"><a href="#Pathier-58"><span class="linenos"> 58</span></a>            <span class="k">return</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span><span class="p">)</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
+</span><span id="Pathier-59"><a href="#Pathier-59"><span class="linenos"> 59</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-60"><a href="#Pathier-60"><span class="linenos"> 60</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-61"><a href="#Pathier-61"><span class="linenos"> 61</span></a>
+</span><span id="Pathier-62"><a href="#Pathier-62"><span class="linenos"> 62</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-63"><a href="#Pathier-63"><span class="linenos"> 63</span></a>    <span class="k">def</span> <span class="nf">last_read_time</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-64"><a href="#Pathier-64"><span class="linenos"> 64</span></a>        <span class="sd">&quot;&quot;&quot;Returns the last time this object made a call to `self.read_text()`, `self.read_bytes()`, or `self.open(mode=&quot;r&quot;|&quot;rb&quot;)`.</span>
+</span><span id="Pathier-65"><a href="#Pathier-65"><span class="linenos"> 65</span></a><span class="sd">        Returns `None` if the file hasn&#39;t been read from.</span>
+</span><span id="Pathier-66"><a href="#Pathier-66"><span class="linenos"> 66</span></a>
+</span><span id="Pathier-67"><a href="#Pathier-67"><span class="linenos"> 67</span></a><span class="sd">        Note: This property is only relative to the lifetime of this `Pathier` instance, not the file itself.</span>
+</span><span id="Pathier-68"><a href="#Pathier-68"><span class="linenos"> 68</span></a><span class="sd">        i.e. This property will reset if you create a new `Pathier` object pointing to the same file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-69"><a href="#Pathier-69"><span class="linenos"> 69</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span><span class="p">:</span>
+</span><span id="Pathier-70"><a href="#Pathier-70"><span class="linenos"> 70</span></a>            <span class="k">return</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span><span class="p">)</span>
+</span><span id="Pathier-71"><a href="#Pathier-71"><span class="linenos"> 71</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-72"><a href="#Pathier-72"><span class="linenos"> 72</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span>
+</span><span id="Pathier-73"><a href="#Pathier-73"><span class="linenos"> 73</span></a>
+</span><span id="Pathier-74"><a href="#Pathier-74"><span class="linenos"> 74</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-75"><a href="#Pathier-75"><span class="linenos"> 75</span></a>    <span class="k">def</span> <span class="nf">modified_since_last_read</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-76"><a href="#Pathier-76"><span class="linenos"> 76</span></a>        <span class="sd">&quot;&quot;&quot;Returns `True` if this file hasn&#39;t been read from or has been modified since the last time this object</span>
+</span><span id="Pathier-77"><a href="#Pathier-77"><span class="linenos"> 77</span></a><span class="sd">        made a call to `self.read_text()`, `self.read_bytes()`, or `self.open(mode=&quot;r&quot;|&quot;rb&quot;)`.</span>
+</span><span id="Pathier-78"><a href="#Pathier-78"><span class="linenos"> 78</span></a>
+</span><span id="Pathier-79"><a href="#Pathier-79"><span class="linenos"> 79</span></a><span class="sd">        Note: This property is only relative to the lifetime of this `Pathier` instance, not the file itself.</span>
+</span><span id="Pathier-80"><a href="#Pathier-80"><span class="linenos"> 80</span></a><span class="sd">        i.e. This property will reset if you create a new `Pathier` object pointing to the same file.</span>
+</span><span id="Pathier-81"><a href="#Pathier-81"><span class="linenos"> 81</span></a>
+</span><span id="Pathier-82"><a href="#Pathier-82"><span class="linenos"> 82</span></a><span class="sd">        #### Caveat:</span>
+</span><span id="Pathier-83"><a href="#Pathier-83"><span class="linenos"> 83</span></a><span class="sd">        May not be accurate if the file was modified within a couple of seconds of checking this property.</span>
+</span><span id="Pathier-84"><a href="#Pathier-84"><span class="linenos"> 84</span></a><span class="sd">        (For instance, on my machine `self.mod_date` is consistently 1-1.5s in the future from when `self.write_text()` was called according to `time.time()`.)</span>
+</span><span id="Pathier-85"><a href="#Pathier-85"><span class="linenos"> 85</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Pathier-86"><a href="#Pathier-86"><span class="linenos"> 86</span></a>
+</span><span id="Pathier-87"><a href="#Pathier-87"><span class="linenos"> 87</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">last_read_time</span> <span class="ow">is</span> <span class="kc">None</span> <span class="ow">or</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">last_read_time</span>
+</span><span id="Pathier-88"><a href="#Pathier-88"><span class="linenos"> 88</span></a>
+</span><span id="Pathier-89"><a href="#Pathier-89"><span class="linenos"> 89</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-90"><a href="#Pathier-90"><span class="linenos"> 90</span></a>    <span class="k">def</span> <span class="nf">size</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Pathier-91"><a href="#Pathier-91"><span class="linenos"> 91</span></a>        <span class="sd">&quot;&quot;&quot;Returns the size in bytes of this file or directory.</span>
+</span><span id="Pathier-92"><a href="#Pathier-92"><span class="linenos"> 92</span></a>
+</span><span id="Pathier-93"><a href="#Pathier-93"><span class="linenos"> 93</span></a><span class="sd">        If this path doesn&#39;t exist, `0` will be returned.&quot;&quot;&quot;</span>
+</span><span id="Pathier-94"><a href="#Pathier-94"><span class="linenos"> 94</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-95"><a href="#Pathier-95"><span class="linenos"> 95</span></a>            <span class="k">return</span> <span class="mi">0</span>
+</span><span id="Pathier-96"><a href="#Pathier-96"><span class="linenos"> 96</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-97"><a href="#Pathier-97"><span class="linenos"> 97</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
+</span><span id="Pathier-98"><a href="#Pathier-98"><span class="linenos"> 98</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-99"><a href="#Pathier-99"><span class="linenos"> 99</span></a>            <span class="k">return</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
+</span><span id="Pathier-100"><a href="#Pathier-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="mi">0</span>
+</span><span id="Pathier-101"><a href="#Pathier-101"><span class="linenos">101</span></a>
+</span><span id="Pathier-102"><a href="#Pathier-102"><span class="linenos">102</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Pathier-103"><a href="#Pathier-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">format_bytes</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Pathier-104"><a href="#Pathier-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;Format `size` with common file size abbreviations and rounded to two decimal places.</span>
+</span><span id="Pathier-105"><a href="#Pathier-105"><span class="linenos">105</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-106"><a href="#Pathier-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
+</span><span id="Pathier-107"><a href="#Pathier-107"><span class="linenos">107</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
+</span><span id="Pathier-108"><a href="#Pathier-108"><span class="linenos">108</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
+</span><span id="Pathier-109"><a href="#Pathier-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
+</span><span id="Pathier-110"><a href="#Pathier-110"><span class="linenos">110</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Pathier-111"><a href="#Pathier-111"><span class="linenos">111</span></a>
+</span><span id="Pathier-112"><a href="#Pathier-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-113"><a href="#Pathier-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-114"><a href="#Pathier-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
+</span><span id="Pathier-115"><a href="#Pathier-115"><span class="linenos">115</span></a>
+</span><span id="Pathier-116"><a href="#Pathier-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-117"><a href="#Pathier-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-118"><a href="#Pathier-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
+</span><span id="Pathier-119"><a href="#Pathier-119"><span class="linenos">119</span></a>
+</span><span id="Pathier-120"><a href="#Pathier-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-121"><a href="#Pathier-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified more recently than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-122"><a href="#Pathier-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
+</span><span id="Pathier-123"><a href="#Pathier-123"><span class="linenos">123</span></a>
+</span><span id="Pathier-124"><a href="#Pathier-124"><span class="linenos">124</span></a>    <span class="c1"># ===============================================navigation===============================================</span>
+</span><span id="Pathier-125"><a href="#Pathier-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-126"><a href="#Pathier-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-127"><a href="#Pathier-127"><span class="linenos">127</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-128"><a href="#Pathier-128"><span class="linenos">128</span></a>
+</span><span id="Pathier-129"><a href="#Pathier-129"><span class="linenos">129</span></a>    <span class="nd">@property</span>
+</span><span id="Pathier-130"><a href="#Pathier-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">in_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier-131"><a href="#Pathier-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Return `True` if this path is in `sys.path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-132"><a href="#Pathier-132"><span class="linenos">132</span></a>        <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="ow">in</span> <span class="n">sys</span><span class="o">.</span><span class="n">path</span>
 </span><span id="Pathier-133"><a href="#Pathier-133"><span class="linenos">133</span></a>
-</span><span id="Pathier-134"><a href="#Pathier-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-135"><a href="#Pathier-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from sys.path</span>
-</span><span id="Pathier-136"><a href="#Pathier-136"><span class="linenos">136</span></a><span class="sd">        if it&#39;s in sys.path.&quot;&quot;&quot;</span>
-</span><span id="Pathier-137"><a href="#Pathier-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier-138"><a href="#Pathier-138"><span class="linenos">138</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
-</span><span id="Pathier-139"><a href="#Pathier-139"><span class="linenos">139</span></a>
-</span><span id="Pathier-140"><a href="#Pathier-140"><span class="linenos">140</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-141"><a href="#Pathier-141"><span class="linenos">141</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is a parent of this instance.</span>
-</span><span id="Pathier-142"><a href="#Pathier-142"><span class="linenos">142</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier-143"><a href="#Pathier-143"><span class="linenos">143</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier-144"><a href="#Pathier-144"><span class="linenos">144</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
-</span><span id="Pathier-145"><a href="#Pathier-145"><span class="linenos">145</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
-</span><span id="Pathier-146"><a href="#Pathier-146"><span class="linenos">146</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
-</span><span id="Pathier-147"><a href="#Pathier-147"><span class="linenos">147</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-148"><a href="#Pathier-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-149"><a href="#Pathier-149"><span class="linenos">149</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-150"><a href="#Pathier-150"><span class="linenos">150</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
-</span><span id="Pathier-151"><a href="#Pathier-151"><span class="linenos">151</span></a>
-</span><span id="Pathier-152"><a href="#Pathier-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="fm">__sub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">levels</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-153"><a href="#Pathier-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object moved up &#39;levels&#39; number of parents from the current path.</span>
-</span><span id="Pathier-154"><a href="#Pathier-154"><span class="linenos">154</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier-155"><a href="#Pathier-155"><span class="linenos">155</span></a><span class="sd">        &gt;&gt;&gt; new_p = p - 3</span>
-</span><span id="Pathier-156"><a href="#Pathier-156"><span class="linenos">156</span></a><span class="sd">        &gt;&gt;&gt; print(new_p)</span>
-</span><span id="Pathier-157"><a href="#Pathier-157"><span class="linenos">157</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier-158"><a href="#Pathier-158"><span class="linenos">158</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span>
-</span><span id="Pathier-159"><a href="#Pathier-159"><span class="linenos">159</span></a>        <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">levels</span><span class="p">):</span>
-</span><span id="Pathier-160"><a href="#Pathier-160"><span class="linenos">160</span></a>            <span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">parent</span>
-</span><span id="Pathier-161"><a href="#Pathier-161"><span class="linenos">161</span></a>        <span class="k">return</span> <span class="n">path</span>
-</span><span id="Pathier-162"><a href="#Pathier-162"><span class="linenos">162</span></a>
-</span><span id="Pathier-163"><a href="#Pathier-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-164"><a href="#Pathier-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object such that the stem</span>
-</span><span id="Pathier-165"><a href="#Pathier-165"><span class="linenos">165</span></a><span class="sd">        is one level below the folder &#39;name&#39;.</span>
-</span><span id="Pathier-166"><a href="#Pathier-166"><span class="linenos">166</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier-167"><a href="#Pathier-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier-168"><a href="#Pathier-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
-</span><span id="Pathier-169"><a href="#Pathier-169"><span class="linenos">169</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier-170"><a href="#Pathier-170"><span class="linenos">170</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-171"><a href="#Pathier-171"><span class="linenos">171</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-172"><a href="#Pathier-172"><span class="linenos">172</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
-</span><span id="Pathier-173"><a href="#Pathier-173"><span class="linenos">173</span></a>
-</span><span id="Pathier-174"><a href="#Pathier-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-175"><a href="#Pathier-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is the</span>
-</span><span id="Pathier-176"><a href="#Pathier-176"><span class="linenos">176</span></a><span class="sd">        relative child path after &#39;name&#39;.</span>
-</span><span id="Pathier-177"><a href="#Pathier-177"><span class="linenos">177</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
+</span><span id="Pathier-134"><a href="#Pathier-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
+</span><span id="Pathier-135"><a href="#Pathier-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into `sys.path` if it isn&#39;t already there.</span>
+</span><span id="Pathier-136"><a href="#Pathier-136"><span class="linenos">136</span></a>
+</span><span id="Pathier-137"><a href="#Pathier-137"><span class="linenos">137</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-138"><a href="#Pathier-138"><span class="linenos">138</span></a>
+</span><span id="Pathier-139"><a href="#Pathier-139"><span class="linenos">139</span></a><span class="sd">        `index`: The index of `sys.path` to insert this path at.&quot;&quot;&quot;</span>
+</span><span id="Pathier-140"><a href="#Pathier-140"><span class="linenos">140</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-141"><a href="#Pathier-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-142"><a href="#Pathier-142"><span class="linenos">142</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
+</span><span id="Pathier-143"><a href="#Pathier-143"><span class="linenos">143</span></a>
+</span><span id="Pathier-144"><a href="#Pathier-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-145"><a href="#Pathier-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to `sys.path` if it isn&#39;t already there.&quot;&quot;&quot;</span>
+</span><span id="Pathier-146"><a href="#Pathier-146"><span class="linenos">146</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-147"><a href="#Pathier-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-148"><a href="#Pathier-148"><span class="linenos">148</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="Pathier-149"><a href="#Pathier-149"><span class="linenos">149</span></a>
+</span><span id="Pathier-150"><a href="#Pathier-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-151"><a href="#Pathier-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from `sys.path` if it&#39;s in `sys.path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-152"><a href="#Pathier-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier-153"><a href="#Pathier-153"><span class="linenos">153</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
+</span><span id="Pathier-154"><a href="#Pathier-154"><span class="linenos">154</span></a>
+</span><span id="Pathier-155"><a href="#Pathier-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-156"><a href="#Pathier-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is a parent of this instance.</span>
+</span><span id="Pathier-157"><a href="#Pathier-157"><span class="linenos">157</span></a>
+</span><span id="Pathier-158"><a href="#Pathier-158"><span class="linenos">158</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier-159"><a href="#Pathier-159"><span class="linenos">159</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier-160"><a href="#Pathier-160"><span class="linenos">160</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
+</span><span id="Pathier-161"><a href="#Pathier-161"><span class="linenos">161</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
+</span><span id="Pathier-162"><a href="#Pathier-162"><span class="linenos">162</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
+</span><span id="Pathier-163"><a href="#Pathier-163"><span class="linenos">163</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-164"><a href="#Pathier-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-165"><a href="#Pathier-165"><span class="linenos">165</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-166"><a href="#Pathier-166"><span class="linenos">166</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
+</span><span id="Pathier-167"><a href="#Pathier-167"><span class="linenos">167</span></a>
+</span><span id="Pathier-168"><a href="#Pathier-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="fm">__sub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">levels</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-169"><a href="#Pathier-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object moved up `levels` number of parents from the current path.</span>
+</span><span id="Pathier-170"><a href="#Pathier-170"><span class="linenos">170</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier-171"><a href="#Pathier-171"><span class="linenos">171</span></a><span class="sd">        &gt;&gt;&gt; new_p = p - 3</span>
+</span><span id="Pathier-172"><a href="#Pathier-172"><span class="linenos">172</span></a><span class="sd">        &gt;&gt;&gt; print(new_p)</span>
+</span><span id="Pathier-173"><a href="#Pathier-173"><span class="linenos">173</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier-174"><a href="#Pathier-174"><span class="linenos">174</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="bp">self</span>
+</span><span id="Pathier-175"><a href="#Pathier-175"><span class="linenos">175</span></a>        <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">levels</span><span class="p">):</span>
+</span><span id="Pathier-176"><a href="#Pathier-176"><span class="linenos">176</span></a>            <span class="n">path</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">parent</span>
+</span><span id="Pathier-177"><a href="#Pathier-177"><span class="linenos">177</span></a>        <span class="k">return</span> <span class="n">path</span>
 </span><span id="Pathier-178"><a href="#Pathier-178"><span class="linenos">178</span></a>
-</span><span id="Pathier-179"><a href="#Pathier-179"><span class="linenos">179</span></a><span class="sd">        :param keep_name: If True, the returned path will start with &#39;name&#39;.</span>
-</span><span id="Pathier-180"><a href="#Pathier-180"><span class="linenos">180</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier-181"><a href="#Pathier-181"><span class="linenos">181</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
-</span><span id="Pathier-182"><a href="#Pathier-182"><span class="linenos">182</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
-</span><span id="Pathier-183"><a href="#Pathier-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
-</span><span id="Pathier-184"><a href="#Pathier-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier-185"><a href="#Pathier-185"><span class="linenos">185</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier-186"><a href="#Pathier-186"><span class="linenos">186</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier-187"><a href="#Pathier-187"><span class="linenos">187</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
-</span><span id="Pathier-188"><a href="#Pathier-188"><span class="linenos">188</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
-</span><span id="Pathier-189"><a href="#Pathier-189"><span class="linenos">189</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
-</span><span id="Pathier-190"><a href="#Pathier-190"><span class="linenos">190</span></a>
-</span><span id="Pathier-191"><a href="#Pathier-191"><span class="linenos">191</span></a>    <span class="c1"># ============================================write and read============================================</span>
-</span><span id="Pathier-192"><a href="#Pathier-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-193"><a href="#Pathier-193"><span class="linenos">193</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
-</span><span id="Pathier-194"><a href="#Pathier-194"><span class="linenos">194</span></a><span class="sd">        Same as Path().mkdir() except</span>
-</span><span id="Pathier-195"><a href="#Pathier-195"><span class="linenos">195</span></a><span class="sd">        &#39;parents&#39; and &#39;exist_ok&#39; default</span>
-</span><span id="Pathier-196"><a href="#Pathier-196"><span class="linenos">196</span></a><span class="sd">        to True instead of False.&quot;&quot;&quot;</span>
-</span><span id="Pathier-197"><a href="#Pathier-197"><span class="linenos">197</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
-</span><span id="Pathier-198"><a href="#Pathier-198"><span class="linenos">198</span></a>
-</span><span id="Pathier-199"><a href="#Pathier-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier-200"><a href="#Pathier-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Create file and parents if necessary.&quot;&quot;&quot;</span>
-</span><span id="Pathier-201"><a href="#Pathier-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="Pathier-202"><a href="#Pathier-202"><span class="linenos">202</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
-</span><span id="Pathier-203"><a href="#Pathier-203"><span class="linenos">203</span></a>
-</span><span id="Pathier-204"><a href="#Pathier-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
-</span><span id="Pathier-205"><a href="#Pathier-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-206"><a href="#Pathier-206"><span class="linenos">206</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-207"><a href="#Pathier-207"><span class="linenos">207</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-208"><a href="#Pathier-208"><span class="linenos">208</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-209"><a href="#Pathier-209"><span class="linenos">209</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-210"><a href="#Pathier-210"><span class="linenos">210</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-211"><a href="#Pathier-211"><span class="linenos">211</span></a>    <span class="p">):</span>
-</span><span id="Pathier-212"><a href="#Pathier-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file. If a TypeError is raised, the function</span>
-</span><span id="Pathier-213"><a href="#Pathier-213"><span class="linenos">213</span></a><span class="sd">        will attempt to case data to a str and try the write again.</span>
-</span><span id="Pathier-214"><a href="#Pathier-214"><span class="linenos">214</span></a><span class="sd">        If a FileNotFoundError is raised and parents = True,</span>
-</span><span id="Pathier-215"><a href="#Pathier-215"><span class="linenos">215</span></a><span class="sd">        self.parent will be created.&quot;&quot;&quot;</span>
-</span><span id="Pathier-216"><a href="#Pathier-216"><span class="linenos">216</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
-</span><span id="Pathier-217"><a href="#Pathier-217"><span class="linenos">217</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
-</span><span id="Pathier-218"><a href="#Pathier-218"><span class="linenos">218</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier-219"><a href="#Pathier-219"><span class="linenos">219</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier-220"><a href="#Pathier-220"><span class="linenos">220</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier-221"><a href="#Pathier-221"><span class="linenos">221</span></a>        <span class="p">)</span>
-</span><span id="Pathier-222"><a href="#Pathier-222"><span class="linenos">222</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier-223"><a href="#Pathier-223"><span class="linenos">223</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-224"><a href="#Pathier-224"><span class="linenos">224</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
-</span><span id="Pathier-225"><a href="#Pathier-225"><span class="linenos">225</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-226"><a href="#Pathier-226"><span class="linenos">226</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-227"><a href="#Pathier-227"><span class="linenos">227</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier-228"><a href="#Pathier-228"><span class="linenos">228</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier-229"><a href="#Pathier-229"><span class="linenos">229</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-230"><a href="#Pathier-230"><span class="linenos">230</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-231"><a href="#Pathier-231"><span class="linenos">231</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-232"><a href="#Pathier-232"><span class="linenos">232</span></a>                <span class="k">raise</span>
-</span><span id="Pathier-233"><a href="#Pathier-233"><span class="linenos">233</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier-234"><a href="#Pathier-234"><span class="linenos">234</span></a>            <span class="k">raise</span>
-</span><span id="Pathier-235"><a href="#Pathier-235"><span class="linenos">235</span></a>
-</span><span id="Pathier-236"><a href="#Pathier-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-237"><a href="#Pathier-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
-</span><span id="Pathier-238"><a href="#Pathier-238"><span class="linenos">238</span></a>
-</span><span id="Pathier-239"><a href="#Pathier-239"><span class="linenos">239</span></a><span class="sd">        :param parents: If True and the write operation fails</span>
-</span><span id="Pathier-240"><a href="#Pathier-240"><span class="linenos">240</span></a><span class="sd">        with a FileNotFoundError, make the parent directory</span>
-</span><span id="Pathier-241"><a href="#Pathier-241"><span class="linenos">241</span></a><span class="sd">        and retry the write.&quot;&quot;&quot;</span>
-</span><span id="Pathier-242"><a href="#Pathier-242"><span class="linenos">242</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier-243"><a href="#Pathier-243"><span class="linenos">243</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-244"><a href="#Pathier-244"><span class="linenos">244</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier-245"><a href="#Pathier-245"><span class="linenos">245</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier-246"><a href="#Pathier-246"><span class="linenos">246</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-247"><a href="#Pathier-247"><span class="linenos">247</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier-248"><a href="#Pathier-248"><span class="linenos">248</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-249"><a href="#Pathier-249"><span class="linenos">249</span></a>                <span class="k">raise</span>
-</span><span id="Pathier-250"><a href="#Pathier-250"><span class="linenos">250</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier-251"><a href="#Pathier-251"><span class="linenos">251</span></a>            <span class="k">raise</span>
-</span><span id="Pathier-252"><a href="#Pathier-252"><span class="linenos">252</span></a>
-</span><span id="Pathier-253"><a href="#Pathier-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-254"><a href="#Pathier-254"><span class="linenos">254</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-255"><a href="#Pathier-255"><span class="linenos">255</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
-</span><span id="Pathier-256"><a href="#Pathier-256"><span class="linenos">256</span></a>
-</span><span id="Pathier-257"><a href="#Pathier-257"><span class="linenos">257</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier-258"><a href="#Pathier-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-259"><a href="#Pathier-259"><span class="linenos">259</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-260"><a href="#Pathier-260"><span class="linenos">260</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-261"><a href="#Pathier-261"><span class="linenos">261</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-262"><a href="#Pathier-262"><span class="linenos">262</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-263"><a href="#Pathier-263"><span class="linenos">263</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-264"><a href="#Pathier-264"><span class="linenos">264</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-265"><a href="#Pathier-265"><span class="linenos">265</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-266"><a href="#Pathier-266"><span class="linenos">266</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-267"><a href="#Pathier-267"><span class="linenos">267</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-268"><a href="#Pathier-268"><span class="linenos">268</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-269"><a href="#Pathier-269"><span class="linenos">269</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier-270"><a href="#Pathier-270"><span class="linenos">270</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
-</span><span id="Pathier-271"><a href="#Pathier-271"><span class="linenos">271</span></a>            <span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier-272"><a href="#Pathier-272"><span class="linenos">272</span></a>            <span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier-273"><a href="#Pathier-273"><span class="linenos">273</span></a>            <span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier-274"><a href="#Pathier-274"><span class="linenos">274</span></a>            <span class="n">parents</span><span class="p">,</span>
-</span><span id="Pathier-275"><a href="#Pathier-275"><span class="linenos">275</span></a>        <span class="p">)</span>
-</span><span id="Pathier-276"><a href="#Pathier-276"><span class="linenos">276</span></a>
-</span><span id="Pathier-277"><a href="#Pathier-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-278"><a href="#Pathier-278"><span class="linenos">278</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-279"><a href="#Pathier-279"><span class="linenos">279</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
-</span><span id="Pathier-280"><a href="#Pathier-280"><span class="linenos">280</span></a>
-</span><span id="Pathier-281"><a href="#Pathier-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
-</span><span id="Pathier-282"><a href="#Pathier-282"><span class="linenos">282</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-283"><a href="#Pathier-283"><span class="linenos">283</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-284"><a href="#Pathier-284"><span class="linenos">284</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-285"><a href="#Pathier-285"><span class="linenos">285</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-286"><a href="#Pathier-286"><span class="linenos">286</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-287"><a href="#Pathier-287"><span class="linenos">287</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-288"><a href="#Pathier-288"><span class="linenos">288</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-289"><a href="#Pathier-289"><span class="linenos">289</span></a>    <span class="p">):</span>
-</span><span id="Pathier-290"><a href="#Pathier-290"><span class="linenos">290</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier-291"><a href="#Pathier-291"><span class="linenos">291</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier-292"><a href="#Pathier-292"><span class="linenos">292</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier-293"><a href="#Pathier-293"><span class="linenos">293</span></a>        <span class="p">)</span>
+</span><span id="Pathier-179"><a href="#Pathier-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-180"><a href="#Pathier-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object such that the stem is one level below the given folder `name`.</span>
+</span><span id="Pathier-181"><a href="#Pathier-181"><span class="linenos">181</span></a>
+</span><span id="Pathier-182"><a href="#Pathier-182"><span class="linenos">182</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier-183"><a href="#Pathier-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier-184"><a href="#Pathier-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
+</span><span id="Pathier-185"><a href="#Pathier-185"><span class="linenos">185</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier-186"><a href="#Pathier-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-187"><a href="#Pathier-187"><span class="linenos">187</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-188"><a href="#Pathier-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
+</span><span id="Pathier-189"><a href="#Pathier-189"><span class="linenos">189</span></a>
+</span><span id="Pathier-190"><a href="#Pathier-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-191"><a href="#Pathier-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is the relative child path after `name`.</span>
+</span><span id="Pathier-192"><a href="#Pathier-192"><span class="linenos">192</span></a>
+</span><span id="Pathier-193"><a href="#Pathier-193"><span class="linenos">193</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier-194"><a href="#Pathier-194"><span class="linenos">194</span></a>
+</span><span id="Pathier-195"><a href="#Pathier-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-196"><a href="#Pathier-196"><span class="linenos">196</span></a>
+</span><span id="Pathier-197"><a href="#Pathier-197"><span class="linenos">197</span></a><span class="sd">        `keep_name`: If `True`, the returned path will start with `name`.</span>
+</span><span id="Pathier-198"><a href="#Pathier-198"><span class="linenos">198</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier-199"><a href="#Pathier-199"><span class="linenos">199</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
+</span><span id="Pathier-200"><a href="#Pathier-200"><span class="linenos">200</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
+</span><span id="Pathier-201"><a href="#Pathier-201"><span class="linenos">201</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
+</span><span id="Pathier-202"><a href="#Pathier-202"><span class="linenos">202</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier-203"><a href="#Pathier-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier-204"><a href="#Pathier-204"><span class="linenos">204</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier-205"><a href="#Pathier-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
+</span><span id="Pathier-206"><a href="#Pathier-206"><span class="linenos">206</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
+</span><span id="Pathier-207"><a href="#Pathier-207"><span class="linenos">207</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
+</span><span id="Pathier-208"><a href="#Pathier-208"><span class="linenos">208</span></a>
+</span><span id="Pathier-209"><a href="#Pathier-209"><span class="linenos">209</span></a>    <span class="c1"># ============================================write and read============================================</span>
+</span><span id="Pathier-210"><a href="#Pathier-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-211"><a href="#Pathier-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
+</span><span id="Pathier-212"><a href="#Pathier-212"><span class="linenos">212</span></a>
+</span><span id="Pathier-213"><a href="#Pathier-213"><span class="linenos">213</span></a><span class="sd">        Same as `Path().mkdir()` except `parents` and `exist_ok` default to `True` instead of `False`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-214"><a href="#Pathier-214"><span class="linenos">214</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
+</span><span id="Pathier-215"><a href="#Pathier-215"><span class="linenos">215</span></a>
+</span><span id="Pathier-216"><a href="#Pathier-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier-217"><a href="#Pathier-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Create file (and parents if necessary).&quot;&quot;&quot;</span>
+</span><span id="Pathier-218"><a href="#Pathier-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="Pathier-219"><a href="#Pathier-219"><span class="linenos">219</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+</span><span id="Pathier-220"><a href="#Pathier-220"><span class="linenos">220</span></a>
+</span><span id="Pathier-221"><a href="#Pathier-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s2">&quot;r&quot;</span><span class="p">,</span> <span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">newline</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier-222"><a href="#Pathier-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Pathier-223"><a href="#Pathier-223"><span class="linenos">223</span></a><span class="sd">        Open the file pointed by this path and return a file object, as</span>
+</span><span id="Pathier-224"><a href="#Pathier-224"><span class="linenos">224</span></a><span class="sd">        the built-in open() function does.</span>
+</span><span id="Pathier-225"><a href="#Pathier-225"><span class="linenos">225</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Pathier-226"><a href="#Pathier-226"><span class="linenos">226</span></a>        <span class="n">stream</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">buffering</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">)</span>
+</span><span id="Pathier-227"><a href="#Pathier-227"><span class="linenos">227</span></a>        <span class="k">if</span> <span class="s2">&quot;r&quot;</span> <span class="ow">in</span> <span class="n">mode</span><span class="p">:</span>
+</span><span id="Pathier-228"><a href="#Pathier-228"><span class="linenos">228</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Pathier-229"><a href="#Pathier-229"><span class="linenos">229</span></a>        <span class="k">return</span> <span class="n">stream</span>
+</span><span id="Pathier-230"><a href="#Pathier-230"><span class="linenos">230</span></a>
+</span><span id="Pathier-231"><a href="#Pathier-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
+</span><span id="Pathier-232"><a href="#Pathier-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-233"><a href="#Pathier-233"><span class="linenos">233</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-234"><a href="#Pathier-234"><span class="linenos">234</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-235"><a href="#Pathier-235"><span class="linenos">235</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-236"><a href="#Pathier-236"><span class="linenos">236</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-237"><a href="#Pathier-237"><span class="linenos">237</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-238"><a href="#Pathier-238"><span class="linenos">238</span></a>    <span class="p">):</span>
+</span><span id="Pathier-239"><a href="#Pathier-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file.</span>
+</span><span id="Pathier-240"><a href="#Pathier-240"><span class="linenos">240</span></a>
+</span><span id="Pathier-241"><a href="#Pathier-241"><span class="linenos">241</span></a><span class="sd">        If a `TypeError` is raised, the function  will attempt to cast `data` to a `str` and try the write again.</span>
+</span><span id="Pathier-242"><a href="#Pathier-242"><span class="linenos">242</span></a>
+</span><span id="Pathier-243"><a href="#Pathier-243"><span class="linenos">243</span></a><span class="sd">        If a `FileNotFoundError` is raised and `parents = True`, `self.parent` will be created.&quot;&quot;&quot;</span>
+</span><span id="Pathier-244"><a href="#Pathier-244"><span class="linenos">244</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
+</span><span id="Pathier-245"><a href="#Pathier-245"><span class="linenos">245</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
+</span><span id="Pathier-246"><a href="#Pathier-246"><span class="linenos">246</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier-247"><a href="#Pathier-247"><span class="linenos">247</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier-248"><a href="#Pathier-248"><span class="linenos">248</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier-249"><a href="#Pathier-249"><span class="linenos">249</span></a>        <span class="p">)</span>
+</span><span id="Pathier-250"><a href="#Pathier-250"><span class="linenos">250</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier-251"><a href="#Pathier-251"><span class="linenos">251</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-252"><a href="#Pathier-252"><span class="linenos">252</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
+</span><span id="Pathier-253"><a href="#Pathier-253"><span class="linenos">253</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-254"><a href="#Pathier-254"><span class="linenos">254</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-255"><a href="#Pathier-255"><span class="linenos">255</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier-256"><a href="#Pathier-256"><span class="linenos">256</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier-257"><a href="#Pathier-257"><span class="linenos">257</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-258"><a href="#Pathier-258"><span class="linenos">258</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-259"><a href="#Pathier-259"><span class="linenos">259</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-260"><a href="#Pathier-260"><span class="linenos">260</span></a>                <span class="k">raise</span>
+</span><span id="Pathier-261"><a href="#Pathier-261"><span class="linenos">261</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier-262"><a href="#Pathier-262"><span class="linenos">262</span></a>            <span class="k">raise</span>
+</span><span id="Pathier-263"><a href="#Pathier-263"><span class="linenos">263</span></a>
+</span><span id="Pathier-264"><a href="#Pathier-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-265"><a href="#Pathier-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
+</span><span id="Pathier-266"><a href="#Pathier-266"><span class="linenos">266</span></a>
+</span><span id="Pathier-267"><a href="#Pathier-267"><span class="linenos">267</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-268"><a href="#Pathier-268"><span class="linenos">268</span></a>
+</span><span id="Pathier-269"><a href="#Pathier-269"><span class="linenos">269</span></a><span class="sd">        `parents`: If `True` and the write operation fails with a `FileNotFoundError`,</span>
+</span><span id="Pathier-270"><a href="#Pathier-270"><span class="linenos">270</span></a><span class="sd">        make the parent directory and retry the write.&quot;&quot;&quot;</span>
+</span><span id="Pathier-271"><a href="#Pathier-271"><span class="linenos">271</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier-272"><a href="#Pathier-272"><span class="linenos">272</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-273"><a href="#Pathier-273"><span class="linenos">273</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier-274"><a href="#Pathier-274"><span class="linenos">274</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier-275"><a href="#Pathier-275"><span class="linenos">275</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-276"><a href="#Pathier-276"><span class="linenos">276</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier-277"><a href="#Pathier-277"><span class="linenos">277</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-278"><a href="#Pathier-278"><span class="linenos">278</span></a>                <span class="k">raise</span>
+</span><span id="Pathier-279"><a href="#Pathier-279"><span class="linenos">279</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier-280"><a href="#Pathier-280"><span class="linenos">280</span></a>            <span class="k">raise</span>
+</span><span id="Pathier-281"><a href="#Pathier-281"><span class="linenos">281</span></a>
+</span><span id="Pathier-282"><a href="#Pathier-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">append</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier-283"><a href="#Pathier-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Append `data` to the file pointed to by this `Pathier` object.</span>
+</span><span id="Pathier-284"><a href="#Pathier-284"><span class="linenos">284</span></a>
+</span><span id="Pathier-285"><a href="#Pathier-285"><span class="linenos">285</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-286"><a href="#Pathier-286"><span class="linenos">286</span></a>
+</span><span id="Pathier-287"><a href="#Pathier-287"><span class="linenos">287</span></a><span class="sd">        `new_line`: If `True`, add `\\n` to `data`.</span>
+</span><span id="Pathier-288"><a href="#Pathier-288"><span class="linenos">288</span></a>
+</span><span id="Pathier-289"><a href="#Pathier-289"><span class="linenos">289</span></a><span class="sd">        `encoding`: The file encoding to use.&quot;&quot;&quot;</span>
+</span><span id="Pathier-290"><a href="#Pathier-290"><span class="linenos">290</span></a>        <span class="k">if</span> <span class="n">new_line</span><span class="p">:</span>
+</span><span id="Pathier-291"><a href="#Pathier-291"><span class="linenos">291</span></a>            <span class="n">data</span> <span class="o">+=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="Pathier-292"><a href="#Pathier-292"><span class="linenos">292</span></a>        <span class="k">with</span> <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;a&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
+</span><span id="Pathier-293"><a href="#Pathier-293"><span class="linenos">293</span></a>            <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
 </span><span id="Pathier-294"><a href="#Pathier-294"><span class="linenos">294</span></a>
-</span><span id="Pathier-295"><a href="#Pathier-295"><span class="linenos">295</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier-296"><a href="#Pathier-296"><span class="linenos">296</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier-297"><a href="#Pathier-297"><span class="linenos">297</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier-298"><a href="#Pathier-298"><span class="linenos">298</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier-299"><a href="#Pathier-299"><span class="linenos">299</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier-300"><a href="#Pathier-300"><span class="linenos">300</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier-301"><a href="#Pathier-301"><span class="linenos">301</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier-295"><a href="#Pathier-295"><span class="linenos">295</span></a>    <span class="k">def</span> <span class="nf">replace</span><span class="p">(</span>
+</span><span id="Pathier-296"><a href="#Pathier-296"><span class="linenos">296</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-297"><a href="#Pathier-297"><span class="linenos">297</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
+</span><span id="Pathier-298"><a href="#Pathier-298"><span class="linenos">298</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
+</span><span id="Pathier-299"><a href="#Pathier-299"><span class="linenos">299</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-300"><a href="#Pathier-300"><span class="linenos">300</span></a>    <span class="p">):</span>
+</span><span id="Pathier-301"><a href="#Pathier-301"><span class="linenos">301</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
 </span><span id="Pathier-302"><a href="#Pathier-302"><span class="linenos">302</span></a>
-</span><span id="Pathier-303"><a href="#Pathier-303"><span class="linenos">303</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
-</span><span id="Pathier-304"><a href="#Pathier-304"><span class="linenos">304</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-305"><a href="#Pathier-305"><span class="linenos">305</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier-306"><a href="#Pathier-306"><span class="linenos">306</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-307"><a href="#Pathier-307"><span class="linenos">307</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-308"><a href="#Pathier-308"><span class="linenos">308</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-309"><a href="#Pathier-309"><span class="linenos">309</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier-310"><a href="#Pathier-310"><span class="linenos">310</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-311"><a href="#Pathier-311"><span class="linenos">311</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier-312"><a href="#Pathier-312"><span class="linenos">312</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier-313"><a href="#Pathier-313"><span class="linenos">313</span></a>    <span class="p">):</span>
-</span><span id="Pathier-314"><a href="#Pathier-314"><span class="linenos">314</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier-315"><a href="#Pathier-315"><span class="linenos">315</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier-316"><a href="#Pathier-316"><span class="linenos">316</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier-317"><a href="#Pathier-317"><span class="linenos">317</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier-318"><a href="#Pathier-318"><span class="linenos">318</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier-319"><a href="#Pathier-319"><span class="linenos">319</span></a>                <span class="p">)</span>
-</span><span id="Pathier-320"><a href="#Pathier-320"><span class="linenos">320</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier-321"><a href="#Pathier-321"><span class="linenos">321</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
-</span><span id="Pathier-322"><a href="#Pathier-322"><span class="linenos">322</span></a>
-</span><span id="Pathier-323"><a href="#Pathier-323"><span class="linenos">323</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier-324"><a href="#Pathier-324"><span class="linenos">324</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
-</span><span id="Pathier-325"><a href="#Pathier-325"><span class="linenos">325</span></a><span class="sd">        Uses self.unlink() if a file and uses shutil.rmtree() if a directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier-326"><a href="#Pathier-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-327"><a href="#Pathier-327"><span class="linenos">327</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
-</span><span id="Pathier-328"><a href="#Pathier-328"><span class="linenos">328</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-329"><a href="#Pathier-329"><span class="linenos">329</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier-330"><a href="#Pathier-330"><span class="linenos">330</span></a>
-</span><span id="Pathier-331"><a href="#Pathier-331"><span class="linenos">331</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
-</span><span id="Pathier-332"><a href="#Pathier-332"><span class="linenos">332</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Pathier-333"><a href="#Pathier-333"><span class="linenos">333</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier-334"><a href="#Pathier-334"><span class="linenos">334</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
-</span><span id="Pathier-335"><a href="#Pathier-335"><span class="linenos">335</span></a><span class="sd">        to the instance pointed to by new_path using shutil.copyfile</span>
-</span><span id="Pathier-336"><a href="#Pathier-336"><span class="linenos">336</span></a><span class="sd">        or shutil.copytree. Returns the new path.</span>
+</span><span id="Pathier-303"><a href="#Pathier-303"><span class="linenos">303</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-304"><a href="#Pathier-304"><span class="linenos">304</span></a>
+</span><span id="Pathier-305"><a href="#Pathier-305"><span class="linenos">305</span></a><span class="sd">        `count`: Only replace this many occurences of each pair.</span>
+</span><span id="Pathier-306"><a href="#Pathier-306"><span class="linenos">306</span></a><span class="sd">        By default (`-1`), all occurences are replaced.</span>
+</span><span id="Pathier-307"><a href="#Pathier-307"><span class="linenos">307</span></a>
+</span><span id="Pathier-308"><a href="#Pathier-308"><span class="linenos">308</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier-309"><a href="#Pathier-309"><span class="linenos">309</span></a>
+</span><span id="Pathier-310"><a href="#Pathier-310"><span class="linenos">310</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier-311"><a href="#Pathier-311"><span class="linenos">311</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;somefile.txt&quot;)</span>
+</span><span id="Pathier-312"><a href="#Pathier-312"><span class="linenos">312</span></a><span class="sd">        &gt;&gt;&gt;</span>
+</span><span id="Pathier-313"><a href="#Pathier-313"><span class="linenos">313</span></a><span class="sd">        &gt;&gt;&gt; path.replace([(&quot;hello&quot;, &quot;yeet&quot;), (&quot;goodbye&quot;, &quot;yeehaw&quot;)])</span>
+</span><span id="Pathier-314"><a href="#Pathier-314"><span class="linenos">314</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier-315"><a href="#Pathier-315"><span class="linenos">315</span></a><span class="sd">        &gt;&gt;&gt; path.write_text(path.read_text().replace(&quot;hello&quot;, &quot;yeet&quot;).replace(&quot;goodbye&quot;, &quot;yeehaw&quot;))&quot;&quot;&quot;</span>
+</span><span id="Pathier-316"><a href="#Pathier-316"><span class="linenos">316</span></a>        <span class="n">text</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier-317"><a href="#Pathier-317"><span class="linenos">317</span></a>        <span class="k">for</span> <span class="n">sub</span> <span class="ow">in</span> <span class="n">substitutions</span><span class="p">:</span>
+</span><span id="Pathier-318"><a href="#Pathier-318"><span class="linenos">318</span></a>            <span class="n">text</span> <span class="o">=</span> <span class="n">text</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">sub</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">sub</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">count</span><span class="p">)</span>
+</span><span id="Pathier-319"><a href="#Pathier-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">text</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier-320"><a href="#Pathier-320"><span class="linenos">320</span></a>
+</span><span id="Pathier-321"><a href="#Pathier-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
+</span><span id="Pathier-322"><a href="#Pathier-322"><span class="linenos">322</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
+</span><span id="Pathier-323"><a href="#Pathier-323"><span class="linenos">323</span></a>
+</span><span id="Pathier-324"><a href="#Pathier-324"><span class="linenos">324</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
+</span><span id="Pathier-325"><a href="#Pathier-325"><span class="linenos">325</span></a>
+</span><span id="Pathier-326"><a href="#Pathier-326"><span class="linenos">326</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-327"><a href="#Pathier-327"><span class="linenos">327</span></a>
+</span><span id="Pathier-328"><a href="#Pathier-328"><span class="linenos">328</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier-329"><a href="#Pathier-329"><span class="linenos">329</span></a>
+</span><span id="Pathier-330"><a href="#Pathier-330"><span class="linenos">330</span></a><span class="sd">        `sep`: The separator to use when joining `data`.&quot;&quot;&quot;</span>
+</span><span id="Pathier-331"><a href="#Pathier-331"><span class="linenos">331</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">sep</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">data</span><span class="p">),</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier-332"><a href="#Pathier-332"><span class="linenos">332</span></a>
+</span><span id="Pathier-333"><a href="#Pathier-333"><span class="linenos">333</span></a>    <span class="k">def</span> <span class="nf">split</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Pathier-334"><a href="#Pathier-334"><span class="linenos">334</span></a>        <span class="sd">&quot;&quot;&quot;Returns the content of the pointed at file as a list of strings, splitting at new line characters.</span>
+</span><span id="Pathier-335"><a href="#Pathier-335"><span class="linenos">335</span></a>
+</span><span id="Pathier-336"><a href="#Pathier-336"><span class="linenos">336</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).read_text(encoding=encoding).splitlines()`</span>
 </span><span id="Pathier-337"><a href="#Pathier-337"><span class="linenos">337</span></a>
-</span><span id="Pathier-338"><a href="#Pathier-338"><span class="linenos">338</span></a><span class="sd">        :param new_path: The copy destination.</span>
+</span><span id="Pathier-338"><a href="#Pathier-338"><span class="linenos">338</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier-339"><a href="#Pathier-339"><span class="linenos">339</span></a>
-</span><span id="Pathier-340"><a href="#Pathier-340"><span class="linenos">340</span></a><span class="sd">        :param overwrite: If True, files already existing in new_path</span>
-</span><span id="Pathier-341"><a href="#Pathier-341"><span class="linenos">341</span></a><span class="sd">        will be overwritten. If False, only files that don&#39;t exist in new_path</span>
-</span><span id="Pathier-342"><a href="#Pathier-342"><span class="linenos">342</span></a><span class="sd">        will be copied.&quot;&quot;&quot;</span>
-</span><span id="Pathier-343"><a href="#Pathier-343"><span class="linenos">343</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier-344"><a href="#Pathier-344"><span class="linenos">344</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier-345"><a href="#Pathier-345"><span class="linenos">345</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-346"><a href="#Pathier-346"><span class="linenos">346</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-347"><a href="#Pathier-347"><span class="linenos">347</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier-348"><a href="#Pathier-348"><span class="linenos">348</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
-</span><span id="Pathier-349"><a href="#Pathier-349"><span class="linenos">349</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Pathier-350"><a href="#Pathier-350"><span class="linenos">350</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="Pathier-351"><a href="#Pathier-351"><span class="linenos">351</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-352"><a href="#Pathier-352"><span class="linenos">352</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
-</span><span id="Pathier-353"><a href="#Pathier-353"><span class="linenos">353</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier-354"><a href="#Pathier-354"><span class="linenos">354</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-355"><a href="#Pathier-355"><span class="linenos">355</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier-356"><a href="#Pathier-356"><span class="linenos">356</span></a>        <span class="k">return</span> <span class="n">new_path</span>
-</span><span id="Pathier-357"><a href="#Pathier-357"><span class="linenos">357</span></a>
-</span><span id="Pathier-358"><a href="#Pathier-358"><span class="linenos">358</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier-359"><a href="#Pathier-359"><span class="linenos">359</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
-</span><span id="Pathier-360"><a href="#Pathier-360"><span class="linenos">360</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
-</span><span id="Pathier-361"><a href="#Pathier-361"><span class="linenos">361</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
-</span><span id="Pathier-362"><a href="#Pathier-362"><span class="linenos">362</span></a>
-</span><span id="Pathier-363"><a href="#Pathier-363"><span class="linenos">363</span></a><span class="sd">        :param `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
-</span><span id="Pathier-364"><a href="#Pathier-364"><span class="linenos">364</span></a>
-</span><span id="Pathier-365"><a href="#Pathier-365"><span class="linenos">365</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
-</span><span id="Pathier-366"><a href="#Pathier-366"><span class="linenos">366</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
-</span><span id="Pathier-367"><a href="#Pathier-367"><span class="linenos">367</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier-368"><a href="#Pathier-368"><span class="linenos">368</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
-</span><span id="Pathier-369"><a href="#Pathier-369"><span class="linenos">369</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
-</span><span id="Pathier-370"><a href="#Pathier-370"><span class="linenos">370</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier-371"><a href="#Pathier-371"><span class="linenos">371</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
-</span><span id="Pathier-372"><a href="#Pathier-372"><span class="linenos">372</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier-373"><a href="#Pathier-373"><span class="linenos">373</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier-374"><a href="#Pathier-374"><span class="linenos">374</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
-</span><span id="Pathier-375"><a href="#Pathier-375"><span class="linenos">375</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
-</span><span id="Pathier-376"><a href="#Pathier-376"><span class="linenos">376</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Pathier-377"><a href="#Pathier-377"><span class="linenos">377</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
-</span><span id="Pathier-378"><a href="#Pathier-378"><span class="linenos">378</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier-379"><a href="#Pathier-379"><span class="linenos">379</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
+</span><span id="Pathier-340"><a href="#Pathier-340"><span class="linenos">340</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier-341"><a href="#Pathier-341"><span class="linenos">341</span></a>
+</span><span id="Pathier-342"><a href="#Pathier-342"><span class="linenos">342</span></a><span class="sd">        `keepend`: If `True`, line breaks will be included in returned strings.&quot;&quot;&quot;</span>
+</span><span id="Pathier-343"><a href="#Pathier-343"><span class="linenos">343</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="n">keepends</span><span class="p">)</span>
+</span><span id="Pathier-344"><a href="#Pathier-344"><span class="linenos">344</span></a>
+</span><span id="Pathier-345"><a href="#Pathier-345"><span class="linenos">345</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-346"><a href="#Pathier-346"><span class="linenos">346</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-347"><a href="#Pathier-347"><span class="linenos">347</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+</span><span id="Pathier-348"><a href="#Pathier-348"><span class="linenos">348</span></a>
+</span><span id="Pathier-349"><a href="#Pathier-349"><span class="linenos">349</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier-350"><a href="#Pathier-350"><span class="linenos">350</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-351"><a href="#Pathier-351"><span class="linenos">351</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-352"><a href="#Pathier-352"><span class="linenos">352</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-353"><a href="#Pathier-353"><span class="linenos">353</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-354"><a href="#Pathier-354"><span class="linenos">354</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-355"><a href="#Pathier-355"><span class="linenos">355</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-356"><a href="#Pathier-356"><span class="linenos">356</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-357"><a href="#Pathier-357"><span class="linenos">357</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-358"><a href="#Pathier-358"><span class="linenos">358</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-359"><a href="#Pathier-359"><span class="linenos">359</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-360"><a href="#Pathier-360"><span class="linenos">360</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-361"><a href="#Pathier-361"><span class="linenos">361</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier-362"><a href="#Pathier-362"><span class="linenos">362</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
+</span><span id="Pathier-363"><a href="#Pathier-363"><span class="linenos">363</span></a>            <span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier-364"><a href="#Pathier-364"><span class="linenos">364</span></a>            <span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier-365"><a href="#Pathier-365"><span class="linenos">365</span></a>            <span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier-366"><a href="#Pathier-366"><span class="linenos">366</span></a>            <span class="n">parents</span><span class="p">,</span>
+</span><span id="Pathier-367"><a href="#Pathier-367"><span class="linenos">367</span></a>        <span class="p">)</span>
+</span><span id="Pathier-368"><a href="#Pathier-368"><span class="linenos">368</span></a>
+</span><span id="Pathier-369"><a href="#Pathier-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-370"><a href="#Pathier-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-371"><a href="#Pathier-371"><span class="linenos">371</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span><span class="o">.</span><span class="n">unwrap</span><span class="p">()</span>
+</span><span id="Pathier-372"><a href="#Pathier-372"><span class="linenos">372</span></a>
+</span><span id="Pathier-373"><a href="#Pathier-373"><span class="linenos">373</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
+</span><span id="Pathier-374"><a href="#Pathier-374"><span class="linenos">374</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-375"><a href="#Pathier-375"><span class="linenos">375</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-376"><a href="#Pathier-376"><span class="linenos">376</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-377"><a href="#Pathier-377"><span class="linenos">377</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-378"><a href="#Pathier-378"><span class="linenos">378</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-379"><a href="#Pathier-379"><span class="linenos">379</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-380"><a href="#Pathier-380"><span class="linenos">380</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-381"><a href="#Pathier-381"><span class="linenos">381</span></a>    <span class="p">):</span>
+</span><span id="Pathier-382"><a href="#Pathier-382"><span class="linenos">382</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier-383"><a href="#Pathier-383"><span class="linenos">383</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier-384"><a href="#Pathier-384"><span class="linenos">384</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier-385"><a href="#Pathier-385"><span class="linenos">385</span></a>        <span class="p">)</span>
+</span><span id="Pathier-386"><a href="#Pathier-386"><span class="linenos">386</span></a>
+</span><span id="Pathier-387"><a href="#Pathier-387"><span class="linenos">387</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier-388"><a href="#Pathier-388"><span class="linenos">388</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier-389"><a href="#Pathier-389"><span class="linenos">389</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier-390"><a href="#Pathier-390"><span class="linenos">390</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier-391"><a href="#Pathier-391"><span class="linenos">391</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier-392"><a href="#Pathier-392"><span class="linenos">392</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier-393"><a href="#Pathier-393"><span class="linenos">393</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier-394"><a href="#Pathier-394"><span class="linenos">394</span></a>
+</span><span id="Pathier-395"><a href="#Pathier-395"><span class="linenos">395</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
+</span><span id="Pathier-396"><a href="#Pathier-396"><span class="linenos">396</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier-397"><a href="#Pathier-397"><span class="linenos">397</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier-398"><a href="#Pathier-398"><span class="linenos">398</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-399"><a href="#Pathier-399"><span class="linenos">399</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-400"><a href="#Pathier-400"><span class="linenos">400</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-401"><a href="#Pathier-401"><span class="linenos">401</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier-402"><a href="#Pathier-402"><span class="linenos">402</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-403"><a href="#Pathier-403"><span class="linenos">403</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier-404"><a href="#Pathier-404"><span class="linenos">404</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier-405"><a href="#Pathier-405"><span class="linenos">405</span></a>    <span class="p">):</span>
+</span><span id="Pathier-406"><a href="#Pathier-406"><span class="linenos">406</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier-407"><a href="#Pathier-407"><span class="linenos">407</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier-408"><a href="#Pathier-408"><span class="linenos">408</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier-409"><a href="#Pathier-409"><span class="linenos">409</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier-410"><a href="#Pathier-410"><span class="linenos">410</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier-411"><a href="#Pathier-411"><span class="linenos">411</span></a>                <span class="p">)</span>
+</span><span id="Pathier-412"><a href="#Pathier-412"><span class="linenos">412</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier-413"><a href="#Pathier-413"><span class="linenos">413</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
+</span><span id="Pathier-414"><a href="#Pathier-414"><span class="linenos">414</span></a>
+</span><span id="Pathier-415"><a href="#Pathier-415"><span class="linenos">415</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier-416"><a href="#Pathier-416"><span class="linenos">416</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
+</span><span id="Pathier-417"><a href="#Pathier-417"><span class="linenos">417</span></a>
+</span><span id="Pathier-418"><a href="#Pathier-418"><span class="linenos">418</span></a><span class="sd">        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier-419"><a href="#Pathier-419"><span class="linenos">419</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-420"><a href="#Pathier-420"><span class="linenos">420</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
+</span><span id="Pathier-421"><a href="#Pathier-421"><span class="linenos">421</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-422"><a href="#Pathier-422"><span class="linenos">422</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier-423"><a href="#Pathier-423"><span class="linenos">423</span></a>
+</span><span id="Pathier-424"><a href="#Pathier-424"><span class="linenos">424</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
+</span><span id="Pathier-425"><a href="#Pathier-425"><span class="linenos">425</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Pathier-426"><a href="#Pathier-426"><span class="linenos">426</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier-427"><a href="#Pathier-427"><span class="linenos">427</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
+</span><span id="Pathier-428"><a href="#Pathier-428"><span class="linenos">428</span></a><span class="sd">        to the instance pointed to by `new_path` using `shutil.copyfile`</span>
+</span><span id="Pathier-429"><a href="#Pathier-429"><span class="linenos">429</span></a><span class="sd">        or `shutil.copytree`.</span>
+</span><span id="Pathier-430"><a href="#Pathier-430"><span class="linenos">430</span></a>
+</span><span id="Pathier-431"><a href="#Pathier-431"><span class="linenos">431</span></a><span class="sd">        Returns the new path.</span>
+</span><span id="Pathier-432"><a href="#Pathier-432"><span class="linenos">432</span></a>
+</span><span id="Pathier-433"><a href="#Pathier-433"><span class="linenos">433</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-434"><a href="#Pathier-434"><span class="linenos">434</span></a>
+</span><span id="Pathier-435"><a href="#Pathier-435"><span class="linenos">435</span></a><span class="sd">        `new_path`: The copy destination.</span>
+</span><span id="Pathier-436"><a href="#Pathier-436"><span class="linenos">436</span></a>
+</span><span id="Pathier-437"><a href="#Pathier-437"><span class="linenos">437</span></a><span class="sd">        `overwrite`: If `True`, files already existing in `new_path` will be overwritten.</span>
+</span><span id="Pathier-438"><a href="#Pathier-438"><span class="linenos">438</span></a><span class="sd">        If `False`, only files that don&#39;t exist in `new_path` will be copied.&quot;&quot;&quot;</span>
+</span><span id="Pathier-439"><a href="#Pathier-439"><span class="linenos">439</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier-440"><a href="#Pathier-440"><span class="linenos">440</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier-441"><a href="#Pathier-441"><span class="linenos">441</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-442"><a href="#Pathier-442"><span class="linenos">442</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-443"><a href="#Pathier-443"><span class="linenos">443</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier-444"><a href="#Pathier-444"><span class="linenos">444</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
+</span><span id="Pathier-445"><a href="#Pathier-445"><span class="linenos">445</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Pathier-446"><a href="#Pathier-446"><span class="linenos">446</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="Pathier-447"><a href="#Pathier-447"><span class="linenos">447</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-448"><a href="#Pathier-448"><span class="linenos">448</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
+</span><span id="Pathier-449"><a href="#Pathier-449"><span class="linenos">449</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier-450"><a href="#Pathier-450"><span class="linenos">450</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-451"><a href="#Pathier-451"><span class="linenos">451</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier-452"><a href="#Pathier-452"><span class="linenos">452</span></a>        <span class="k">return</span> <span class="n">new_path</span>
+</span><span id="Pathier-453"><a href="#Pathier-453"><span class="linenos">453</span></a>
+</span><span id="Pathier-454"><a href="#Pathier-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier-455"><a href="#Pathier-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
+</span><span id="Pathier-456"><a href="#Pathier-456"><span class="linenos">456</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
+</span><span id="Pathier-457"><a href="#Pathier-457"><span class="linenos">457</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
+</span><span id="Pathier-458"><a href="#Pathier-458"><span class="linenos">458</span></a>
+</span><span id="Pathier-459"><a href="#Pathier-459"><span class="linenos">459</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-460"><a href="#Pathier-460"><span class="linenos">460</span></a>
+</span><span id="Pathier-461"><a href="#Pathier-461"><span class="linenos">461</span></a><span class="sd">        `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
+</span><span id="Pathier-462"><a href="#Pathier-462"><span class="linenos">462</span></a>
+</span><span id="Pathier-463"><a href="#Pathier-463"><span class="linenos">463</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
+</span><span id="Pathier-464"><a href="#Pathier-464"><span class="linenos">464</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
+</span><span id="Pathier-465"><a href="#Pathier-465"><span class="linenos">465</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier-466"><a href="#Pathier-466"><span class="linenos">466</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
+</span><span id="Pathier-467"><a href="#Pathier-467"><span class="linenos">467</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
+</span><span id="Pathier-468"><a href="#Pathier-468"><span class="linenos">468</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier-469"><a href="#Pathier-469"><span class="linenos">469</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
+</span><span id="Pathier-470"><a href="#Pathier-470"><span class="linenos">470</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier-471"><a href="#Pathier-471"><span class="linenos">471</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier-472"><a href="#Pathier-472"><span class="linenos">472</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
+</span><span id="Pathier-473"><a href="#Pathier-473"><span class="linenos">473</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
+</span><span id="Pathier-474"><a href="#Pathier-474"><span class="linenos">474</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Pathier-475"><a href="#Pathier-475"><span class="linenos">475</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
+</span><span id="Pathier-476"><a href="#Pathier-476"><span class="linenos">476</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier-477"><a href="#Pathier-477"><span class="linenos">477</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
+</span><span id="Pathier-478"><a href="#Pathier-478"><span class="linenos">478</span></a>
+</span><span id="Pathier-479"><a href="#Pathier-479"><span class="linenos">479</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Pathier-480"><a href="#Pathier-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Make a call to `os.system` using the path pointed to by this Pathier object.</span>
+</span><span id="Pathier-481"><a href="#Pathier-481"><span class="linenos">481</span></a>
+</span><span id="Pathier-482"><a href="#Pathier-482"><span class="linenos">482</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier-483"><a href="#Pathier-483"><span class="linenos">483</span></a>
+</span><span id="Pathier-484"><a href="#Pathier-484"><span class="linenos">484</span></a><span class="sd">        `command`: Program/command to precede the path with.</span>
+</span><span id="Pathier-485"><a href="#Pathier-485"><span class="linenos">485</span></a>
+</span><span id="Pathier-486"><a href="#Pathier-486"><span class="linenos">486</span></a><span class="sd">        `args`: Any arguments that should come after the path.</span>
+</span><span id="Pathier-487"><a href="#Pathier-487"><span class="linenos">487</span></a>
+</span><span id="Pathier-488"><a href="#Pathier-488"><span class="linenos">488</span></a><span class="sd">        :returns: The integer output of `os.system`.</span>
+</span><span id="Pathier-489"><a href="#Pathier-489"><span class="linenos">489</span></a>
+</span><span id="Pathier-490"><a href="#Pathier-490"><span class="linenos">490</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier-491"><a href="#Pathier-491"><span class="linenos">491</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;mydirectory&quot;) / &quot;myscript.py&quot;</span>
+</span><span id="Pathier-492"><a href="#Pathier-492"><span class="linenos">492</span></a><span class="sd">        then</span>
+</span><span id="Pathier-493"><a href="#Pathier-493"><span class="linenos">493</span></a><span class="sd">        &gt;&gt;&gt; path.execute(&quot;py&quot;, &quot;--iterations 10&quot;)</span>
+</span><span id="Pathier-494"><a href="#Pathier-494"><span class="linenos">494</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier-495"><a href="#Pathier-495"><span class="linenos">495</span></a><span class="sd">        &gt;&gt;&gt; os.system(f&quot;py {path} --iterations 10&quot;)&quot;&quot;&quot;</span>
+</span><span id="Pathier-496"><a href="#Pathier-496"><span class="linenos">496</span></a>        <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclasses the standard library pathlib.Path class.</p>
 </div>
 
 
@@ -548,16 +695,15 @@
                                 <div class="attr variable">
             <span class="name">dob</span><span class="annotation">: datetime.datetime | None</span>
 
         
     </div>
     <a class="headerlink" href="#Pathier.dob"></a>
     
-            <div class="docstring"><p>Returns the creation date of this file
-or directory as a dateime.datetime object.</p>
+            <div class="docstring"><p>Returns the creation date of this file or directory as a <code>dateime.datetime</code> object.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.age" class="classattr">
                                 <div class="attr variable">
             <span class="name">age</span><span class="annotation">: float | None</span>
@@ -575,101 +721,111 @@
                                 <div class="attr variable">
             <span class="name">mod_date</span><span class="annotation">: datetime.datetime | None</span>
 
         
     </div>
     <a class="headerlink" href="#Pathier.mod_date"></a>
     
-            <div class="docstring"><p>Returns the modification date of this file
-or directory as a datetime.datetime object.</p>
+            <div class="docstring"><p>Returns the modification date of this file or directory as a <code>datetime.datetime</code> object.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.mod_delta" class="classattr">
                                 <div class="attr variable">
             <span class="name">mod_delta</span><span class="annotation">: float | None</span>
 
         
     </div>
     <a class="headerlink" href="#Pathier.mod_delta"></a>
     
-            <div class="docstring"><p>Returns how long ago in seconds this file
-or directory was modified.</p>
+            <div class="docstring"><p>Returns how long ago in seconds this file or directory was modified.</p>
 </div>
 
 
                             </div>
-                            <div id="Pathier.size" class="classattr">
-                                        <input id="Pathier.size-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr function">
-            
-        <span class="def">def</span>
-        <span class="name">size</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span>:</span></span>
+                            <div id="Pathier.last_read_time" class="classattr">
+                                <div class="attr variable">
+            <span class="name">last_read_time</span><span class="annotation">: datetime.datetime | None</span>
 
-                <label class="view-source-button" for="Pathier.size-view-source"><span>View Source</span></label>
+        
+    </div>
+    <a class="headerlink" href="#Pathier.last_read_time"></a>
+    
+            <div class="docstring"><p>Returns the last time this object made a call to <code>self.read_text()</code>, <code>self.read_bytes()</code>, or <code>self.open(mode="r"|"rb")</code>.
+Returns <code>None</code> if the file hasn't been read from.</p>
+
+<p>Note: This property is only relative to the lifetime of this <code><a href="#Pathier">Pathier</a></code> instance, not the file itself.
+i.e. This property will reset if you create a new <code><a href="#Pathier">Pathier</a></code> object pointing to the same file.</p>
+</div>
+
+
+                            </div>
+                            <div id="Pathier.modified_since_last_read" class="classattr">
+                                <div class="attr variable">
+            <span class="name">modified_since_last_read</span><span class="annotation">: bool</span>
 
+        
     </div>
-    <a class="headerlink" href="#Pathier.size"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.size-65"><a href="#Pathier.size-65"><span class="linenos">65</span></a>    <span class="k">def</span> <span class="nf">size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="nb">format</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier.size-66"><a href="#Pathier.size-66"><span class="linenos">66</span></a>        <span class="sd">&quot;&quot;&quot;Returns the size in bytes of this file or directory.</span>
-</span><span id="Pathier.size-67"><a href="#Pathier.size-67"><span class="linenos">67</span></a><span class="sd">        Returns None if this path doesn&#39;t exist.</span>
-</span><span id="Pathier.size-68"><a href="#Pathier.size-68"><span class="linenos">68</span></a>
-</span><span id="Pathier.size-69"><a href="#Pathier.size-69"><span class="linenos">69</span></a><span class="sd">        :param format: If True, return value as a formatted string.&quot;&quot;&quot;</span>
-</span><span id="Pathier.size-70"><a href="#Pathier.size-70"><span class="linenos">70</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.size-71"><a href="#Pathier.size-71"><span class="linenos">71</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier.size-72"><a href="#Pathier.size-72"><span class="linenos">72</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.size-73"><a href="#Pathier.size-73"><span class="linenos">73</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span>
-</span><span id="Pathier.size-74"><a href="#Pathier.size-74"><span class="linenos">74</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.size-75"><a href="#Pathier.size-75"><span class="linenos">75</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="Pathier.size-76"><a href="#Pathier.size-76"><span class="linenos">76</span></a>        <span class="k">if</span> <span class="nb">format</span><span class="p">:</span>
-</span><span id="Pathier.size-77"><a href="#Pathier.size-77"><span class="linenos">77</span></a>            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">)</span>
-</span><span id="Pathier.size-78"><a href="#Pathier.size-78"><span class="linenos">78</span></a>        <span class="k">return</span> <span class="n">size</span>
-</span></pre></div>
+    <a class="headerlink" href="#Pathier.modified_since_last_read"></a>
+    
+            <div class="docstring"><p>Returns <code>True</code> if this file hasn't been read from or has been modified since the last time this object
+made a call to <code>self.read_text()</code>, <code>self.read_bytes()</code>, or <code>self.open(mode="r"|"rb")</code>.</p>
 
+<p>Note: This property is only relative to the lifetime of this <code><a href="#Pathier">Pathier</a></code> instance, not the file itself.
+i.e. This property will reset if you create a new <code><a href="#Pathier">Pathier</a></code> object pointing to the same file.</p>
 
-            <div class="docstring"><p>Returns the size in bytes of this file or directory.
-Returns None if this path doesn't exist.</p>
+<h4 id="caveat">Caveat:</h4>
 
-<h6 id="parameters">Parameters</h6>
+<p>May not be accurate if the file was modified within a couple of seconds of checking this property.
+(For instance, on my machine <code>self.mod_date</code> is consistently 1-1.5s in the future from when <code>self.write_text()</code> was called according to <code>time.time()</code>.)</p>
+</div>
+
+
+                            </div>
+                            <div id="Pathier.size" class="classattr">
+                                <div class="attr variable">
+            <span class="name">size</span><span class="annotation">: int</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Pathier.size"></a>
+    
+            <div class="docstring"><p>Returns the size in bytes of this file or directory.</p>
 
-<ul>
-<li><strong>format</strong>:  If True, return value as a formatted string.</li>
-</ul>
+<p>If this path doesn't exist, <code>0</code> will be returned.</p>
 </div>
 
 
                             </div>
-                            <div id="Pathier.format_size" class="classattr">
-                                        <input id="Pathier.format_size-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="Pathier.format_bytes" class="classattr">
+                                        <input id="Pathier.format_bytes-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
                     <div class="decorator">@staticmethod</div>
 
         <span class="def">def</span>
-        <span class="name">format_size</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">size</span><span class="p">:</span> <span class="nb">int</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
+        <span class="name">format_bytes</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">size</span><span class="p">:</span> <span class="nb">int</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
-                <label class="view-source-button" for="Pathier.format_size-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Pathier.format_bytes-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Pathier.format_size"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.format_size-80"><a href="#Pathier.format_size-80"><span class="linenos">80</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="Pathier.format_size-81"><a href="#Pathier.format_size-81"><span class="linenos">81</span></a>    <span class="k">def</span> <span class="nf">format_size</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Pathier.format_size-82"><a href="#Pathier.format_size-82"><span class="linenos">82</span></a>        <span class="sd">&quot;&quot;&quot;Format &#39;size&#39; with common file size abbreviations</span>
-</span><span id="Pathier.format_size-83"><a href="#Pathier.format_size-83"><span class="linenos">83</span></a><span class="sd">        and rounded to two decimal places.</span>
-</span><span id="Pathier.format_size-84"><a href="#Pathier.format_size-84"><span class="linenos">84</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier.format_size-85"><a href="#Pathier.format_size-85"><span class="linenos">85</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
-</span><span id="Pathier.format_size-86"><a href="#Pathier.format_size-86"><span class="linenos">86</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
-</span><span id="Pathier.format_size-87"><a href="#Pathier.format_size-87"><span class="linenos">87</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
-</span><span id="Pathier.format_size-88"><a href="#Pathier.format_size-88"><span class="linenos">88</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
-</span><span id="Pathier.format_size-89"><a href="#Pathier.format_size-89"><span class="linenos">89</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
+    <a class="headerlink" href="#Pathier.format_bytes"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.format_bytes-102"><a href="#Pathier.format_bytes-102"><span class="linenos">102</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="Pathier.format_bytes-103"><a href="#Pathier.format_bytes-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">format_bytes</span><span class="p">(</span><span class="n">size</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Pathier.format_bytes-104"><a href="#Pathier.format_bytes-104"><span class="linenos">104</span></a>        <span class="sd">&quot;&quot;&quot;Format `size` with common file size abbreviations and rounded to two decimal places.</span>
+</span><span id="Pathier.format_bytes-105"><a href="#Pathier.format_bytes-105"><span class="linenos">105</span></a><span class="sd">        &gt;&gt;&gt; 1234 -&gt; &quot;1.23 kb&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier.format_bytes-106"><a href="#Pathier.format_bytes-106"><span class="linenos">106</span></a>        <span class="k">for</span> <span class="n">unit</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;bytes&quot;</span><span class="p">,</span> <span class="s2">&quot;kb&quot;</span><span class="p">,</span> <span class="s2">&quot;mb&quot;</span><span class="p">,</span> <span class="s2">&quot;gb&quot;</span><span class="p">,</span> <span class="s2">&quot;tb&quot;</span><span class="p">,</span> <span class="s2">&quot;pb&quot;</span><span class="p">]:</span>
+</span><span id="Pathier.format_bytes-107"><a href="#Pathier.format_bytes-107"><span class="linenos">107</span></a>            <span class="k">if</span> <span class="n">unit</span> <span class="o">!=</span> <span class="s2">&quot;bytes&quot;</span><span class="p">:</span>
+</span><span id="Pathier.format_bytes-108"><a href="#Pathier.format_bytes-108"><span class="linenos">108</span></a>                <span class="n">size</span> <span class="o">*=</span> <span class="mf">0.001</span>
+</span><span id="Pathier.format_bytes-109"><a href="#Pathier.format_bytes-109"><span class="linenos">109</span></a>            <span class="k">if</span> <span class="n">size</span> <span class="o">&lt;</span> <span class="mi">1000</span> <span class="ow">or</span> <span class="n">unit</span> <span class="o">==</span> <span class="s2">&quot;pb&quot;</span><span class="p">:</span>
+</span><span id="Pathier.format_bytes-110"><a href="#Pathier.format_bytes-110"><span class="linenos">110</span></a>                <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">round</span><span class="p">(</span><span class="n">size</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">unit</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Format 'size' with common file size abbreviations
-and rounded to two decimal places.</p>
+            <div class="docstring"><p>Format <code><a href="#Pathier.size">size</a></code> with common file size abbreviations and rounded to two decimal places.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="mi">1234</span> <span class="o">-&gt;</span> <span class="s2">&quot;1.23 kb&quot;</span>
 </code></pre>
 </div>
 </div>
 
@@ -682,23 +838,21 @@
         <span class="def">def</span>
         <span class="name">is_larger</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.is_larger-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.is_larger"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_larger-91"><a href="#Pathier.is_larger-91"><span class="linenos">91</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.is_larger-92"><a href="#Pathier.is_larger-92"><span class="linenos">92</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than</span>
-</span><span id="Pathier.is_larger-93"><a href="#Pathier.is_larger-93"><span class="linenos">93</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier.is_larger-94"><a href="#Pathier.is_larger-94"><span class="linenos">94</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_larger-112"><a href="#Pathier.is_larger-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">is_larger</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.is_larger-113"><a href="#Pathier.is_larger-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is larger than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.is_larger-114"><a href="#Pathier.is_larger-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Returns whether this file or folder is larger than
-the one pointed to by 'path'.</p>
+            <div class="docstring"><p>Returns whether this file or folder is larger than the one pointed to by <code>path</code>.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.is_older" class="classattr">
                                         <input id="Pathier.is_older-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -706,23 +860,21 @@
         <span class="def">def</span>
         <span class="name">is_older</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.is_older-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.is_older"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_older-96"><a href="#Pathier.is_older-96"><span class="linenos">96</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.is_older-97"><a href="#Pathier.is_older-97"><span class="linenos">97</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than</span>
-</span><span id="Pathier.is_older-98"><a href="#Pathier.is_older-98"><span class="linenos">98</span></a><span class="sd">        the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier.is_older-99"><a href="#Pathier.is_older-99"><span class="linenos">99</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.is_older-116"><a href="#Pathier.is_older-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">is_older</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.is_older-117"><a href="#Pathier.is_older-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder is older than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.is_older-118"><a href="#Pathier.is_older-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">dob</span> <span class="o">&lt;</span> <span class="n">path</span><span class="o">.</span><span class="n">dob</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Returns whether this file or folder is older than
-the one pointed to by 'path'.</p>
+            <div class="docstring"><p>Returns whether this file or folder is older than the one pointed to by <code>path</code>.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.modified_more_recently" class="classattr">
                                         <input id="Pathier.modified_more_recently-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -730,23 +882,21 @@
         <span class="def">def</span>
         <span class="name">modified_more_recently</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">path</span><span class="p">:</span> <span class="n">Self</span></span><span class="return-annotation">) -> <span class="nb">bool</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.modified_more_recently-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.modified_more_recently"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.modified_more_recently-101"><a href="#Pathier.modified_more_recently-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-</span><span id="Pathier.modified_more_recently-102"><a href="#Pathier.modified_more_recently-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified</span>
-</span><span id="Pathier.modified_more_recently-103"><a href="#Pathier.modified_more_recently-103"><span class="linenos">103</span></a><span class="sd">        more recently than the one pointed to by &#39;path&#39;.&quot;&quot;&quot;</span>
-</span><span id="Pathier.modified_more_recently-104"><a href="#Pathier.modified_more_recently-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.modified_more_recently-120"><a href="#Pathier.modified_more_recently-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">modified_more_recently</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">path</span><span class="p">:</span> <span class="n">Self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+</span><span id="Pathier.modified_more_recently-121"><a href="#Pathier.modified_more_recently-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Returns whether this file or folder was modified more recently than the one pointed to by `path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.modified_more_recently-122"><a href="#Pathier.modified_more_recently-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">mod_date</span> <span class="o">&gt;</span> <span class="n">path</span><span class="o">.</span><span class="n">mod_date</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Returns whether this file or folder was modified
-more recently than the one pointed to by 'path'.</p>
+            <div class="docstring"><p>Returns whether this file or folder was modified more recently than the one pointed to by <code>path</code>.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.mkcwd" class="classattr">
                                         <input id="Pathier.mkcwd-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -754,17 +904,17 @@
         <span class="def">def</span>
         <span class="name">mkcwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.mkcwd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.mkcwd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkcwd-107"><a href="#Pathier.mkcwd-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.mkcwd-108"><a href="#Pathier.mkcwd-108"><span class="linenos">108</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier.mkcwd-109"><a href="#Pathier.mkcwd-109"><span class="linenos">109</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkcwd-125"><a href="#Pathier.mkcwd-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">mkcwd</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.mkcwd-126"><a href="#Pathier.mkcwd-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Make this path your current working directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier.mkcwd-127"><a href="#Pathier.mkcwd-127"><span class="linenos">127</span></a>        <span class="n">os</span><span class="o">.</span><span class="n">chdir</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make this path your current working directory.</p>
 </div>
 
 
@@ -773,16 +923,15 @@
                                 <div class="attr variable">
             <span class="name">in_PATH</span><span class="annotation">: bool</span>
 
         
     </div>
     <a class="headerlink" href="#Pathier.in_PATH"></a>
     
-            <div class="docstring"><p>Return True if this
-path is in sys.path.</p>
+            <div class="docstring"><p>Return <code>True</code> if this path is in <code>sys.path</code>.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.add_to_PATH" class="classattr">
                                         <input id="Pathier.add_to_PATH-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -790,35 +939,31 @@
         <span class="def">def</span>
         <span class="name">add_to_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.add_to_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.add_to_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.add_to_PATH-117"><a href="#Pathier.add_to_PATH-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
-</span><span id="Pathier.add_to_PATH-118"><a href="#Pathier.add_to_PATH-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into sys.path</span>
-</span><span id="Pathier.add_to_PATH-119"><a href="#Pathier.add_to_PATH-119"><span class="linenos">119</span></a><span class="sd">        if it isn&#39;t already there.</span>
-</span><span id="Pathier.add_to_PATH-120"><a href="#Pathier.add_to_PATH-120"><span class="linenos">120</span></a>
-</span><span id="Pathier.add_to_PATH-121"><a href="#Pathier.add_to_PATH-121"><span class="linenos">121</span></a><span class="sd">        :param index: The index of sys.path</span>
-</span><span id="Pathier.add_to_PATH-122"><a href="#Pathier.add_to_PATH-122"><span class="linenos">122</span></a><span class="sd">        to insert this path at.&quot;&quot;&quot;</span>
-</span><span id="Pathier.add_to_PATH-123"><a href="#Pathier.add_to_PATH-123"><span class="linenos">123</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier.add_to_PATH-124"><a href="#Pathier.add_to_PATH-124"><span class="linenos">124</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.add_to_PATH-125"><a href="#Pathier.add_to_PATH-125"><span class="linenos">125</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.add_to_PATH-134"><a href="#Pathier.add_to_PATH-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">add_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">):</span>
+</span><span id="Pathier.add_to_PATH-135"><a href="#Pathier.add_to_PATH-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Insert this path into `sys.path` if it isn&#39;t already there.</span>
+</span><span id="Pathier.add_to_PATH-136"><a href="#Pathier.add_to_PATH-136"><span class="linenos">136</span></a>
+</span><span id="Pathier.add_to_PATH-137"><a href="#Pathier.add_to_PATH-137"><span class="linenos">137</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.add_to_PATH-138"><a href="#Pathier.add_to_PATH-138"><span class="linenos">138</span></a>
+</span><span id="Pathier.add_to_PATH-139"><a href="#Pathier.add_to_PATH-139"><span class="linenos">139</span></a><span class="sd">        `index`: The index of `sys.path` to insert this path at.&quot;&quot;&quot;</span>
+</span><span id="Pathier.add_to_PATH-140"><a href="#Pathier.add_to_PATH-140"><span class="linenos">140</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier.add_to_PATH-141"><a href="#Pathier.add_to_PATH-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.add_to_PATH-142"><a href="#Pathier.add_to_PATH-142"><span class="linenos">142</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="n">path</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Insert this path into sys.path
-if it isn't already there.</p>
-
-<h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><strong>index</strong>:  The index of sys.path
-to insert this path at.</li>
-</ul>
+            <div class="docstring"><p>Insert this path into <code>sys.path</code> if it isn't already there.</p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>index</code>: The index of <code>sys.path</code> to insert this path at.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.append_to_PATH" class="classattr">
                                         <input id="Pathier.append_to_PATH-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -826,25 +971,23 @@
         <span class="def">def</span>
         <span class="name">append_to_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.append_to_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.append_to_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append_to_PATH-127"><a href="#Pathier.append_to_PATH-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.append_to_PATH-128"><a href="#Pathier.append_to_PATH-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to sys.path</span>
-</span><span id="Pathier.append_to_PATH-129"><a href="#Pathier.append_to_PATH-129"><span class="linenos">129</span></a><span class="sd">        if it isn&#39;t already there.&quot;&quot;&quot;</span>
-</span><span id="Pathier.append_to_PATH-130"><a href="#Pathier.append_to_PATH-130"><span class="linenos">130</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
-</span><span id="Pathier.append_to_PATH-131"><a href="#Pathier.append_to_PATH-131"><span class="linenos">131</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.append_to_PATH-132"><a href="#Pathier.append_to_PATH-132"><span class="linenos">132</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append_to_PATH-144"><a href="#Pathier.append_to_PATH-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">append_to_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.append_to_PATH-145"><a href="#Pathier.append_to_PATH-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Append this path to `sys.path` if it isn&#39;t already there.&quot;&quot;&quot;</span>
+</span><span id="Pathier.append_to_PATH-146"><a href="#Pathier.append_to_PATH-146"><span class="linenos">146</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+</span><span id="Pathier.append_to_PATH-147"><a href="#Pathier.append_to_PATH-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.append_to_PATH-148"><a href="#Pathier.append_to_PATH-148"><span class="linenos">148</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Append this path to sys.path
-if it isn't already there.</p>
+            <div class="docstring"><p>Append this path to <code>sys.path</code> if it isn't already there.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.remove_from_PATH" class="classattr">
                                         <input id="Pathier.remove_from_PATH-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -852,24 +995,22 @@
         <span class="def">def</span>
         <span class="name">remove_from_PATH</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.remove_from_PATH-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.remove_from_PATH"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.remove_from_PATH-134"><a href="#Pathier.remove_from_PATH-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.remove_from_PATH-135"><a href="#Pathier.remove_from_PATH-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from sys.path</span>
-</span><span id="Pathier.remove_from_PATH-136"><a href="#Pathier.remove_from_PATH-136"><span class="linenos">136</span></a><span class="sd">        if it&#39;s in sys.path.&quot;&quot;&quot;</span>
-</span><span id="Pathier.remove_from_PATH-137"><a href="#Pathier.remove_from_PATH-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
-</span><span id="Pathier.remove_from_PATH-138"><a href="#Pathier.remove_from_PATH-138"><span class="linenos">138</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.remove_from_PATH-150"><a href="#Pathier.remove_from_PATH-150"><span class="linenos">150</span></a>    <span class="k">def</span> <span class="nf">remove_from_PATH</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.remove_from_PATH-151"><a href="#Pathier.remove_from_PATH-151"><span class="linenos">151</span></a>        <span class="sd">&quot;&quot;&quot;Remove this path from `sys.path` if it&#39;s in `sys.path`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.remove_from_PATH-152"><a href="#Pathier.remove_from_PATH-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">in_PATH</span><span class="p">:</span>
+</span><span id="Pathier.remove_from_PATH-153"><a href="#Pathier.remove_from_PATH-153"><span class="linenos">153</span></a>            <span class="n">sys</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">remove</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="bp">self</span><span class="p">))</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Remove this path from sys.path
-if it's in sys.path.</p>
+            <div class="docstring"><p>Remove this path from <code>sys.path</code> if it's in <code>sys.path</code>.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.moveup" class="classattr">
                                         <input id="Pathier.moveup-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -877,30 +1018,32 @@
         <span class="def">def</span>
         <span class="name">moveup</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.moveup-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.moveup"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.moveup-140"><a href="#Pathier.moveup-140"><span class="linenos">140</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.moveup-141"><a href="#Pathier.moveup-141"><span class="linenos">141</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is a parent of this instance.</span>
-</span><span id="Pathier.moveup-142"><a href="#Pathier.moveup-142"><span class="linenos">142</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier.moveup-143"><a href="#Pathier.moveup-143"><span class="linenos">143</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
-</span><span id="Pathier.moveup-144"><a href="#Pathier.moveup-144"><span class="linenos">144</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
-</span><span id="Pathier.moveup-145"><a href="#Pathier.moveup-145"><span class="linenos">145</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
-</span><span id="Pathier.moveup-146"><a href="#Pathier.moveup-146"><span class="linenos">146</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
-</span><span id="Pathier.moveup-147"><a href="#Pathier.moveup-147"><span class="linenos">147</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
-</span><span id="Pathier.moveup-148"><a href="#Pathier.moveup-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.moveup-149"><a href="#Pathier.moveup-149"><span class="linenos">149</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.moveup-150"><a href="#Pathier.moveup-150"><span class="linenos">150</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.moveup-155"><a href="#Pathier.moveup-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">moveup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.moveup-156"><a href="#Pathier.moveup-156"><span class="linenos">156</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is a parent of this instance.</span>
+</span><span id="Pathier.moveup-157"><a href="#Pathier.moveup-157"><span class="linenos">157</span></a>
+</span><span id="Pathier.moveup-158"><a href="#Pathier.moveup-158"><span class="linenos">158</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier.moveup-159"><a href="#Pathier.moveup-159"><span class="linenos">159</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;C:\some\directory\in\your\system&quot;)</span>
+</span><span id="Pathier.moveup-160"><a href="#Pathier.moveup-160"><span class="linenos">160</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;directory&quot;))</span>
+</span><span id="Pathier.moveup-161"><a href="#Pathier.moveup-161"><span class="linenos">161</span></a><span class="sd">        &gt;&gt;&gt; &quot;C:\some\directory&quot;</span>
+</span><span id="Pathier.moveup-162"><a href="#Pathier.moveup-162"><span class="linenos">162</span></a><span class="sd">        &gt;&gt;&gt; print(p.moveup(&quot;yeet&quot;))</span>
+</span><span id="Pathier.moveup-163"><a href="#Pathier.moveup-163"><span class="linenos">163</span></a><span class="sd">        &gt;&gt;&gt; &quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot; &quot;&quot;&quot;</span>
+</span><span id="Pathier.moveup-164"><a href="#Pathier.moveup-164"><span class="linenos">164</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.moveup-165"><a href="#Pathier.moveup-165"><span class="linenos">165</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.moveup-166"><a href="#Pathier.moveup-166"><span class="linenos">166</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[:</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span><span class="p">]))</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Return a new Pathier object that is a parent of this instance.
-'name' is case-sensitive and raises an exception if it isn't in self.parts.</p>
+            <div class="docstring"><p>Return a new <code><a href="#Pathier">Pathier</a></code> object that is a parent of this instance.</p>
+
+<p><code><a href="#Pathier.name">name</a></code> is case-sensitive and raises an exception if it isn't in <code>self.parts</code>.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">p</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;C:\some\directory\in\your\system&quot;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="nb">print</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">moveup</span><span class="p">(</span><span class="s2">&quot;directory&quot;</span><span class="p">))</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="s2">&quot;C:\some\directory&quot;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="nb">print</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">moveup</span><span class="p">(</span><span class="s2">&quot;yeet&quot;</span><span class="p">))</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="s2">&quot;Exception: yeet is not a parent of C:\some\directory\in\your\system&quot;</span>
@@ -917,30 +1060,30 @@
         <span class="def">def</span>
         <span class="name">move_under</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.move_under-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.move_under"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.move_under-163"><a href="#Pathier.move_under-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.move_under-164"><a href="#Pathier.move_under-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object such that the stem</span>
-</span><span id="Pathier.move_under-165"><a href="#Pathier.move_under-165"><span class="linenos">165</span></a><span class="sd">        is one level below the folder &#39;name&#39;.</span>
-</span><span id="Pathier.move_under-166"><a href="#Pathier.move_under-166"><span class="linenos">166</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier.move_under-167"><a href="#Pathier.move_under-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier.move_under-168"><a href="#Pathier.move_under-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
-</span><span id="Pathier.move_under-169"><a href="#Pathier.move_under-169"><span class="linenos">169</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier.move_under-170"><a href="#Pathier.move_under-170"><span class="linenos">170</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.move_under-171"><a href="#Pathier.move_under-171"><span class="linenos">171</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.move_under-172"><a href="#Pathier.move_under-172"><span class="linenos">172</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.move_under-179"><a href="#Pathier.move_under-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">move_under</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.move_under-180"><a href="#Pathier.move_under-180"><span class="linenos">180</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object such that the stem is one level below the given folder `name`.</span>
+</span><span id="Pathier.move_under-181"><a href="#Pathier.move_under-181"><span class="linenos">181</span></a>
+</span><span id="Pathier.move_under-182"><a href="#Pathier.move_under-182"><span class="linenos">182</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier.move_under-183"><a href="#Pathier.move_under-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier.move_under-184"><a href="#Pathier.move_under-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; print(p.move_under(&quot;c&quot;))</span>
+</span><span id="Pathier.move_under-185"><a href="#Pathier.move_under-185"><span class="linenos">185</span></a><span class="sd">        &gt;&gt;&gt; &#39;a/b/c/d&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier.move_under-186"><a href="#Pathier.move_under-186"><span class="linenos">186</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.move_under-187"><a href="#Pathier.move_under-187"><span class="linenos">187</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.move_under-188"><a href="#Pathier.move_under-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="bp">self</span> <span class="o">-</span> <span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">)</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">-</span> <span class="mi">2</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Return a new Pathier object such that the stem
-is one level below the folder 'name'.
-'name' is case-sensitive and raises an exception if it isn't in self.parts.</p>
+            <div class="docstring"><p>Return a new <code><a href="#Pathier">Pathier</a></code> object such that the stem is one level below the given folder <code><a href="#Pathier.name">name</a></code>.</p>
+
+<p><code><a href="#Pathier.name">name</a></code> is case-sensitive and raises an exception if it isn't in <code>self.parts</code>.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">p</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;a/b/c/d/e/f/g&quot;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="nb">print</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">move_under</span><span class="p">(</span><span class="s2">&quot;c&quot;</span><span class="p">))</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="s1">&#39;a/b/c/d&#39;</span>
 </code></pre>
 </div>
@@ -955,47 +1098,51 @@
         <span class="def">def</span>
         <span class="name">separate</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.separate-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.separate"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.separate-174"><a href="#Pathier.separate-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.separate-175"><a href="#Pathier.separate-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Return a new Pathier object that is the</span>
-</span><span id="Pathier.separate-176"><a href="#Pathier.separate-176"><span class="linenos">176</span></a><span class="sd">        relative child path after &#39;name&#39;.</span>
-</span><span id="Pathier.separate-177"><a href="#Pathier.separate-177"><span class="linenos">177</span></a><span class="sd">        &#39;name&#39; is case-sensitive and raises an exception if it isn&#39;t in self.parts.</span>
-</span><span id="Pathier.separate-178"><a href="#Pathier.separate-178"><span class="linenos">178</span></a>
-</span><span id="Pathier.separate-179"><a href="#Pathier.separate-179"><span class="linenos">179</span></a><span class="sd">        :param keep_name: If True, the returned path will start with &#39;name&#39;.</span>
-</span><span id="Pathier.separate-180"><a href="#Pathier.separate-180"><span class="linenos">180</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
-</span><span id="Pathier.separate-181"><a href="#Pathier.separate-181"><span class="linenos">181</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
-</span><span id="Pathier.separate-182"><a href="#Pathier.separate-182"><span class="linenos">182</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
-</span><span id="Pathier.separate-183"><a href="#Pathier.separate-183"><span class="linenos">183</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
-</span><span id="Pathier.separate-184"><a href="#Pathier.separate-184"><span class="linenos">184</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
-</span><span id="Pathier.separate-185"><a href="#Pathier.separate-185"><span class="linenos">185</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
-</span><span id="Pathier.separate-186"><a href="#Pathier.separate-186"><span class="linenos">186</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Pathier.separate-187"><a href="#Pathier.separate-187"><span class="linenos">187</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
-</span><span id="Pathier.separate-188"><a href="#Pathier.separate-188"><span class="linenos">188</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
-</span><span id="Pathier.separate-189"><a href="#Pathier.separate-189"><span class="linenos">189</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.separate-190"><a href="#Pathier.separate-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">separate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">keep_name</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.separate-191"><a href="#Pathier.separate-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Return a new `Pathier` object that is the relative child path after `name`.</span>
+</span><span id="Pathier.separate-192"><a href="#Pathier.separate-192"><span class="linenos">192</span></a>
+</span><span id="Pathier.separate-193"><a href="#Pathier.separate-193"><span class="linenos">193</span></a><span class="sd">        `name` is case-sensitive and raises an exception if it isn&#39;t in `self.parts`.</span>
+</span><span id="Pathier.separate-194"><a href="#Pathier.separate-194"><span class="linenos">194</span></a>
+</span><span id="Pathier.separate-195"><a href="#Pathier.separate-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.separate-196"><a href="#Pathier.separate-196"><span class="linenos">196</span></a>
+</span><span id="Pathier.separate-197"><a href="#Pathier.separate-197"><span class="linenos">197</span></a><span class="sd">        `keep_name`: If `True`, the returned path will start with `name`.</span>
+</span><span id="Pathier.separate-198"><a href="#Pathier.separate-198"><span class="linenos">198</span></a><span class="sd">        &gt;&gt;&gt; p = Pathier(&quot;a/b/c/d/e/f/g&quot;)</span>
+</span><span id="Pathier.separate-199"><a href="#Pathier.separate-199"><span class="linenos">199</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;))</span>
+</span><span id="Pathier.separate-200"><a href="#Pathier.separate-200"><span class="linenos">200</span></a><span class="sd">        &gt;&gt;&gt; &#39;d/e/f/g&#39;</span>
+</span><span id="Pathier.separate-201"><a href="#Pathier.separate-201"><span class="linenos">201</span></a><span class="sd">        &gt;&gt;&gt; print(p.separate(&quot;c&quot;, True))</span>
+</span><span id="Pathier.separate-202"><a href="#Pathier.separate-202"><span class="linenos">202</span></a><span class="sd">        &gt;&gt;&gt; &#39;c/d/e/f/g&#39;&quot;&quot;&quot;</span>
+</span><span id="Pathier.separate-203"><a href="#Pathier.separate-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">:</span>
+</span><span id="Pathier.separate-204"><a href="#Pathier.separate-204"><span class="linenos">204</span></a>            <span class="k">raise</span> <span class="ne">Exception</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> is not a parent of </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Pathier.separate-205"><a href="#Pathier.separate-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="n">keep_name</span><span class="p">:</span>
+</span><span id="Pathier.separate-206"><a href="#Pathier.separate-206"><span class="linenos">206</span></a>            <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="p">:])</span>
+</span><span id="Pathier.separate-207"><a href="#Pathier.separate-207"><span class="linenos">207</span></a>        <span class="k">return</span> <span class="n">Pathier</span><span class="p">(</span><span class="o">*</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">parts</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">name</span><span class="p">)</span> <span class="o">+</span> <span class="mi">1</span> <span class="p">:])</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Return a new Pathier object that is the
-relative child path after 'name'.
-'name' is case-sensitive and raises an exception if it isn't in self.parts.</p>
-
-<h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><strong>keep_name</strong>:  If True, the returned path will start with 'name'.
-&gt;&gt;&gt; p = Pathier("a/b/c/d/e/f/g")
-&gt;&gt;&gt; print(p.separate("c"))
-&gt;&gt;&gt; 'd/e/f/g'
-&gt;&gt;&gt; print(p.separate("c", True))
-&gt;&gt;&gt; 'c/d/e/f/g'</li>
-</ul>
+            <div class="docstring"><p>Return a new <code><a href="#Pathier">Pathier</a></code> object that is the relative child path after <code><a href="#Pathier.name">name</a></code>.</p>
+
+<p><code><a href="#Pathier.name">name</a></code> is case-sensitive and raises an exception if it isn't in <code>self.parts</code>.</p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>keep_name</code>: If <code>True</code>, the returned path will start with <code><a href="#Pathier.name">name</a></code>.</p>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">p</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;a/b/c/d/e/f/g&quot;</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="nb">print</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="s2">&quot;c&quot;</span><span class="p">))</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="s1">&#39;d/e/f/g&#39;</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="nb">print</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="s2">&quot;c&quot;</span><span class="p">,</span> <span class="kc">True</span><span class="p">))</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="s1">&#39;c/d/e/f/g&#39;</span>
+</code></pre>
+</div>
 </div>
 
 
                             </div>
                             <div id="Pathier.mkdir" class="classattr">
                                         <input id="Pathier.mkdir-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1003,27 +1150,25 @@
         <span class="def">def</span>
         <span class="name">mkdir</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span>, </span><span class="param"><span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>, </span><span class="param"><span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.mkdir-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.mkdir"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkdir-192"><a href="#Pathier.mkdir-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.mkdir-193"><a href="#Pathier.mkdir-193"><span class="linenos">193</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
-</span><span id="Pathier.mkdir-194"><a href="#Pathier.mkdir-194"><span class="linenos">194</span></a><span class="sd">        Same as Path().mkdir() except</span>
-</span><span id="Pathier.mkdir-195"><a href="#Pathier.mkdir-195"><span class="linenos">195</span></a><span class="sd">        &#39;parents&#39; and &#39;exist_ok&#39; default</span>
-</span><span id="Pathier.mkdir-196"><a href="#Pathier.mkdir-196"><span class="linenos">196</span></a><span class="sd">        to True instead of False.&quot;&quot;&quot;</span>
-</span><span id="Pathier.mkdir-197"><a href="#Pathier.mkdir-197"><span class="linenos">197</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.mkdir-210"><a href="#Pathier.mkdir-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">mkdir</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">511</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.mkdir-211"><a href="#Pathier.mkdir-211"><span class="linenos">211</span></a>        <span class="sd">&quot;&quot;&quot;Create this directory.</span>
+</span><span id="Pathier.mkdir-212"><a href="#Pathier.mkdir-212"><span class="linenos">212</span></a>
+</span><span id="Pathier.mkdir-213"><a href="#Pathier.mkdir-213"><span class="linenos">213</span></a><span class="sd">        Same as `Path().mkdir()` except `parents` and `exist_ok` default to `True` instead of `False`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.mkdir-214"><a href="#Pathier.mkdir-214"><span class="linenos">214</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">parents</span><span class="p">,</span> <span class="n">exist_ok</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Create this directory.
-Same as Path().mkdir() except
-'parents' and 'exist_ok' default
-to True instead of False.</p>
+            <div class="docstring"><p>Create this directory.</p>
+
+<p>Same as <code>Path().mkdir()</code> except <code><a href="#Pathier.parents">parents</a></code> and <code>exist_ok</code> default to <code>True</code> instead of <code>False</code>.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.touch" class="classattr">
                                         <input id="Pathier.touch-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1031,22 +1176,51 @@
         <span class="def">def</span>
         <span class="name">touch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.touch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.touch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.touch-199"><a href="#Pathier.touch-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Pathier.touch-200"><a href="#Pathier.touch-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Create file and parents if necessary.&quot;&quot;&quot;</span>
-</span><span id="Pathier.touch-201"><a href="#Pathier.touch-201"><span class="linenos">201</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
-</span><span id="Pathier.touch-202"><a href="#Pathier.touch-202"><span class="linenos">202</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.touch-216"><a href="#Pathier.touch-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">touch</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Pathier.touch-217"><a href="#Pathier.touch-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Create file (and parents if necessary).&quot;&quot;&quot;</span>
+</span><span id="Pathier.touch-218"><a href="#Pathier.touch-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">()</span>
+</span><span id="Pathier.touch-219"><a href="#Pathier.touch-219"><span class="linenos">219</span></a>        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">touch</span><span class="p">()</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Create file (and parents if necessary).</p>
+</div>
+
+
+                            </div>
+                            <div id="Pathier.open" class="classattr">
+                                        <input id="Pathier.open-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">open</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">mode</span><span class="o">=</span><span class="s1">&#39;r&#39;</span>,</span><span class="param">	<span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span>,</span><span class="param">	<span class="n">encoding</span><span class="o">=</span><span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="o">=</span><span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="o">=</span><span class="kc">None</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Pathier.open-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Pathier.open"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.open-221"><a href="#Pathier.open-221"><span class="linenos">221</span></a>    <span class="k">def</span> <span class="nf">open</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mode</span><span class="o">=</span><span class="s2">&quot;r&quot;</span><span class="p">,</span> <span class="n">buffering</span><span class="o">=-</span><span class="mi">1</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">newline</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier.open-222"><a href="#Pathier.open-222"><span class="linenos">222</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Pathier.open-223"><a href="#Pathier.open-223"><span class="linenos">223</span></a><span class="sd">        Open the file pointed by this path and return a file object, as</span>
+</span><span id="Pathier.open-224"><a href="#Pathier.open-224"><span class="linenos">224</span></a><span class="sd">        the built-in open() function does.</span>
+</span><span id="Pathier.open-225"><a href="#Pathier.open-225"><span class="linenos">225</span></a><span class="sd">        &quot;&quot;&quot;</span>
+</span><span id="Pathier.open-226"><a href="#Pathier.open-226"><span class="linenos">226</span></a>        <span class="n">stream</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="n">mode</span><span class="p">,</span> <span class="n">buffering</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">)</span>
+</span><span id="Pathier.open-227"><a href="#Pathier.open-227"><span class="linenos">227</span></a>        <span class="k">if</span> <span class="s2">&quot;r&quot;</span> <span class="ow">in</span> <span class="n">mode</span><span class="p">:</span>
+</span><span id="Pathier.open-228"><a href="#Pathier.open-228"><span class="linenos">228</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_last_read_time</span> <span class="o">=</span> <span class="n">time</span><span class="o">.</span><span class="n">time</span><span class="p">()</span>
+</span><span id="Pathier.open-229"><a href="#Pathier.open-229"><span class="linenos">229</span></a>        <span class="k">return</span> <span class="n">stream</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Create file and parents if necessary.</p>
+            <div class="docstring"><p>Open the file pointed by this path and return a file object, as
+the built-in open() function does.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.write_text" class="classattr">
                                         <input id="Pathier.write_text-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1054,52 +1228,54 @@
         <span class="def">def</span>
         <span class="name">write_text</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.write_text-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.write_text"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_text-204"><a href="#Pathier.write_text-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
-</span><span id="Pathier.write_text-205"><a href="#Pathier.write_text-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.write_text-206"><a href="#Pathier.write_text-206"><span class="linenos">206</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.write_text-207"><a href="#Pathier.write_text-207"><span class="linenos">207</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-208"><a href="#Pathier.write_text-208"><span class="linenos">208</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-209"><a href="#Pathier.write_text-209"><span class="linenos">209</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.write_text-210"><a href="#Pathier.write_text-210"><span class="linenos">210</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.write_text-211"><a href="#Pathier.write_text-211"><span class="linenos">211</span></a>    <span class="p">):</span>
-</span><span id="Pathier.write_text-212"><a href="#Pathier.write_text-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file. If a TypeError is raised, the function</span>
-</span><span id="Pathier.write_text-213"><a href="#Pathier.write_text-213"><span class="linenos">213</span></a><span class="sd">        will attempt to case data to a str and try the write again.</span>
-</span><span id="Pathier.write_text-214"><a href="#Pathier.write_text-214"><span class="linenos">214</span></a><span class="sd">        If a FileNotFoundError is raised and parents = True,</span>
-</span><span id="Pathier.write_text-215"><a href="#Pathier.write_text-215"><span class="linenos">215</span></a><span class="sd">        self.parent will be created.&quot;&quot;&quot;</span>
-</span><span id="Pathier.write_text-216"><a href="#Pathier.write_text-216"><span class="linenos">216</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
-</span><span id="Pathier.write_text-217"><a href="#Pathier.write_text-217"><span class="linenos">217</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
-</span><span id="Pathier.write_text-218"><a href="#Pathier.write_text-218"><span class="linenos">218</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier.write_text-219"><a href="#Pathier.write_text-219"><span class="linenos">219</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier.write_text-220"><a href="#Pathier.write_text-220"><span class="linenos">220</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier.write_text-221"><a href="#Pathier.write_text-221"><span class="linenos">221</span></a>        <span class="p">)</span>
-</span><span id="Pathier.write_text-222"><a href="#Pathier.write_text-222"><span class="linenos">222</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier.write_text-223"><a href="#Pathier.write_text-223"><span class="linenos">223</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-224"><a href="#Pathier.write_text-224"><span class="linenos">224</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
-</span><span id="Pathier.write_text-225"><a href="#Pathier.write_text-225"><span class="linenos">225</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-226"><a href="#Pathier.write_text-226"><span class="linenos">226</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-227"><a href="#Pathier.write_text-227"><span class="linenos">227</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier.write_text-228"><a href="#Pathier.write_text-228"><span class="linenos">228</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier.write_text-229"><a href="#Pathier.write_text-229"><span class="linenos">229</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.write_text-230"><a href="#Pathier.write_text-230"><span class="linenos">230</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_text-231"><a href="#Pathier.write_text-231"><span class="linenos">231</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.write_text-232"><a href="#Pathier.write_text-232"><span class="linenos">232</span></a>                <span class="k">raise</span>
-</span><span id="Pathier.write_text-233"><a href="#Pathier.write_text-233"><span class="linenos">233</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier.write_text-234"><a href="#Pathier.write_text-234"><span class="linenos">234</span></a>            <span class="k">raise</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_text-231"><a href="#Pathier.write_text-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">write_text</span><span class="p">(</span>
+</span><span id="Pathier.write_text-232"><a href="#Pathier.write_text-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.write_text-233"><a href="#Pathier.write_text-233"><span class="linenos">233</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.write_text-234"><a href="#Pathier.write_text-234"><span class="linenos">234</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-235"><a href="#Pathier.write_text-235"><span class="linenos">235</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-236"><a href="#Pathier.write_text-236"><span class="linenos">236</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.write_text-237"><a href="#Pathier.write_text-237"><span class="linenos">237</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.write_text-238"><a href="#Pathier.write_text-238"><span class="linenos">238</span></a>    <span class="p">):</span>
+</span><span id="Pathier.write_text-239"><a href="#Pathier.write_text-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Write data to file.</span>
+</span><span id="Pathier.write_text-240"><a href="#Pathier.write_text-240"><span class="linenos">240</span></a>
+</span><span id="Pathier.write_text-241"><a href="#Pathier.write_text-241"><span class="linenos">241</span></a><span class="sd">        If a `TypeError` is raised, the function  will attempt to cast `data` to a `str` and try the write again.</span>
+</span><span id="Pathier.write_text-242"><a href="#Pathier.write_text-242"><span class="linenos">242</span></a>
+</span><span id="Pathier.write_text-243"><a href="#Pathier.write_text-243"><span class="linenos">243</span></a><span class="sd">        If a `FileNotFoundError` is raised and `parents = True`, `self.parent` will be created.&quot;&quot;&quot;</span>
+</span><span id="Pathier.write_text-244"><a href="#Pathier.write_text-244"><span class="linenos">244</span></a>        <span class="n">write</span> <span class="o">=</span> <span class="n">functools</span><span class="o">.</span><span class="n">partial</span><span class="p">(</span>
+</span><span id="Pathier.write_text-245"><a href="#Pathier.write_text-245"><span class="linenos">245</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_text</span><span class="p">,</span>
+</span><span id="Pathier.write_text-246"><a href="#Pathier.write_text-246"><span class="linenos">246</span></a>            <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier.write_text-247"><a href="#Pathier.write_text-247"><span class="linenos">247</span></a>            <span class="n">errors</span><span class="o">=</span><span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier.write_text-248"><a href="#Pathier.write_text-248"><span class="linenos">248</span></a>            <span class="n">newline</span><span class="o">=</span><span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier.write_text-249"><a href="#Pathier.write_text-249"><span class="linenos">249</span></a>        <span class="p">)</span>
+</span><span id="Pathier.write_text-250"><a href="#Pathier.write_text-250"><span class="linenos">250</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier.write_text-251"><a href="#Pathier.write_text-251"><span class="linenos">251</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-252"><a href="#Pathier.write_text-252"><span class="linenos">252</span></a>        <span class="k">except</span> <span class="ne">TypeError</span><span class="p">:</span>
+</span><span id="Pathier.write_text-253"><a href="#Pathier.write_text-253"><span class="linenos">253</span></a>            <span class="n">data</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-254"><a href="#Pathier.write_text-254"><span class="linenos">254</span></a>            <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-255"><a href="#Pathier.write_text-255"><span class="linenos">255</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier.write_text-256"><a href="#Pathier.write_text-256"><span class="linenos">256</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier.write_text-257"><a href="#Pathier.write_text-257"><span class="linenos">257</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.write_text-258"><a href="#Pathier.write_text-258"><span class="linenos">258</span></a>                <span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_text-259"><a href="#Pathier.write_text-259"><span class="linenos">259</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.write_text-260"><a href="#Pathier.write_text-260"><span class="linenos">260</span></a>                <span class="k">raise</span>
+</span><span id="Pathier.write_text-261"><a href="#Pathier.write_text-261"><span class="linenos">261</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier.write_text-262"><a href="#Pathier.write_text-262"><span class="linenos">262</span></a>            <span class="k">raise</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Write data to file. If a TypeError is raised, the function
-will attempt to case data to a str and try the write again.
-If a FileNotFoundError is raised and parents = True,
-self.parent will be created.</p>
+            <div class="docstring"><p>Write data to file.</p>
+
+<p>If a <code>TypeError</code> is raised, the function  will attempt to cast <code>data</code> to a <code>str</code> and try the write again.</p>
+
+<p>If a <code>FileNotFoundError</code> is raised and <code>parents = True</code>, <code>self.parent</code> will be created.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.write_bytes" class="classattr">
                                         <input id="Pathier.write_bytes-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1107,42 +1283,215 @@
         <span class="def">def</span>
         <span class="name">write_bytes</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span>, </span><span class="param"><span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.write_bytes-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.write_bytes"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_bytes-236"><a href="#Pathier.write_bytes-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.write_bytes-237"><a href="#Pathier.write_bytes-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
-</span><span id="Pathier.write_bytes-238"><a href="#Pathier.write_bytes-238"><span class="linenos">238</span></a>
-</span><span id="Pathier.write_bytes-239"><a href="#Pathier.write_bytes-239"><span class="linenos">239</span></a><span class="sd">        :param parents: If True and the write operation fails</span>
-</span><span id="Pathier.write_bytes-240"><a href="#Pathier.write_bytes-240"><span class="linenos">240</span></a><span class="sd">        with a FileNotFoundError, make the parent directory</span>
-</span><span id="Pathier.write_bytes-241"><a href="#Pathier.write_bytes-241"><span class="linenos">241</span></a><span class="sd">        and retry the write.&quot;&quot;&quot;</span>
-</span><span id="Pathier.write_bytes-242"><a href="#Pathier.write_bytes-242"><span class="linenos">242</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-243"><a href="#Pathier.write_bytes-243"><span class="linenos">243</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-244"><a href="#Pathier.write_bytes-244"><span class="linenos">244</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-245"><a href="#Pathier.write_bytes-245"><span class="linenos">245</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-246"><a href="#Pathier.write_bytes-246"><span class="linenos">246</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-247"><a href="#Pathier.write_bytes-247"><span class="linenos">247</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="Pathier.write_bytes-248"><a href="#Pathier.write_bytes-248"><span class="linenos">248</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-249"><a href="#Pathier.write_bytes-249"><span class="linenos">249</span></a>                <span class="k">raise</span>
-</span><span id="Pathier.write_bytes-250"><a href="#Pathier.write_bytes-250"><span class="linenos">250</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="Pathier.write_bytes-251"><a href="#Pathier.write_bytes-251"><span class="linenos">251</span></a>            <span class="k">raise</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.write_bytes-264"><a href="#Pathier.write_bytes-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">write_bytes</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">bytes</span><span class="p">,</span> <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.write_bytes-265"><a href="#Pathier.write_bytes-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Write bytes to file.</span>
+</span><span id="Pathier.write_bytes-266"><a href="#Pathier.write_bytes-266"><span class="linenos">266</span></a>
+</span><span id="Pathier.write_bytes-267"><a href="#Pathier.write_bytes-267"><span class="linenos">267</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.write_bytes-268"><a href="#Pathier.write_bytes-268"><span class="linenos">268</span></a>
+</span><span id="Pathier.write_bytes-269"><a href="#Pathier.write_bytes-269"><span class="linenos">269</span></a><span class="sd">        `parents`: If `True` and the write operation fails with a `FileNotFoundError`,</span>
+</span><span id="Pathier.write_bytes-270"><a href="#Pathier.write_bytes-270"><span class="linenos">270</span></a><span class="sd">        make the parent directory and retry the write.&quot;&quot;&quot;</span>
+</span><span id="Pathier.write_bytes-271"><a href="#Pathier.write_bytes-271"><span class="linenos">271</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-272"><a href="#Pathier.write_bytes-272"><span class="linenos">272</span></a>            <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-273"><a href="#Pathier.write_bytes-273"><span class="linenos">273</span></a>        <span class="k">except</span> <span class="ne">FileNotFoundError</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-274"><a href="#Pathier.write_bytes-274"><span class="linenos">274</span></a>            <span class="k">if</span> <span class="n">parents</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-275"><a href="#Pathier.write_bytes-275"><span class="linenos">275</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">mkdir</span><span class="p">(</span><span class="n">parents</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-276"><a href="#Pathier.write_bytes-276"><span class="linenos">276</span></a>                <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">write_bytes</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="Pathier.write_bytes-277"><a href="#Pathier.write_bytes-277"><span class="linenos">277</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-278"><a href="#Pathier.write_bytes-278"><span class="linenos">278</span></a>                <span class="k">raise</span>
+</span><span id="Pathier.write_bytes-279"><a href="#Pathier.write_bytes-279"><span class="linenos">279</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Pathier.write_bytes-280"><a href="#Pathier.write_bytes-280"><span class="linenos">280</span></a>            <span class="k">raise</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Write bytes to file.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><strong>parents</strong>:  If True and the write operation fails
-with a FileNotFoundError, make the parent directory
-and retry the write.</li>
-</ul>
+<p><code><a href="#Pathier.parents">parents</a></code>: If <code>True</code> and the write operation fails with a <code>FileNotFoundError</code>,
+make the parent directory and retry the write.</p>
+</div>
+
+
+                            </div>
+                            <div id="Pathier.append" class="classattr">
+                                        <input id="Pathier.append-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">append</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">str</span>,</span><span class="param">	<span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Pathier.append-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Pathier.append"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.append-282"><a href="#Pathier.append-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">append</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">new_line</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="Pathier.append-283"><a href="#Pathier.append-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Append `data` to the file pointed to by this `Pathier` object.</span>
+</span><span id="Pathier.append-284"><a href="#Pathier.append-284"><span class="linenos">284</span></a>
+</span><span id="Pathier.append-285"><a href="#Pathier.append-285"><span class="linenos">285</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.append-286"><a href="#Pathier.append-286"><span class="linenos">286</span></a>
+</span><span id="Pathier.append-287"><a href="#Pathier.append-287"><span class="linenos">287</span></a><span class="sd">        `new_line`: If `True`, add `\\n` to `data`.</span>
+</span><span id="Pathier.append-288"><a href="#Pathier.append-288"><span class="linenos">288</span></a>
+</span><span id="Pathier.append-289"><a href="#Pathier.append-289"><span class="linenos">289</span></a><span class="sd">        `encoding`: The file encoding to use.&quot;&quot;&quot;</span>
+</span><span id="Pathier.append-290"><a href="#Pathier.append-290"><span class="linenos">290</span></a>        <span class="k">if</span> <span class="n">new_line</span><span class="p">:</span>
+</span><span id="Pathier.append-291"><a href="#Pathier.append-291"><span class="linenos">291</span></a>            <span class="n">data</span> <span class="o">+=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="Pathier.append-292"><a href="#Pathier.append-292"><span class="linenos">292</span></a>        <span class="k">with</span> <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;a&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
+</span><span id="Pathier.append-293"><a href="#Pathier.append-293"><span class="linenos">293</span></a>            <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Append <code>data</code> to the file pointed to by this <code><a href="#Pathier">Pathier</a></code> object.</p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>new_line</code>: If <code>True</code>, add <code>\n</code> to <code>data</code>.</p>
+
+<p><code>encoding</code>: The file encoding to use.</p>
+</div>
+
+
+                            </div>
+                            <div id="Pathier.replace" class="classattr">
+                                        <input id="Pathier.replace-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">replace</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]]</span>,</span><span class="param">	<span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Pathier.replace-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Pathier.replace"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.replace-295"><a href="#Pathier.replace-295"><span class="linenos">295</span></a>    <span class="k">def</span> <span class="nf">replace</span><span class="p">(</span>
+</span><span id="Pathier.replace-296"><a href="#Pathier.replace-296"><span class="linenos">296</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.replace-297"><a href="#Pathier.replace-297"><span class="linenos">297</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
+</span><span id="Pathier.replace-298"><a href="#Pathier.replace-298"><span class="linenos">298</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
+</span><span id="Pathier.replace-299"><a href="#Pathier.replace-299"><span class="linenos">299</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.replace-300"><a href="#Pathier.replace-300"><span class="linenos">300</span></a>    <span class="p">):</span>
+</span><span id="Pathier.replace-301"><a href="#Pathier.replace-301"><span class="linenos">301</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
+</span><span id="Pathier.replace-302"><a href="#Pathier.replace-302"><span class="linenos">302</span></a>
+</span><span id="Pathier.replace-303"><a href="#Pathier.replace-303"><span class="linenos">303</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.replace-304"><a href="#Pathier.replace-304"><span class="linenos">304</span></a>
+</span><span id="Pathier.replace-305"><a href="#Pathier.replace-305"><span class="linenos">305</span></a><span class="sd">        `count`: Only replace this many occurences of each pair.</span>
+</span><span id="Pathier.replace-306"><a href="#Pathier.replace-306"><span class="linenos">306</span></a><span class="sd">        By default (`-1`), all occurences are replaced.</span>
+</span><span id="Pathier.replace-307"><a href="#Pathier.replace-307"><span class="linenos">307</span></a>
+</span><span id="Pathier.replace-308"><a href="#Pathier.replace-308"><span class="linenos">308</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier.replace-309"><a href="#Pathier.replace-309"><span class="linenos">309</span></a>
+</span><span id="Pathier.replace-310"><a href="#Pathier.replace-310"><span class="linenos">310</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier.replace-311"><a href="#Pathier.replace-311"><span class="linenos">311</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;somefile.txt&quot;)</span>
+</span><span id="Pathier.replace-312"><a href="#Pathier.replace-312"><span class="linenos">312</span></a><span class="sd">        &gt;&gt;&gt;</span>
+</span><span id="Pathier.replace-313"><a href="#Pathier.replace-313"><span class="linenos">313</span></a><span class="sd">        &gt;&gt;&gt; path.replace([(&quot;hello&quot;, &quot;yeet&quot;), (&quot;goodbye&quot;, &quot;yeehaw&quot;)])</span>
+</span><span id="Pathier.replace-314"><a href="#Pathier.replace-314"><span class="linenos">314</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier.replace-315"><a href="#Pathier.replace-315"><span class="linenos">315</span></a><span class="sd">        &gt;&gt;&gt; path.write_text(path.read_text().replace(&quot;hello&quot;, &quot;yeet&quot;).replace(&quot;goodbye&quot;, &quot;yeehaw&quot;))&quot;&quot;&quot;</span>
+</span><span id="Pathier.replace-316"><a href="#Pathier.replace-316"><span class="linenos">316</span></a>        <span class="n">text</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">)</span>
+</span><span id="Pathier.replace-317"><a href="#Pathier.replace-317"><span class="linenos">317</span></a>        <span class="k">for</span> <span class="n">sub</span> <span class="ow">in</span> <span class="n">substitutions</span><span class="p">:</span>
+</span><span id="Pathier.replace-318"><a href="#Pathier.replace-318"><span class="linenos">318</span></a>            <span class="n">text</span> <span class="o">=</span> <span class="n">text</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">sub</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">sub</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">count</span><span class="p">)</span>
+</span><span id="Pathier.replace-319"><a href="#Pathier.replace-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">text</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>For each pair in <code>substitutions</code>, replace the first string with the second string.</p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>count</code>: Only replace this many occurences of each pair.
+By default (<code>-1</code>), all occurences are replaced.</p>
+
+<p><code>encoding</code>: The file encoding to use.</p>
+
+<p>e.g.</p>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;somefile.txt&quot;</span><span class="p">)</span>
+<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">path</span><span class="o">.</span><span class="n">replace</span><span class="p">([(</span><span class="s2">&quot;hello&quot;</span><span class="p">,</span> <span class="s2">&quot;yeet&quot;</span><span class="p">),</span> <span class="p">(</span><span class="s2">&quot;goodbye&quot;</span><span class="p">,</span> <span class="s2">&quot;yeehaw&quot;</span><span class="p">)])</span>
+<span class="go">equivalent to</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;hello&quot;</span><span class="p">,</span> <span class="s2">&quot;yeet&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;goodbye&quot;</span><span class="p">,</span> <span class="s2">&quot;yeehaw&quot;</span><span class="p">))</span>
+</code></pre>
+</div>
+</div>
+
+
+                            </div>
+                            <div id="Pathier.join" class="classattr">
+                                        <input id="Pathier.join-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">join</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="Pathier.join-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Pathier.join"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.join-321"><a href="#Pathier.join-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
+</span><span id="Pathier.join-322"><a href="#Pathier.join-322"><span class="linenos">322</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
+</span><span id="Pathier.join-323"><a href="#Pathier.join-323"><span class="linenos">323</span></a>
+</span><span id="Pathier.join-324"><a href="#Pathier.join-324"><span class="linenos">324</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
+</span><span id="Pathier.join-325"><a href="#Pathier.join-325"><span class="linenos">325</span></a>
+</span><span id="Pathier.join-326"><a href="#Pathier.join-326"><span class="linenos">326</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.join-327"><a href="#Pathier.join-327"><span class="linenos">327</span></a>
+</span><span id="Pathier.join-328"><a href="#Pathier.join-328"><span class="linenos">328</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier.join-329"><a href="#Pathier.join-329"><span class="linenos">329</span></a>
+</span><span id="Pathier.join-330"><a href="#Pathier.join-330"><span class="linenos">330</span></a><span class="sd">        `sep`: The separator to use when joining `data`.&quot;&quot;&quot;</span>
+</span><span id="Pathier.join-331"><a href="#Pathier.join-331"><span class="linenos">331</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">sep</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">data</span><span class="p">),</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Write a list of strings, joined by <code>sep</code>, to the file pointed at by this instance.</p>
+
+<p>Equivalent to <code>Pathier("somefile.txt").write_text(sep.join(data), encoding=encoding)</code></p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>encoding</code>: The file encoding to use.</p>
+
+<p><code>sep</code>: The separator to use when joining <code>data</code>.</p>
+</div>
+
+
+                            </div>
+                            <div id="Pathier.split" class="classattr">
+                                        <input id="Pathier.split-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">split</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
+
+                <label class="view-source-button" for="Pathier.split-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Pathier.split"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.split-333"><a href="#Pathier.split-333"><span class="linenos">333</span></a>    <span class="k">def</span> <span class="nf">split</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">keepends</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="Pathier.split-334"><a href="#Pathier.split-334"><span class="linenos">334</span></a>        <span class="sd">&quot;&quot;&quot;Returns the content of the pointed at file as a list of strings, splitting at new line characters.</span>
+</span><span id="Pathier.split-335"><a href="#Pathier.split-335"><span class="linenos">335</span></a>
+</span><span id="Pathier.split-336"><a href="#Pathier.split-336"><span class="linenos">336</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).read_text(encoding=encoding).splitlines()`</span>
+</span><span id="Pathier.split-337"><a href="#Pathier.split-337"><span class="linenos">337</span></a>
+</span><span id="Pathier.split-338"><a href="#Pathier.split-338"><span class="linenos">338</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.split-339"><a href="#Pathier.split-339"><span class="linenos">339</span></a>
+</span><span id="Pathier.split-340"><a href="#Pathier.split-340"><span class="linenos">340</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
+</span><span id="Pathier.split-341"><a href="#Pathier.split-341"><span class="linenos">341</span></a>
+</span><span id="Pathier.split-342"><a href="#Pathier.split-342"><span class="linenos">342</span></a><span class="sd">        `keepend`: If `True`, line breaks will be included in returned strings.&quot;&quot;&quot;</span>
+</span><span id="Pathier.split-343"><a href="#Pathier.split-343"><span class="linenos">343</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span><span class="o">.</span><span class="n">splitlines</span><span class="p">(</span><span class="n">keepends</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Returns the content of the pointed at file as a list of strings, splitting at new line characters.</p>
+
+<p>Equivalent to <code>Pathier("somefile.txt").read_text(encoding=encoding).splitlines()</code></p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>encoding</code>: The file encoding to use.</p>
+
+<p><code>keepend</code>: If <code>True</code>, line breaks will be included in returned strings.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.json_loads" class="classattr">
                                         <input id="Pathier.json_loads-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1150,17 +1499,17 @@
         <span class="def">def</span>
         <span class="name">json_loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.json_loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.json_loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_loads-253"><a href="#Pathier.json_loads-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.json_loads-254"><a href="#Pathier.json_loads-254"><span class="linenos">254</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.json_loads-255"><a href="#Pathier.json_loads-255"><span class="linenos">255</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_loads-345"><a href="#Pathier.json_loads-345"><span class="linenos">345</span></a>    <span class="k">def</span> <span class="nf">json_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.json_loads-346"><a href="#Pathier.json_loads-346"><span class="linenos">346</span></a>        <span class="sd">&quot;&quot;&quot;Load json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.json_loads-347"><a href="#Pathier.json_loads-347"><span class="linenos">347</span></a>        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load json file.</p>
 </div>
 
 
@@ -1172,37 +1521,37 @@
         <span class="def">def</span>
         <span class="name">json_dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">indent</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">default</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.json_dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.json_dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_dumps-257"><a href="#Pathier.json_dumps-257"><span class="linenos">257</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier.json_dumps-258"><a href="#Pathier.json_dumps-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-259"><a href="#Pathier.json_dumps-259"><span class="linenos">259</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-260"><a href="#Pathier.json_dumps-260"><span class="linenos">260</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-261"><a href="#Pathier.json_dumps-261"><span class="linenos">261</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-262"><a href="#Pathier.json_dumps-262"><span class="linenos">262</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-263"><a href="#Pathier.json_dumps-263"><span class="linenos">263</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-264"><a href="#Pathier.json_dumps-264"><span class="linenos">264</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-265"><a href="#Pathier.json_dumps-265"><span class="linenos">265</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-266"><a href="#Pathier.json_dumps-266"><span class="linenos">266</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-267"><a href="#Pathier.json_dumps-267"><span class="linenos">267</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.json_dumps-268"><a href="#Pathier.json_dumps-268"><span class="linenos">268</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to json file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.json_dumps-269"><a href="#Pathier.json_dumps-269"><span class="linenos">269</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier.json_dumps-270"><a href="#Pathier.json_dumps-270"><span class="linenos">270</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
-</span><span id="Pathier.json_dumps-271"><a href="#Pathier.json_dumps-271"><span class="linenos">271</span></a>            <span class="n">encoding</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-272"><a href="#Pathier.json_dumps-272"><span class="linenos">272</span></a>            <span class="n">errors</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-273"><a href="#Pathier.json_dumps-273"><span class="linenos">273</span></a>            <span class="n">newline</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-274"><a href="#Pathier.json_dumps-274"><span class="linenos">274</span></a>            <span class="n">parents</span><span class="p">,</span>
-</span><span id="Pathier.json_dumps-275"><a href="#Pathier.json_dumps-275"><span class="linenos">275</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.json_dumps-349"><a href="#Pathier.json_dumps-349"><span class="linenos">349</span></a>    <span class="k">def</span> <span class="nf">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier.json_dumps-350"><a href="#Pathier.json_dumps-350"><span class="linenos">350</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-351"><a href="#Pathier.json_dumps-351"><span class="linenos">351</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-352"><a href="#Pathier.json_dumps-352"><span class="linenos">352</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-353"><a href="#Pathier.json_dumps-353"><span class="linenos">353</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-354"><a href="#Pathier.json_dumps-354"><span class="linenos">354</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-355"><a href="#Pathier.json_dumps-355"><span class="linenos">355</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-356"><a href="#Pathier.json_dumps-356"><span class="linenos">356</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-357"><a href="#Pathier.json_dumps-357"><span class="linenos">357</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-358"><a href="#Pathier.json_dumps-358"><span class="linenos">358</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-359"><a href="#Pathier.json_dumps-359"><span class="linenos">359</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.json_dumps-360"><a href="#Pathier.json_dumps-360"><span class="linenos">360</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to json file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.json_dumps-361"><a href="#Pathier.json_dumps-361"><span class="linenos">361</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier.json_dumps-362"><a href="#Pathier.json_dumps-362"><span class="linenos">362</span></a>            <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">indent</span><span class="o">=</span><span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="n">default</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="n">sort_keys</span><span class="p">),</span>
+</span><span id="Pathier.json_dumps-363"><a href="#Pathier.json_dumps-363"><span class="linenos">363</span></a>            <span class="n">encoding</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-364"><a href="#Pathier.json_dumps-364"><span class="linenos">364</span></a>            <span class="n">errors</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-365"><a href="#Pathier.json_dumps-365"><span class="linenos">365</span></a>            <span class="n">newline</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-366"><a href="#Pathier.json_dumps-366"><span class="linenos">366</span></a>            <span class="n">parents</span><span class="p">,</span>
+</span><span id="Pathier.json_dumps-367"><a href="#Pathier.json_dumps-367"><span class="linenos">367</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Dump data to json file.</p>
+            <div class="docstring"><p>Dump <code>data</code> to json file.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.toml_loads" class="classattr">
                                         <input id="Pathier.toml_loads-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1210,17 +1559,17 @@
         <span class="def">def</span>
         <span class="name">toml_loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.toml_loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.toml_loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_loads-277"><a href="#Pathier.toml_loads-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.toml_loads-278"><a href="#Pathier.toml_loads-278"><span class="linenos">278</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.toml_loads-279"><a href="#Pathier.toml_loads-279"><span class="linenos">279</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_loads-369"><a href="#Pathier.toml_loads-369"><span class="linenos">369</span></a>    <span class="k">def</span> <span class="nf">toml_loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.toml_loads-370"><a href="#Pathier.toml_loads-370"><span class="linenos">370</span></a>        <span class="sd">&quot;&quot;&quot;Load toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.toml_loads-371"><a href="#Pathier.toml_loads-371"><span class="linenos">371</span></a>        <span class="k">return</span> <span class="n">tomlkit</span><span class="o">.</span><span class="n">loads</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">))</span><span class="o">.</span><span class="n">unwrap</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load toml file.</p>
 </div>
 
 
@@ -1232,31 +1581,31 @@
         <span class="def">def</span>
         <span class="name">toml_dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.toml_dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.toml_dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_dumps-281"><a href="#Pathier.toml_dumps-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
-</span><span id="Pathier.toml_dumps-282"><a href="#Pathier.toml_dumps-282"><span class="linenos">282</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-283"><a href="#Pathier.toml_dumps-283"><span class="linenos">283</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-284"><a href="#Pathier.toml_dumps-284"><span class="linenos">284</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-285"><a href="#Pathier.toml_dumps-285"><span class="linenos">285</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-286"><a href="#Pathier.toml_dumps-286"><span class="linenos">286</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-287"><a href="#Pathier.toml_dumps-287"><span class="linenos">287</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-288"><a href="#Pathier.toml_dumps-288"><span class="linenos">288</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.toml_dumps-289"><a href="#Pathier.toml_dumps-289"><span class="linenos">289</span></a>    <span class="p">):</span>
-</span><span id="Pathier.toml_dumps-290"><a href="#Pathier.toml_dumps-290"><span class="linenos">290</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to toml file.&quot;&quot;&quot;</span>
-</span><span id="Pathier.toml_dumps-291"><a href="#Pathier.toml_dumps-291"><span class="linenos">291</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="Pathier.toml_dumps-292"><a href="#Pathier.toml_dumps-292"><span class="linenos">292</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier.toml_dumps-293"><a href="#Pathier.toml_dumps-293"><span class="linenos">293</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.toml_dumps-373"><a href="#Pathier.toml_dumps-373"><span class="linenos">373</span></a>    <span class="k">def</span> <span class="nf">toml_dumps</span><span class="p">(</span>
+</span><span id="Pathier.toml_dumps-374"><a href="#Pathier.toml_dumps-374"><span class="linenos">374</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-375"><a href="#Pathier.toml_dumps-375"><span class="linenos">375</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-376"><a href="#Pathier.toml_dumps-376"><span class="linenos">376</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-377"><a href="#Pathier.toml_dumps-377"><span class="linenos">377</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-378"><a href="#Pathier.toml_dumps-378"><span class="linenos">378</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-379"><a href="#Pathier.toml_dumps-379"><span class="linenos">379</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-380"><a href="#Pathier.toml_dumps-380"><span class="linenos">380</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.toml_dumps-381"><a href="#Pathier.toml_dumps-381"><span class="linenos">381</span></a>    <span class="p">):</span>
+</span><span id="Pathier.toml_dumps-382"><a href="#Pathier.toml_dumps-382"><span class="linenos">382</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to toml file.&quot;&quot;&quot;</span>
+</span><span id="Pathier.toml_dumps-383"><a href="#Pathier.toml_dumps-383"><span class="linenos">383</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="Pathier.toml_dumps-384"><a href="#Pathier.toml_dumps-384"><span class="linenos">384</span></a>            <span class="n">tomlkit</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">),</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier.toml_dumps-385"><a href="#Pathier.toml_dumps-385"><span class="linenos">385</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Dump data to toml file.</p>
+            <div class="docstring"><p>Dump <code>data</code> to toml file.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.loads" class="classattr">
                                         <input id="Pathier.loads-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1264,21 +1613,21 @@
         <span class="def">def</span>
         <span class="name">loads</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.loads-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.loads"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.loads-295"><a href="#Pathier.loads-295"><span class="linenos">295</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="Pathier.loads-296"><a href="#Pathier.loads-296"><span class="linenos">296</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier.loads-297"><a href="#Pathier.loads-297"><span class="linenos">297</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier.loads-298"><a href="#Pathier.loads-298"><span class="linenos">298</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier.loads-299"><a href="#Pathier.loads-299"><span class="linenos">299</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
-</span><span id="Pathier.loads-300"><a href="#Pathier.loads-300"><span class="linenos">300</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier.loads-301"><a href="#Pathier.loads-301"><span class="linenos">301</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.loads-387"><a href="#Pathier.loads-387"><span class="linenos">387</span></a>    <span class="k">def</span> <span class="nf">loads</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="Pathier.loads-388"><a href="#Pathier.loads-388"><span class="linenos">388</span></a>        <span class="sd">&quot;&quot;&quot;Load a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier.loads-389"><a href="#Pathier.loads-389"><span class="linenos">389</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier.loads-390"><a href="#Pathier.loads-390"><span class="linenos">390</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier.loads-391"><a href="#Pathier.loads-391"><span class="linenos">391</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">json_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
+</span><span id="Pathier.loads-392"><a href="#Pathier.loads-392"><span class="linenos">392</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier.loads-393"><a href="#Pathier.loads-393"><span class="linenos">393</span></a>                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">toml_loads</span><span class="p">(</span><span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Load a json or toml file based off this instance's suffix.</p>
 </div>
 
 
@@ -1290,37 +1639,37 @@
         <span class="def">def</span>
         <span class="name">dumps</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Any</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">errors</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">newline</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>,</span><span class="param">	<span class="n">indent</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">default</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.dumps-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.dumps"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.dumps-303"><a href="#Pathier.dumps-303"><span class="linenos">303</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
-</span><span id="Pathier.dumps-304"><a href="#Pathier.dumps-304"><span class="linenos">304</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.dumps-305"><a href="#Pathier.dumps-305"><span class="linenos">305</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
-</span><span id="Pathier.dumps-306"><a href="#Pathier.dumps-306"><span class="linenos">306</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-307"><a href="#Pathier.dumps-307"><span class="linenos">307</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-308"><a href="#Pathier.dumps-308"><span class="linenos">308</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-309"><a href="#Pathier.dumps-309"><span class="linenos">309</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="Pathier.dumps-310"><a href="#Pathier.dumps-310"><span class="linenos">310</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-311"><a href="#Pathier.dumps-311"><span class="linenos">311</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="Pathier.dumps-312"><a href="#Pathier.dumps-312"><span class="linenos">312</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="Pathier.dumps-313"><a href="#Pathier.dumps-313"><span class="linenos">313</span></a>    <span class="p">):</span>
-</span><span id="Pathier.dumps-314"><a href="#Pathier.dumps-314"><span class="linenos">314</span></a>        <span class="sd">&quot;&quot;&quot;Dump data to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
-</span><span id="Pathier.dumps-315"><a href="#Pathier.dumps-315"><span class="linenos">315</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
-</span><span id="Pathier.dumps-316"><a href="#Pathier.dumps-316"><span class="linenos">316</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
-</span><span id="Pathier.dumps-317"><a href="#Pathier.dumps-317"><span class="linenos">317</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
-</span><span id="Pathier.dumps-318"><a href="#Pathier.dumps-318"><span class="linenos">318</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
-</span><span id="Pathier.dumps-319"><a href="#Pathier.dumps-319"><span class="linenos">319</span></a>                <span class="p">)</span>
-</span><span id="Pathier.dumps-320"><a href="#Pathier.dumps-320"><span class="linenos">320</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
-</span><span id="Pathier.dumps-321"><a href="#Pathier.dumps-321"><span class="linenos">321</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.dumps-395"><a href="#Pathier.dumps-395"><span class="linenos">395</span></a>    <span class="k">def</span> <span class="nf">dumps</span><span class="p">(</span>
+</span><span id="Pathier.dumps-396"><a href="#Pathier.dumps-396"><span class="linenos">396</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="Pathier.dumps-397"><a href="#Pathier.dumps-397"><span class="linenos">397</span></a>        <span class="n">data</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span>
+</span><span id="Pathier.dumps-398"><a href="#Pathier.dumps-398"><span class="linenos">398</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-399"><a href="#Pathier.dumps-399"><span class="linenos">399</span></a>        <span class="n">errors</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-400"><a href="#Pathier.dumps-400"><span class="linenos">400</span></a>        <span class="n">newline</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-401"><a href="#Pathier.dumps-401"><span class="linenos">401</span></a>        <span class="n">sort_keys</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="Pathier.dumps-402"><a href="#Pathier.dumps-402"><span class="linenos">402</span></a>        <span class="n">indent</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-403"><a href="#Pathier.dumps-403"><span class="linenos">403</span></a>        <span class="n">default</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="Pathier.dumps-404"><a href="#Pathier.dumps-404"><span class="linenos">404</span></a>        <span class="n">parents</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="Pathier.dumps-405"><a href="#Pathier.dumps-405"><span class="linenos">405</span></a>    <span class="p">):</span>
+</span><span id="Pathier.dumps-406"><a href="#Pathier.dumps-406"><span class="linenos">406</span></a>        <span class="sd">&quot;&quot;&quot;Dump `data` to a json or toml file based off this instance&#39;s suffix.&quot;&quot;&quot;</span>
+</span><span id="Pathier.dumps-407"><a href="#Pathier.dumps-407"><span class="linenos">407</span></a>        <span class="k">match</span> <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="p">:</span>
+</span><span id="Pathier.dumps-408"><a href="#Pathier.dumps-408"><span class="linenos">408</span></a>            <span class="k">case</span> <span class="s2">&quot;.json&quot;</span><span class="p">:</span>
+</span><span id="Pathier.dumps-409"><a href="#Pathier.dumps-409"><span class="linenos">409</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">json_dumps</span><span class="p">(</span>
+</span><span id="Pathier.dumps-410"><a href="#Pathier.dumps-410"><span class="linenos">410</span></a>                    <span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">indent</span><span class="p">,</span> <span class="n">default</span><span class="p">,</span> <span class="n">parents</span>
+</span><span id="Pathier.dumps-411"><a href="#Pathier.dumps-411"><span class="linenos">411</span></a>                <span class="p">)</span>
+</span><span id="Pathier.dumps-412"><a href="#Pathier.dumps-412"><span class="linenos">412</span></a>            <span class="k">case</span> <span class="s2">&quot;.toml&quot;</span><span class="p">:</span>
+</span><span id="Pathier.dumps-413"><a href="#Pathier.dumps-413"><span class="linenos">413</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">toml_dumps</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">encoding</span><span class="p">,</span> <span class="n">errors</span><span class="p">,</span> <span class="n">newline</span><span class="p">,</span> <span class="n">sort_keys</span><span class="p">,</span> <span class="n">parents</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Dump data to a json or toml file based off this instance's suffix.</p>
+            <div class="docstring"><p>Dump <code>data</code> to a json or toml file based off this instance's suffix.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.delete" class="classattr">
                                         <input id="Pathier.delete-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1328,26 +1677,28 @@
         <span class="def">def</span>
         <span class="name">delete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.delete-323"><a href="#Pathier.delete-323"><span class="linenos">323</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="Pathier.delete-324"><a href="#Pathier.delete-324"><span class="linenos">324</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
-</span><span id="Pathier.delete-325"><a href="#Pathier.delete-325"><span class="linenos">325</span></a><span class="sd">        Uses self.unlink() if a file and uses shutil.rmtree() if a directory.&quot;&quot;&quot;</span>
-</span><span id="Pathier.delete-326"><a href="#Pathier.delete-326"><span class="linenos">326</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.delete-327"><a href="#Pathier.delete-327"><span class="linenos">327</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
-</span><span id="Pathier.delete-328"><a href="#Pathier.delete-328"><span class="linenos">328</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.delete-329"><a href="#Pathier.delete-329"><span class="linenos">329</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.delete-415"><a href="#Pathier.delete-415"><span class="linenos">415</span></a>    <span class="k">def</span> <span class="nf">delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">missing_ok</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="Pathier.delete-416"><a href="#Pathier.delete-416"><span class="linenos">416</span></a>        <span class="sd">&quot;&quot;&quot;Delete the file or folder pointed to by this instance.</span>
+</span><span id="Pathier.delete-417"><a href="#Pathier.delete-417"><span class="linenos">417</span></a>
+</span><span id="Pathier.delete-418"><a href="#Pathier.delete-418"><span class="linenos">418</span></a><span class="sd">        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a directory.&quot;&quot;&quot;</span>
+</span><span id="Pathier.delete-419"><a href="#Pathier.delete-419"><span class="linenos">419</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier.delete-420"><a href="#Pathier.delete-420"><span class="linenos">420</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">unlink</span><span class="p">(</span><span class="n">missing_ok</span><span class="p">)</span>
+</span><span id="Pathier.delete-421"><a href="#Pathier.delete-421"><span class="linenos">421</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier.delete-422"><a href="#Pathier.delete-422"><span class="linenos">422</span></a>            <span class="n">shutil</span><span class="o">.</span><span class="n">rmtree</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Delete the file or folder pointed to by this instance.
-Uses self.unlink() if a file and uses shutil.rmtree() if a directory.</p>
+            <div class="docstring"><p>Delete the file or folder pointed to by this instance.</p>
+
+<p>Uses <code>self.unlink()</code> if a file and uses <code>shutil.rmtree()</code> if a directory.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.copy" class="classattr">
                                         <input id="Pathier.copy-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1355,55 +1706,58 @@
         <span class="def">def</span>
         <span class="name">copy</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">new_path</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="n">Self</span><span class="p">,</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">,</span> <span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Self</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.copy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.copy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.copy-331"><a href="#Pathier.copy-331"><span class="linenos">331</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
-</span><span id="Pathier.copy-332"><a href="#Pathier.copy-332"><span class="linenos">332</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="Pathier.copy-333"><a href="#Pathier.copy-333"><span class="linenos">333</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
-</span><span id="Pathier.copy-334"><a href="#Pathier.copy-334"><span class="linenos">334</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
-</span><span id="Pathier.copy-335"><a href="#Pathier.copy-335"><span class="linenos">335</span></a><span class="sd">        to the instance pointed to by new_path using shutil.copyfile</span>
-</span><span id="Pathier.copy-336"><a href="#Pathier.copy-336"><span class="linenos">336</span></a><span class="sd">        or shutil.copytree. Returns the new path.</span>
-</span><span id="Pathier.copy-337"><a href="#Pathier.copy-337"><span class="linenos">337</span></a>
-</span><span id="Pathier.copy-338"><a href="#Pathier.copy-338"><span class="linenos">338</span></a><span class="sd">        :param new_path: The copy destination.</span>
-</span><span id="Pathier.copy-339"><a href="#Pathier.copy-339"><span class="linenos">339</span></a>
-</span><span id="Pathier.copy-340"><a href="#Pathier.copy-340"><span class="linenos">340</span></a><span class="sd">        :param overwrite: If True, files already existing in new_path</span>
-</span><span id="Pathier.copy-341"><a href="#Pathier.copy-341"><span class="linenos">341</span></a><span class="sd">        will be overwritten. If False, only files that don&#39;t exist in new_path</span>
-</span><span id="Pathier.copy-342"><a href="#Pathier.copy-342"><span class="linenos">342</span></a><span class="sd">        will be copied.&quot;&quot;&quot;</span>
-</span><span id="Pathier.copy-343"><a href="#Pathier.copy-343"><span class="linenos">343</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier.copy-344"><a href="#Pathier.copy-344"><span class="linenos">344</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
-</span><span id="Pathier.copy-345"><a href="#Pathier.copy-345"><span class="linenos">345</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-346"><a href="#Pathier.copy-346"><span class="linenos">346</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.copy-347"><a href="#Pathier.copy-347"><span class="linenos">347</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="Pathier.copy-348"><a href="#Pathier.copy-348"><span class="linenos">348</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
-</span><span id="Pathier.copy-349"><a href="#Pathier.copy-349"><span class="linenos">349</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="Pathier.copy-350"><a href="#Pathier.copy-350"><span class="linenos">350</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
-</span><span id="Pathier.copy-351"><a href="#Pathier.copy-351"><span class="linenos">351</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-352"><a href="#Pathier.copy-352"><span class="linenos">352</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
-</span><span id="Pathier.copy-353"><a href="#Pathier.copy-353"><span class="linenos">353</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="Pathier.copy-354"><a href="#Pathier.copy-354"><span class="linenos">354</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.copy-355"><a href="#Pathier.copy-355"><span class="linenos">355</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
-</span><span id="Pathier.copy-356"><a href="#Pathier.copy-356"><span class="linenos">356</span></a>        <span class="k">return</span> <span class="n">new_path</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.copy-424"><a href="#Pathier.copy-424"><span class="linenos">424</span></a>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span>
+</span><span id="Pathier.copy-425"><a href="#Pathier.copy-425"><span class="linenos">425</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">:</span> <span class="n">Self</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span><span class="p">,</span> <span class="n">overwrite</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="Pathier.copy-426"><a href="#Pathier.copy-426"><span class="linenos">426</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span><span class="p">:</span>
+</span><span id="Pathier.copy-427"><a href="#Pathier.copy-427"><span class="linenos">427</span></a>        <span class="sd">&quot;&quot;&quot;Copy the path pointed to by this instance</span>
+</span><span id="Pathier.copy-428"><a href="#Pathier.copy-428"><span class="linenos">428</span></a><span class="sd">        to the instance pointed to by `new_path` using `shutil.copyfile`</span>
+</span><span id="Pathier.copy-429"><a href="#Pathier.copy-429"><span class="linenos">429</span></a><span class="sd">        or `shutil.copytree`.</span>
+</span><span id="Pathier.copy-430"><a href="#Pathier.copy-430"><span class="linenos">430</span></a>
+</span><span id="Pathier.copy-431"><a href="#Pathier.copy-431"><span class="linenos">431</span></a><span class="sd">        Returns the new path.</span>
+</span><span id="Pathier.copy-432"><a href="#Pathier.copy-432"><span class="linenos">432</span></a>
+</span><span id="Pathier.copy-433"><a href="#Pathier.copy-433"><span class="linenos">433</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.copy-434"><a href="#Pathier.copy-434"><span class="linenos">434</span></a>
+</span><span id="Pathier.copy-435"><a href="#Pathier.copy-435"><span class="linenos">435</span></a><span class="sd">        `new_path`: The copy destination.</span>
+</span><span id="Pathier.copy-436"><a href="#Pathier.copy-436"><span class="linenos">436</span></a>
+</span><span id="Pathier.copy-437"><a href="#Pathier.copy-437"><span class="linenos">437</span></a><span class="sd">        `overwrite`: If `True`, files already existing in `new_path` will be overwritten.</span>
+</span><span id="Pathier.copy-438"><a href="#Pathier.copy-438"><span class="linenos">438</span></a><span class="sd">        If `False`, only files that don&#39;t exist in `new_path` will be copied.&quot;&quot;&quot;</span>
+</span><span id="Pathier.copy-439"><a href="#Pathier.copy-439"><span class="linenos">439</span></a>        <span class="n">new_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier.copy-440"><a href="#Pathier.copy-440"><span class="linenos">440</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_dir</span><span class="p">():</span>
+</span><span id="Pathier.copy-441"><a href="#Pathier.copy-441"><span class="linenos">441</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-442"><a href="#Pathier.copy-442"><span class="linenos">442</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copytree</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">,</span> <span class="n">dirs_exist_ok</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.copy-443"><a href="#Pathier.copy-443"><span class="linenos">443</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="Pathier.copy-444"><a href="#Pathier.copy-444"><span class="linenos">444</span></a>                <span class="n">files</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">)</span>
+</span><span id="Pathier.copy-445"><a href="#Pathier.copy-445"><span class="linenos">445</span></a>                <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="Pathier.copy-446"><a href="#Pathier.copy-446"><span class="linenos">446</span></a>                    <span class="n">dst</span> <span class="o">=</span> <span class="n">new_path</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="p">)</span>
+</span><span id="Pathier.copy-447"><a href="#Pathier.copy-447"><span class="linenos">447</span></a>                    <span class="k">if</span> <span class="ow">not</span> <span class="n">dst</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-448"><a href="#Pathier.copy-448"><span class="linenos">448</span></a>                        <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="n">file</span><span class="p">,</span> <span class="n">dst</span><span class="p">)</span>
+</span><span id="Pathier.copy-449"><a href="#Pathier.copy-449"><span class="linenos">449</span></a>        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="Pathier.copy-450"><a href="#Pathier.copy-450"><span class="linenos">450</span></a>            <span class="k">if</span> <span class="n">overwrite</span> <span class="ow">or</span> <span class="ow">not</span> <span class="n">new_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.copy-451"><a href="#Pathier.copy-451"><span class="linenos">451</span></a>                <span class="n">shutil</span><span class="o">.</span><span class="n">copyfile</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_path</span><span class="p">)</span>
+</span><span id="Pathier.copy-452"><a href="#Pathier.copy-452"><span class="linenos">452</span></a>        <span class="k">return</span> <span class="n">new_path</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Copy the path pointed to by this instance
-to the instance pointed to by new_path using shutil.copyfile
-or shutil.copytree. Returns the new path.</p>
+to the instance pointed to by <code>new_path</code> using <code>shutil.copyfile</code>
+or <code>shutil.copytree</code>.</p>
+
+<p>Returns the new path.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><p><strong>new_path</strong>:  The copy destination.</p></li>
-<li><p><strong>overwrite</strong>:  If True, files already existing in new_path
-will be overwritten. If False, only files that don't exist in new_path
-will be copied.</p></li>
-</ul>
+<p><code>new_path</code>: The copy destination.</p>
+
+<p><code>overwrite</code>: If <code>True</code>, files already existing in <code>new_path</code> will be overwritten.
+If <code>False</code>, only files that don't exist in <code>new_path</code> will be copied.</p>
 </div>
 
 
                             </div>
                             <div id="Pathier.backup" class="classattr">
                                         <input id="Pathier.backup-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1411,48 +1765,48 @@
         <span class="def">def</span>
         <span class="name">backup</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="n">Optional</span><span class="p">[</span><span class="n">Self</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="Pathier.backup-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.backup"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.backup-358"><a href="#Pathier.backup-358"><span class="linenos">358</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="Pathier.backup-359"><a href="#Pathier.backup-359"><span class="linenos">359</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
-</span><span id="Pathier.backup-360"><a href="#Pathier.backup-360"><span class="linenos">360</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
-</span><span id="Pathier.backup-361"><a href="#Pathier.backup-361"><span class="linenos">361</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
-</span><span id="Pathier.backup-362"><a href="#Pathier.backup-362"><span class="linenos">362</span></a>
-</span><span id="Pathier.backup-363"><a href="#Pathier.backup-363"><span class="linenos">363</span></a><span class="sd">        :param `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
-</span><span id="Pathier.backup-364"><a href="#Pathier.backup-364"><span class="linenos">364</span></a>
-</span><span id="Pathier.backup-365"><a href="#Pathier.backup-365"><span class="linenos">365</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
-</span><span id="Pathier.backup-366"><a href="#Pathier.backup-366"><span class="linenos">366</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
-</span><span id="Pathier.backup-367"><a href="#Pathier.backup-367"><span class="linenos">367</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier.backup-368"><a href="#Pathier.backup-368"><span class="linenos">368</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
-</span><span id="Pathier.backup-369"><a href="#Pathier.backup-369"><span class="linenos">369</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
-</span><span id="Pathier.backup-370"><a href="#Pathier.backup-370"><span class="linenos">370</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
-</span><span id="Pathier.backup-371"><a href="#Pathier.backup-371"><span class="linenos">371</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
-</span><span id="Pathier.backup-372"><a href="#Pathier.backup-372"><span class="linenos">372</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="Pathier.backup-373"><a href="#Pathier.backup-373"><span class="linenos">373</span></a>            <span class="k">return</span> <span class="kc">None</span>
-</span><span id="Pathier.backup-374"><a href="#Pathier.backup-374"><span class="linenos">374</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
-</span><span id="Pathier.backup-375"><a href="#Pathier.backup-375"><span class="linenos">375</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
-</span><span id="Pathier.backup-376"><a href="#Pathier.backup-376"><span class="linenos">376</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="Pathier.backup-377"><a href="#Pathier.backup-377"><span class="linenos">377</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
-</span><span id="Pathier.backup-378"><a href="#Pathier.backup-378"><span class="linenos">378</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
-</span><span id="Pathier.backup-379"><a href="#Pathier.backup-379"><span class="linenos">379</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.backup-454"><a href="#Pathier.backup-454"><span class="linenos">454</span></a>    <span class="k">def</span> <span class="nf">backup</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">timestamp</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Self</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="Pathier.backup-455"><a href="#Pathier.backup-455"><span class="linenos">455</span></a>        <span class="sd">&quot;&quot;&quot;Create a copy of this file or directory with `_backup` appended to the path stem.</span>
+</span><span id="Pathier.backup-456"><a href="#Pathier.backup-456"><span class="linenos">456</span></a><span class="sd">        If the path to be backed up doesn&#39;t exist, `None` is returned.</span>
+</span><span id="Pathier.backup-457"><a href="#Pathier.backup-457"><span class="linenos">457</span></a><span class="sd">        Otherwise a `Pathier` object for the backup is returned.</span>
+</span><span id="Pathier.backup-458"><a href="#Pathier.backup-458"><span class="linenos">458</span></a>
+</span><span id="Pathier.backup-459"><a href="#Pathier.backup-459"><span class="linenos">459</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.backup-460"><a href="#Pathier.backup-460"><span class="linenos">460</span></a>
+</span><span id="Pathier.backup-461"><a href="#Pathier.backup-461"><span class="linenos">461</span></a><span class="sd">        `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.</span>
+</span><span id="Pathier.backup-462"><a href="#Pathier.backup-462"><span class="linenos">462</span></a>
+</span><span id="Pathier.backup-463"><a href="#Pathier.backup-463"><span class="linenos">463</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;some_file.txt&quot;)</span>
+</span><span id="Pathier.backup-464"><a href="#Pathier.backup-464"><span class="linenos">464</span></a><span class="sd">        &gt;&gt;&gt; path.backup()</span>
+</span><span id="Pathier.backup-465"><a href="#Pathier.backup-465"><span class="linenos">465</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier.backup-466"><a href="#Pathier.backup-466"><span class="linenos">466</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;]</span>
+</span><span id="Pathier.backup-467"><a href="#Pathier.backup-467"><span class="linenos">467</span></a><span class="sd">        &gt;&gt;&gt; path.backup(True)</span>
+</span><span id="Pathier.backup-468"><a href="#Pathier.backup-468"><span class="linenos">468</span></a><span class="sd">        &gt;&gt;&gt; list(path.iterdir())</span>
+</span><span id="Pathier.backup-469"><a href="#Pathier.backup-469"><span class="linenos">469</span></a><span class="sd">        &gt;&gt;&gt; [&#39;some_file.txt&#39;, &#39;some_file_backup.txt&#39;, &#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;]&quot;&quot;&quot;</span>
+</span><span id="Pathier.backup-470"><a href="#Pathier.backup-470"><span class="linenos">470</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="Pathier.backup-471"><a href="#Pathier.backup-471"><span class="linenos">471</span></a>            <span class="k">return</span> <span class="kc">None</span>
+</span><span id="Pathier.backup-472"><a href="#Pathier.backup-472"><span class="linenos">472</span></a>        <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_backup&quot;</span>
+</span><span id="Pathier.backup-473"><a href="#Pathier.backup-473"><span class="linenos">473</span></a>        <span class="k">if</span> <span class="n">timestamp</span><span class="p">:</span>
+</span><span id="Pathier.backup-474"><a href="#Pathier.backup-474"><span class="linenos">474</span></a>            <span class="n">backup_stem</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">backup_stem</span><span class="si">}</span><span class="s2">_</span><span class="si">{</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span><span class="o">.</span><span class="n">strftime</span><span class="p">(</span><span class="s1">&#39;%m-</span><span class="si">%d</span><span class="s1">-%Y-%I_%M_%S_%p&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="Pathier.backup-475"><a href="#Pathier.backup-475"><span class="linenos">475</span></a>        <span class="n">backup_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">backup_stem</span><span class="p">)</span>
+</span><span id="Pathier.backup-476"><a href="#Pathier.backup-476"><span class="linenos">476</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">(</span><span class="n">backup_path</span><span class="p">,</span> <span class="kc">True</span><span class="p">)</span>
+</span><span id="Pathier.backup-477"><a href="#Pathier.backup-477"><span class="linenos">477</span></a>        <span class="k">return</span> <span class="n">backup_path</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a copy of this file or directory with <code>_backup</code> appended to the path stem.
 If the path to be backed up doesn't exist, <code>None</code> is returned.
 Otherwise a <code><a href="#Pathier">Pathier</a></code> object for the backup is returned.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
 
-<ul>
-<li><strong><code>timestamp</code></strong>:  Add a timestamp to the backup name to prevent overriding previous backups.</li>
-</ul>
+<p><code>timestamp</code>: Add a timestamp to the backup name to prevent overriding previous backups.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;some_file.txt&quot;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">path</span><span class="o">.</span><span class="n">backup</span><span class="p">()</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">iterdir</span><span class="p">())</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="p">[</span><span class="s1">&#39;some_file.txt&#39;</span><span class="p">,</span> <span class="s1">&#39;some_file_backup.txt&#39;</span><span class="p">]</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">path</span><span class="o">.</span><span class="n">backup</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span>
@@ -1460,14 +1814,70 @@
 <span class="gp">&gt;&gt;&gt; </span><span class="p">[</span><span class="s1">&#39;some_file.txt&#39;</span><span class="p">,</span> <span class="s1">&#39;some_file_backup.txt&#39;</span><span class="p">,</span> <span class="s1">&#39;some_file_backup_04-28-2023-06_25_52_PM.txt&#39;</span><span class="p">]</span>
 </code></pre>
 </div>
 </div>
 
 
                             </div>
+                            <div id="Pathier.execute" class="classattr">
+                                        <input id="Pathier.execute-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">execute</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
+
+                <label class="view-source-button" for="Pathier.execute-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#Pathier.execute"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.execute-479"><a href="#Pathier.execute-479"><span class="linenos">479</span></a>    <span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Pathier.execute-480"><a href="#Pathier.execute-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Make a call to `os.system` using the path pointed to by this Pathier object.</span>
+</span><span id="Pathier.execute-481"><a href="#Pathier.execute-481"><span class="linenos">481</span></a>
+</span><span id="Pathier.execute-482"><a href="#Pathier.execute-482"><span class="linenos">482</span></a><span class="sd">        #### :params:</span>
+</span><span id="Pathier.execute-483"><a href="#Pathier.execute-483"><span class="linenos">483</span></a>
+</span><span id="Pathier.execute-484"><a href="#Pathier.execute-484"><span class="linenos">484</span></a><span class="sd">        `command`: Program/command to precede the path with.</span>
+</span><span id="Pathier.execute-485"><a href="#Pathier.execute-485"><span class="linenos">485</span></a>
+</span><span id="Pathier.execute-486"><a href="#Pathier.execute-486"><span class="linenos">486</span></a><span class="sd">        `args`: Any arguments that should come after the path.</span>
+</span><span id="Pathier.execute-487"><a href="#Pathier.execute-487"><span class="linenos">487</span></a>
+</span><span id="Pathier.execute-488"><a href="#Pathier.execute-488"><span class="linenos">488</span></a><span class="sd">        :returns: The integer output of `os.system`.</span>
+</span><span id="Pathier.execute-489"><a href="#Pathier.execute-489"><span class="linenos">489</span></a>
+</span><span id="Pathier.execute-490"><a href="#Pathier.execute-490"><span class="linenos">490</span></a><span class="sd">        e.g.</span>
+</span><span id="Pathier.execute-491"><a href="#Pathier.execute-491"><span class="linenos">491</span></a><span class="sd">        &gt;&gt;&gt; path = Pathier(&quot;mydirectory&quot;) / &quot;myscript.py&quot;</span>
+</span><span id="Pathier.execute-492"><a href="#Pathier.execute-492"><span class="linenos">492</span></a><span class="sd">        then</span>
+</span><span id="Pathier.execute-493"><a href="#Pathier.execute-493"><span class="linenos">493</span></a><span class="sd">        &gt;&gt;&gt; path.execute(&quot;py&quot;, &quot;--iterations 10&quot;)</span>
+</span><span id="Pathier.execute-494"><a href="#Pathier.execute-494"><span class="linenos">494</span></a><span class="sd">        equivalent to</span>
+</span><span id="Pathier.execute-495"><a href="#Pathier.execute-495"><span class="linenos">495</span></a><span class="sd">        &gt;&gt;&gt; os.system(f&quot;py {path} --iterations 10&quot;)&quot;&quot;&quot;</span>
+</span><span id="Pathier.execute-496"><a href="#Pathier.execute-496"><span class="linenos">496</span></a>        <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="bp">self</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Make a call to <code>os.system</code> using the path pointed to by this Pathier object.</p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>command</code>: Program/command to precede the path with.</p>
+
+<p><code>args</code>: Any arguments that should come after the path.</p>
+
+<p>:returns: The integer output of <code>os.system</code>.</p>
+
+<p>e.g.</p>
+
+<div class="pdoc-code codehilite">
+<pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;mydirectory&quot;</span><span class="p">)</span> <span class="o">/</span> <span class="s2">&quot;myscript.py&quot;</span>
+<span class="go">then</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">path</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="s2">&quot;py&quot;</span><span class="p">,</span> <span class="s2">&quot;--iterations 10&quot;</span><span class="p">)</span>
+<span class="go">equivalent to</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;py </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s2"> --iterations 10&quot;</span><span class="p">)</span>
+</code></pre>
+</div>
+</div>
+
+
+                            </div>
                             <div class="inherited">
                                 <h5>Inherited Members</h5>
                                 <dl>
                                     <div><dt>pathlib.Path</dt>
                                 <dd id="Pathier.cwd" class="function">cwd</dd>
                 <dd id="Pathier.home" class="function">home</dd>
                 <dd id="Pathier.samefile" class="function">samefile</dd>
@@ -1475,25 +1885,23 @@
                 <dd id="Pathier.glob" class="function">glob</dd>
                 <dd id="Pathier.rglob" class="function">rglob</dd>
                 <dd id="Pathier.absolute" class="function">absolute</dd>
                 <dd id="Pathier.resolve" class="function">resolve</dd>
                 <dd id="Pathier.stat" class="function">stat</dd>
                 <dd id="Pathier.owner" class="function">owner</dd>
                 <dd id="Pathier.group" class="function">group</dd>
-                <dd id="Pathier.open" class="function">open</dd>
                 <dd id="Pathier.read_bytes" class="function">read_bytes</dd>
                 <dd id="Pathier.read_text" class="function">read_text</dd>
                 <dd id="Pathier.readlink" class="function">readlink</dd>
                 <dd id="Pathier.chmod" class="function">chmod</dd>
                 <dd id="Pathier.lchmod" class="function">lchmod</dd>
                 <dd id="Pathier.unlink" class="function">unlink</dd>
                 <dd id="Pathier.rmdir" class="function">rmdir</dd>
                 <dd id="Pathier.lstat" class="function">lstat</dd>
                 <dd id="Pathier.rename" class="function">rename</dd>
-                <dd id="Pathier.replace" class="function">replace</dd>
                 <dd id="Pathier.symlink_to" class="function">symlink_to</dd>
                 <dd id="Pathier.hardlink_to" class="function">hardlink_to</dd>
                 <dd id="Pathier.link_to" class="function">link_to</dd>
                 <dd id="Pathier.exists" class="function">exists</dd>
                 <dd id="Pathier.is_dir" class="function">is_dir</dd>
                 <dd id="Pathier.is_file" class="function">is_file</dd>
                 <dd id="Pathier.is_mount" class="function">is_mount</dd>
@@ -1528,10 +1936,32 @@
                 <dd id="Pathier.is_reserved" class="function">is_reserved</dd>
                 <dd id="Pathier.match" class="function">match</dd>
 
             </div>
                                 </dl>
                             </div>
                 </section>
+                <section id="Pathy">
+                    <div class="attr variable">
+            <span class="name">Pathy</span><span class="default_value"> = <a href="#Pathier">pathier.Pathier</a> | pathlib.Path</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Pathy"></a>
+    
+    
+
+                </section>
+                <section id="Pathish">
+                    <div class="attr variable">
+            <span class="name">Pathish</span><span class="default_value"> = <a href="#Pathier">pathier.Pathier</a> | pathlib.Path | str</span>
+
+        
+    </div>
+    <a class="headerlink" href="#Pathish"></a>
+    
+    
+
+                </section>
     </main>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -4,47 +4,57 @@
 ***** API Documentation *****
     * Pathier
           o Pathier
           o dob
           o age
           o mod_date
           o mod_delta
+          o last_read_time
+          o modified_since_last_read
           o size
-          o format_size
+          o format_bytes
           o is_larger
           o is_older
           o modified_more_recently
           o mkcwd
           o in_PATH
           o add_to_PATH
           o append_to_PATH
           o remove_from_PATH
           o moveup
           o move_under
           o separate
           o mkdir
           o touch
+          o open
           o write_text
           o write_bytes
+          o append
+          o replace
+          o join
+          o split
           o json_loads
           o json_dumps
           o toml_loads
           o toml_dumps
           o loads
           o dumps
           o delete
           o copy
           o backup
+          o execute
+    * Pathy
+    * Pathish
 built_with_pdoc[pdoc_logo]
 
 ****** pathier ******
 ⁰ View Source
-1from .pathier import Pathier
+1from .pathier import Pathier, Pathish, Pathy
 2
-3__all__ = ["Pathier"]
+3__all__ = ["Pathier", "Pathy", "Pathish"]
   ⁰
 class Pathier(pathlib.Path): View Source
 _16class Pathier(pathlib.Path):
 _17    """Subclasses the standard library pathlib.Path class."""
 _18
 _19    def __new__(cls, *args, **kwargs):
 _20        if cls is Pathier:
@@ -56,855 +66,1209 @@
 _26            )
 _27        return self
 _28
 _29    #
 ===============================================stats===============================================
 _30    @property
 _31    def dob(self) -> datetime.datetime | None:
-_32        """Returns the creation date of this file
-_33        or directory as a dateime.datetime object."""
-_34        if self.exists():
-_35            return datetime.datetime.fromtimestamp(self.stat().st_ctime)
-_36        else:
-_37            return None
-_38
-_39    @property
-_40    def age(self) -> float | None:
-_41        """Returns the age in seconds of this file or directory."""
-_42        if self.exists():
-_43            return (datetime.datetime.now() - self.dob).total_seconds()
-_44        else:
-_45            return None
-_46
-_47    @property
-_48    def mod_date(self) -> datetime.datetime | None:
-_49        """Returns the modification date of this file
-_50        or directory as a datetime.datetime object."""
-_51        if self.exists():
-_52            return datetime.datetime.fromtimestamp(self.stat().st_mtime)
-_53        else:
-_54            return None
-_55
-_56    @property
-_57    def mod_delta(self) -> float | None:
-_58        """Returns how long ago in seconds this file
-_59        or directory was modified."""
-_60        if self.exists():
-_61            return (datetime.datetime.now() - self.mod_date).total_seconds()
-_62        else:
-_63            return None
-_64
-_65    def size(self, format: bool = False) -> int | str | None:
-_66        """Returns the size in bytes of this file or directory.
-_67        Returns None if this path doesn't exist.
-_68
-_69        :param format: If True, return value as a formatted string."""
-_70        if not self.exists():
-_71            return None
-_72        if self.is_file():
-_73            size = self.stat().st_size
-_74        if self.is_dir():
-_75            size = sum(file.stat().st_size for file in self.rglob("*.*"))
-_76        if format:
-_77            return self.format_size(size)
-_78        return size
-_79
-_80    @staticmethod
-_81    def format_size(size: int) -> str:
-_82        """Format 'size' with common file size abbreviations
-_83        and rounded to two decimal places.
-_84        >>> 1234 -> "1.23 kb" """
-_85        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
-_86            if unit != "bytes":
-_87                size *= 0.001
-_88            if size < 1000 or unit == "pb":
-_89                return f"{round(size, 2)} {unit}"
-_90
-_91    def is_larger(self, path: Self) -> bool:
-_92        """Returns whether this file or folder is larger than
-_93        the one pointed to by 'path'."""
-_94        return self.size() > path.size()
-_95
-_96    def is_older(self, path: Self) -> bool:
-_97        """Returns whether this file or folder is older than
-_98        the one pointed to by 'path'."""
-_99        return self.dob < path.dob
-100
-101    def modified_more_recently(self, path: Self) -> bool:
-102        """Returns whether this file or folder was modified
-103        more recently than the one pointed to by 'path'."""
-104        return self.mod_date > path.mod_date
-105
-106    #
+_32        """Returns the creation date of this file or directory as a
+`dateime.datetime` object."""
+_33        if self.exists():
+_34            return datetime.datetime.fromtimestamp(self.stat().st_ctime)
+_35        else:
+_36            return None
+_37
+_38    @property
+_39    def age(self) -> float | None:
+_40        """Returns the age in seconds of this file or directory."""
+_41        if self.exists():
+_42            return (datetime.datetime.now() - self.dob).total_seconds()
+_43        else:
+_44            return None
+_45
+_46    @property
+_47    def mod_date(self) -> datetime.datetime | None:
+_48        """Returns the modification date of this file or directory as a
+`datetime.datetime` object."""
+_49        if self.exists():
+_50            return datetime.datetime.fromtimestamp(self.stat().st_mtime)
+_51        else:
+_52            return None
+_53
+_54    @property
+_55    def mod_delta(self) -> float | None:
+_56        """Returns how long ago in seconds this file or directory was
+modified."""
+_57        if self.exists():
+_58            return (datetime.datetime.now() - self.mod_date).total_seconds()
+_59        else:
+_60            return None
+_61
+_62    @property
+_63    def last_read_time(self) -> datetime.datetime | None:
+_64        """Returns the last time this object made a call to `self.read_text
+()`, `self.read_bytes()`, or `self.open(mode="r"|"rb")`.
+_65        Returns `None` if the file hasn't been read from.
+_66
+_67        Note: This property is only relative to the lifetime of this
+`Pathier` instance, not the file itself.
+_68        i.e. This property will reset if you create a new `Pathier` object
+pointing to the same file."""
+_69        if self._last_read_time:
+_70            return datetime.datetime.fromtimestamp(self._last_read_time)
+_71        else:
+_72            return self._last_read_time
+_73
+_74    @property
+_75    def modified_since_last_read(self) -> bool:
+_76        """Returns `True` if this file hasn't been read from or has been
+modified since the last time this object
+_77        made a call to `self.read_text()`, `self.read_bytes()`, or
+`self.open(mode="r"|"rb")`.
+_78
+_79        Note: This property is only relative to the lifetime of this
+`Pathier` instance, not the file itself.
+_80        i.e. This property will reset if you create a new `Pathier` object
+pointing to the same file.
+_81
+_82        #### Caveat:
+_83        May not be accurate if the file was modified within a couple of
+seconds of checking this property.
+_84        (For instance, on my machine `self.mod_date` is consistently 1-1.5s
+in the future from when `self.write_text()` was called according to `time.time
+()`.)
+_85        """
+_86
+_87        return self.last_read_time is None or self.mod_date >
+self.last_read_time
+_88
+_89    @property
+_90    def size(self) -> int:
+_91        """Returns the size in bytes of this file or directory.
+_92
+_93        If this path doesn't exist, `0` will be returned."""
+_94        if not self.exists():
+_95            return 0
+_96        elif self.is_file():
+_97            return self.stat().st_size
+_98        elif self.is_dir():
+_99            return sum(file.stat().st_size for file in self.rglob("*.*"))
+100        return 0
+101
+102    @staticmethod
+103    def format_bytes(size: int) -> str:
+104        """Format `size` with common file size abbreviations and rounded to
+two decimal places.
+105        >>> 1234 -> "1.23 kb" """
+106        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
+107            if unit != "bytes":
+108                size *= 0.001
+109            if size < 1000 or unit == "pb":
+110                return f"{round(size, 2)} {unit}"
+111
+112    def is_larger(self, path: Self) -> bool:
+113        """Returns whether this file or folder is larger than the one
+pointed to by `path`."""
+114        return self.size > path.size
+115
+116    def is_older(self, path: Self) -> bool:
+117        """Returns whether this file or folder is older than the one pointed
+to by `path`."""
+118        return self.dob < path.dob
+119
+120    def modified_more_recently(self, path: Self) -> bool:
+121        """Returns whether this file or folder was modified more recently
+than the one pointed to by `path`."""
+122        return self.mod_date > path.mod_date
+123
+124    #
 ===============================================navigation===============================================
-107    def mkcwd(self):
-108        """Make this path your current working directory."""
-109        os.chdir(self)
-110
-111    @property
-112    def in_PATH(self) -> bool:
-113        """Return True if this
-114        path is in sys.path."""
-115        return str(self) in sys.path
-116
-117    def add_to_PATH(self, index: int = 0):
-118        """Insert this path into sys.path
-119        if it isn't already there.
-120
-121        :param index: The index of sys.path
-122        to insert this path at."""
-123        path = str(self)
-124        if not self.in_PATH:
-125            sys.path.insert(index, path)
-126
-127    def append_to_PATH(self):
-128        """Append this path to sys.path
-129        if it isn't already there."""
-130        path = str(self)
-131        if not self.in_PATH:
-132            sys.path.append(path)
+125    def mkcwd(self):
+126        """Make this path your current working directory."""
+127        os.chdir(self)
+128
+129    @property
+130    def in_PATH(self) -> bool:
+131        """Return `True` if this path is in `sys.path`."""
+132        return str(self) in sys.path
 133
-134    def remove_from_PATH(self):
-135        """Remove this path from sys.path
-136        if it's in sys.path."""
-137        if self.in_PATH:
-138            sys.path.remove(str(self))
-139
-140    def moveup(self, name: str) -> Self:
-141        """Return a new Pathier object that is a parent of this instance.
-142        'name' is case-sensitive and raises an exception if it isn't in
-self.parts.
-143        >>> p = Pathier("C:\some\directory\in\your\system")
-144        >>> print(p.moveup("directory"))
-145        >>> "C:\some\directory"
-146        >>> print(p.moveup("yeet"))
-147        >>> "Exception: yeet is not a parent of C:
+134    def add_to_PATH(self, index: int = 0):
+135        """Insert this path into `sys.path` if it isn't already there.
+136
+137        #### :params:
+138
+139        `index`: The index of `sys.path` to insert this path at."""
+140        path = str(self)
+141        if not self.in_PATH:
+142            sys.path.insert(index, path)
+143
+144    def append_to_PATH(self):
+145        """Append this path to `sys.path` if it isn't already there."""
+146        path = str(self)
+147        if not self.in_PATH:
+148            sys.path.append(path)
+149
+150    def remove_from_PATH(self):
+151        """Remove this path from `sys.path` if it's in `sys.path`."""
+152        if self.in_PATH:
+153            sys.path.remove(str(self))
+154
+155    def moveup(self, name: str) -> Self:
+156        """Return a new `Pathier` object that is a parent of this instance.
+157
+158        `name` is case-sensitive and raises an exception if it isn't in
+`self.parts`.
+159        >>> p = Pathier("C:\some\directory\in\your\system")
+160        >>> print(p.moveup("directory"))
+161        >>> "C:\some\directory"
+162        >>> print(p.moveup("yeet"))
+163        >>> "Exception: yeet is not a parent of C:
 \some\directory\in\your\system" """
-148        if name not in self.parts:
-149            raise Exception(f"{name} is not a parent of {self}")
-150        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
-151
-152    def __sub__(self, levels: int) -> Self:
-153        """Return a new Pathier object moved up 'levels' number of parents
+164        if name not in self.parts:
+165            raise Exception(f"{name} is not a parent of {self}")
+166        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
+167
+168    def __sub__(self, levels: int) -> Self:
+169        """Return a new `Pathier` object moved up `levels` number of parents
 from the current path.
-154        >>> p = Pathier("C:\some\directory\in\your\system")
-155        >>> new_p = p - 3
-156        >>> print(new_p)
-157        >>> "C:\some\directory" """
-158        path = self
-159        for _ in range(levels):
-160            path = path.parent
-161        return path
-162
-163    def move_under(self, name: str) -> Self:
-164        """Return a new Pathier object such that the stem
-165        is one level below the folder 'name'.
-166        'name' is case-sensitive and raises an exception if it isn't in
-self.parts.
-167        >>> p = Pathier("a/b/c/d/e/f/g")
-168        >>> print(p.move_under("c"))
-169        >>> 'a/b/c/d'"""
-170        if name not in self.parts:
-171            raise Exception(f"{name} is not a parent of {self}")
-172        return self - (len(self.parts) - self.parts.index(name) - 2)
-173
-174    def separate(self, name: str, keep_name: bool = False) -> Self:
-175        """Return a new Pathier object that is the
-176        relative child path after 'name'.
-177        'name' is case-sensitive and raises an exception if it isn't in
-self.parts.
+170        >>> p = Pathier("C:\some\directory\in\your\system")
+171        >>> new_p = p - 3
+172        >>> print(new_p)
+173        >>> "C:\some\directory" """
+174        path = self
+175        for _ in range(levels):
+176            path = path.parent
+177        return path
 178
-179        :param keep_name: If True, the returned path will start with 'name'.
-180        >>> p = Pathier("a/b/c/d/e/f/g")
-181        >>> print(p.separate("c"))
-182        >>> 'd/e/f/g'
-183        >>> print(p.separate("c", True))
-184        >>> 'c/d/e/f/g'"""
-185        if name not in self.parts:
-186            raise Exception(f"{name} is not a parent of {self}")
-187        if keep_name:
-188            return Pathier(*self.parts[self.parts.index(name) :])
-189        return Pathier(*self.parts[self.parts.index(name) + 1 :])
-190
-191    # ============================================write and
+179    def move_under(self, name: str) -> Self:
+180        """Return a new `Pathier` object such that the stem is one level
+below the given folder `name`.
+181
+182        `name` is case-sensitive and raises an exception if it isn't in
+`self.parts`.
+183        >>> p = Pathier("a/b/c/d/e/f/g")
+184        >>> print(p.move_under("c"))
+185        >>> 'a/b/c/d'"""
+186        if name not in self.parts:
+187            raise Exception(f"{name} is not a parent of {self}")
+188        return self - (len(self.parts) - self.parts.index(name) - 2)
+189
+190    def separate(self, name: str, keep_name: bool = False) -> Self:
+191        """Return a new `Pathier` object that is the relative child path
+after `name`.
+192
+193        `name` is case-sensitive and raises an exception if it isn't in
+`self.parts`.
+194
+195        #### :params:
+196
+197        `keep_name`: If `True`, the returned path will start with `name`.
+198        >>> p = Pathier("a/b/c/d/e/f/g")
+199        >>> print(p.separate("c"))
+200        >>> 'd/e/f/g'
+201        >>> print(p.separate("c", True))
+202        >>> 'c/d/e/f/g'"""
+203        if name not in self.parts:
+204            raise Exception(f"{name} is not a parent of {self}")
+205        if keep_name:
+206            return Pathier(*self.parts[self.parts.index(name) :])
+207        return Pathier(*self.parts[self.parts.index(name) + 1 :])
+208
+209    # ============================================write and
 read============================================
-192    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
+210    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
 True):
-193        """Create this directory.
-194        Same as Path().mkdir() except
-195        'parents' and 'exist_ok' default
-196        to True instead of False."""
-197        super().mkdir(mode, parents, exist_ok)
-198
-199    def touch(self):
-200        """Create file and parents if necessary."""
-201        self.parent.mkdir()
-202        super().touch()
-203
-204    def write_text(
-205        self,
-206        data: Any,
-207        encoding: Any | None = None,
-208        errors: Any | None = None,
-209        newline: Any | None = None,
-210        parents: bool = True,
-211    ):
-212        """Write data to file. If a TypeError is raised, the function
-213        will attempt to case data to a str and try the write again.
-214        If a FileNotFoundError is raised and parents = True,
-215        self.parent will be created."""
-216        write = functools.partial(
-217            super().write_text,
-218            encoding=encoding,
-219            errors=errors,
-220            newline=newline,
-221        )
-222        try:
-223            write(data)
-224        except TypeError:
-225            data = str(data)
-226            write(data)
-227        except FileNotFoundError:
-228            if parents:
-229                self.parent.mkdir(parents=True)
-230                write(data)
-231            else:
-232                raise
-233        except Exception as e:
-234            raise
-235
-236    def write_bytes(self, data: bytes, parents: bool = True):
-237        """Write bytes to file.
-238
-239        :param parents: If True and the write operation fails
-240        with a FileNotFoundError, make the parent directory
-241        and retry the write."""
-242        try:
-243            super().write_bytes(data)
-244        except FileNotFoundError:
-245            if parents:
-246                self.parent.mkdir(parents=True)
-247                super().write_bytes(data)
-248            else:
-249                raise
-250        except Exception as e:
-251            raise
-252
-253    def json_loads(self, encoding: Any | None = None, errors: Any | None =
+211        """Create this directory.
+212
+213        Same as `Path().mkdir()` except `parents` and `exist_ok` default to
+`True` instead of `False`."""
+214        super().mkdir(mode, parents, exist_ok)
+215
+216    def touch(self):
+217        """Create file (and parents if necessary)."""
+218        self.parent.mkdir()
+219        super().touch()
+220
+221    def open(self, mode="r", buffering=-1, encoding=None, errors=None,
+newline=None):
+222        """
+223        Open the file pointed by this path and return a file object, as
+224        the built-in open() function does.
+225        """
+226        stream = super().open(mode, buffering, encoding, errors, newline)
+227        if "r" in mode:
+228            self._last_read_time = time.time()
+229        return stream
+230
+231    def write_text(
+232        self,
+233        data: Any,
+234        encoding: Any | None = None,
+235        errors: Any | None = None,
+236        newline: Any | None = None,
+237        parents: bool = True,
+238    ):
+239        """Write data to file.
+240
+241        If a `TypeError` is raised, the function  will attempt to cast
+`data` to a `str` and try the write again.
+242
+243        If a `FileNotFoundError` is raised and `parents = True`,
+`self.parent` will be created."""
+244        write = functools.partial(
+245            super().write_text,
+246            encoding=encoding,
+247            errors=errors,
+248            newline=newline,
+249        )
+250        try:
+251            write(data)
+252        except TypeError:
+253            data = str(data)
+254            write(data)
+255        except FileNotFoundError:
+256            if parents:
+257                self.parent.mkdir(parents=True)
+258                write(data)
+259            else:
+260                raise
+261        except Exception as e:
+262            raise
+263
+264    def write_bytes(self, data: bytes, parents: bool = True):
+265        """Write bytes to file.
+266
+267        #### :params:
+268
+269        `parents`: If `True` and the write operation fails with a
+`FileNotFoundError`,
+270        make the parent directory and retry the write."""
+271        try:
+272            super().write_bytes(data)
+273        except FileNotFoundError:
+274            if parents:
+275                self.parent.mkdir(parents=True)
+276                super().write_bytes(data)
+277            else:
+278                raise
+279        except Exception as e:
+280            raise
+281
+282    def append(self, data: str, new_line: bool = True, encoding: Any | None
+= None):
+283        """Append `data` to the file pointed to by this `Pathier` object.
+284
+285        #### :params:
+286
+287        `new_line`: If `True`, add `\\n` to `data`.
+288
+289        `encoding`: The file encoding to use."""
+290        if new_line:
+291            data += "\n"
+292        with self.open("a", encoding=encoding) as file:
+293            file.write(data)
+294
+295    def replace(
+296        self,
+297        substitutions: list[tuple[str, str]],
+298        count: int = -1,
+299        encoding: Any | None = None,
+300    ):
+301        """For each pair in `substitutions`, replace the first string with
+the second string.
+302
+303        #### :params:
+304
+305        `count`: Only replace this many occurences of each pair.
+306        By default (`-1`), all occurences are replaced.
+307
+308        `encoding`: The file encoding to use.
+309
+310        e.g.
+311        >>> path = Pathier("somefile.txt")
+312        >>>
+313        >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
+314        equivalent to
+315        >>> path.write_text(path.read_text().replace("hello",
+"yeet").replace("goodbye", "yeehaw"))"""
+316        text = self.read_text(encoding)
+317        for sub in substitutions:
+318            text = text.replace(sub[0], sub[1], count)
+319        self.write_text(text, encoding=encoding)
+320
+321    def join(self, data: list[str], encoding: Any | None = None, sep: str =
+"\n"):
+322        """Write a list of strings, joined by `sep`, to the file pointed at
+by this instance.
+323
+324        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
+encoding=encoding)`
+325
+326        #### :params:
+327
+328        `encoding`: The file encoding to use.
+329
+330        `sep`: The separator to use when joining `data`."""
+331        self.write_text(sep.join(data), encoding=encoding)
+332
+333    def split(self, encoding: Any | None = None, keepends: bool = False) -
+> list[str]:
+334        """Returns the content of the pointed at file as a list of strings,
+splitting at new line characters.
+335
+336        Equivalent to `Pathier("somefile.txt").read_text
+(encoding=encoding).splitlines()`
+337
+338        #### :params:
+339
+340        `encoding`: The file encoding to use.
+341
+342        `keepend`: If `True`, line breaks will be included in returned
+strings."""
+343        return self.read_text(encoding=encoding).splitlines(keepends)
+344
+345    def json_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-254        """Load json file."""
-255        return json.loads(self.read_text(encoding, errors))
-256
-257    def json_dumps(
-258        self,
-259        data: Any,
-260        encoding: Any | None = None,
-261        errors: Any | None = None,
-262        newline: Any | None = None,
-263        sort_keys: bool = False,
-264        indent: Any | None = None,
-265        default: Any | None = None,
-266        parents: bool = True,
-267    ) -> Any:
-268        """Dump data to json file."""
-269        self.write_text(
-270            json.dumps(data, indent=indent, default=default,
+346        """Load json file."""
+347        return json.loads(self.read_text(encoding, errors))
+348
+349    def json_dumps(
+350        self,
+351        data: Any,
+352        encoding: Any | None = None,
+353        errors: Any | None = None,
+354        newline: Any | None = None,
+355        sort_keys: bool = False,
+356        indent: Any | None = None,
+357        default: Any | None = None,
+358        parents: bool = True,
+359    ) -> Any:
+360        """Dump `data` to json file."""
+361        self.write_text(
+362            json.dumps(data, indent=indent, default=default,
 sort_keys=sort_keys),
-271            encoding,
-272            errors,
-273            newline,
-274            parents,
-275        )
-276
-277    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
+363            encoding,
+364            errors,
+365            newline,
+366            parents,
+367        )
+368
+369    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-278        """Load toml file."""
-279        return tomlkit.loads(self.read_text(encoding, errors))
-280
-281    def toml_dumps(
-282        self,
-283        data: Any,
-284        encoding: Any | None = None,
-285        errors: Any | None = None,
-286        newline: Any | None = None,
-287        sort_keys: bool = False,
-288        parents: bool = True,
-289    ):
-290        """Dump data to toml file."""
-291        self.write_text(
-292            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
+370        """Load toml file."""
+371        return tomlkit.loads(self.read_text(encoding, errors)).unwrap()
+372
+373    def toml_dumps(
+374        self,
+375        data: Any,
+376        encoding: Any | None = None,
+377        errors: Any | None = None,
+378        newline: Any | None = None,
+379        sort_keys: bool = False,
+380        parents: bool = True,
+381    ):
+382        """Dump `data` to toml file."""
+383        self.write_text(
+384            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
 parents
-293        )
-294
-295    def loads(self, encoding: Any | None = None, errors: Any | None = None)
+385        )
+386
+387    def loads(self, encoding: Any | None = None, errors: Any | None = None)
 -> Any:
-296        """Load a json or toml file based off this instance's suffix."""
-297        match self.suffix:
-298            case ".json":
-299                return self.json_loads(encoding, errors)
-300            case ".toml":
-301                return self.toml_loads(encoding, errors)
-302
-303    def dumps(
-304        self,
-305        data: Any,
-306        encoding: Any | None = None,
-307        errors: Any | None = None,
-308        newline: Any | None = None,
-309        sort_keys: bool = False,
-310        indent: Any | None = None,
-311        default: Any | None = None,
-312        parents: bool = True,
-313    ):
-314        """Dump data to a json or toml file based off this instance's
+388        """Load a json or toml file based off this instance's suffix."""
+389        match self.suffix:
+390            case ".json":
+391                return self.json_loads(encoding, errors)
+392            case ".toml":
+393                return self.toml_loads(encoding, errors)
+394
+395    def dumps(
+396        self,
+397        data: Any,
+398        encoding: Any | None = None,
+399        errors: Any | None = None,
+400        newline: Any | None = None,
+401        sort_keys: bool = False,
+402        indent: Any | None = None,
+403        default: Any | None = None,
+404        parents: bool = True,
+405    ):
+406        """Dump `data` to a json or toml file based off this instance's
 suffix."""
-315        match self.suffix:
-316            case ".json":
-317                self.json_dumps(
-318                    data, encoding, errors, newline, sort_keys, indent,
+407        match self.suffix:
+408            case ".json":
+409                self.json_dumps(
+410                    data, encoding, errors, newline, sort_keys, indent,
 default, parents
-319                )
-320            case ".toml":
-321                self.toml_dumps(data, encoding, errors, newline, sort_keys,
+411                )
+412            case ".toml":
+413                self.toml_dumps(data, encoding, errors, newline, sort_keys,
 parents)
-322
-323    def delete(self, missing_ok: bool = True):
-324        """Delete the file or folder pointed to by this instance.
-325        Uses self.unlink() if a file and uses shutil.rmtree() if a
+414
+415    def delete(self, missing_ok: bool = True):
+416        """Delete the file or folder pointed to by this instance.
+417
+418        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a
 directory."""
-326        if self.is_file():
-327            self.unlink(missing_ok)
-328        elif self.is_dir():
-329            shutil.rmtree(self)
-330
-331    def copy(
-332        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
-333    ) -> Self:
-334        """Copy the path pointed to by this instance
-335        to the instance pointed to by new_path using shutil.copyfile
-336        or shutil.copytree. Returns the new path.
-337
-338        :param new_path: The copy destination.
-339
-340        :param overwrite: If True, files already existing in new_path
-341        will be overwritten. If False, only files that don't exist in
-new_path
-342        will be copied."""
-343        new_path = Pathier(new_path)
-344        if self.is_dir():
-345            if overwrite or not new_path.exists():
-346                shutil.copytree(self, new_path, dirs_exist_ok=True)
-347            else:
-348                files = self.rglob("*.*")
-349                for file in files:
-350                    dst = new_path.with_name(file.name)
-351                    if not dst.exists():
-352                        shutil.copyfile(file, dst)
-353        elif self.is_file():
-354            if overwrite or not new_path.exists():
-355                shutil.copyfile(self, new_path)
-356        return new_path
-357
-358    def backup(self, timestamp: bool = False) -> Self | None:
-359        """Create a copy of this file or directory with `_backup` appended
+419        if self.is_file():
+420            self.unlink(missing_ok)
+421        elif self.is_dir():
+422            shutil.rmtree(self)
+423
+424    def copy(
+425        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
+426    ) -> Self:
+427        """Copy the path pointed to by this instance
+428        to the instance pointed to by `new_path` using `shutil.copyfile`
+429        or `shutil.copytree`.
+430
+431        Returns the new path.
+432
+433        #### :params:
+434
+435        `new_path`: The copy destination.
+436
+437        `overwrite`: If `True`, files already existing in `new_path` will be
+overwritten.
+438        If `False`, only files that don't exist in `new_path` will be
+copied."""
+439        new_path = Pathier(new_path)
+440        if self.is_dir():
+441            if overwrite or not new_path.exists():
+442                shutil.copytree(self, new_path, dirs_exist_ok=True)
+443            else:
+444                files = self.rglob("*.*")
+445                for file in files:
+446                    dst = new_path.with_name(file.name)
+447                    if not dst.exists():
+448                        shutil.copyfile(file, dst)
+449        elif self.is_file():
+450            if overwrite or not new_path.exists():
+451                shutil.copyfile(self, new_path)
+452        return new_path
+453
+454    def backup(self, timestamp: bool = False) -> Self | None:
+455        """Create a copy of this file or directory with `_backup` appended
 to the path stem.
-360        If the path to be backed up doesn't exist, `None` is returned.
-361        Otherwise a `Pathier` object for the backup is returned.
-362
-363        :param `timestamp`: Add a timestamp to the backup name to prevent
+456        If the path to be backed up doesn't exist, `None` is returned.
+457        Otherwise a `Pathier` object for the backup is returned.
+458
+459        #### :params:
+460
+461        `timestamp`: Add a timestamp to the backup name to prevent
 overriding previous backups.
-364
-365        >>> path = Pathier("some_file.txt")
-366        >>> path.backup()
-367        >>> list(path.iterdir())
-368        >>> ['some_file.txt', 'some_file_backup.txt']
-369        >>> path.backup(True)
-370        >>> list(path.iterdir())
-371        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
+462
+463        >>> path = Pathier("some_file.txt")
+464        >>> path.backup()
+465        >>> list(path.iterdir())
+466        >>> ['some_file.txt', 'some_file_backup.txt']
+467        >>> path.backup(True)
+468        >>> list(path.iterdir())
+469        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
 28-2023-06_25_52_PM.txt']"""
-372        if not self.exists():
-373            return None
-374        backup_stem = f"{self.stem}_backup"
-375        if timestamp:
-376            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
+470        if not self.exists():
+471            return None
+472        backup_stem = f"{self.stem}_backup"
+473        if timestamp:
+474            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
 ('%m-%d-%Y-%I_%M_%S_%p')}"
-377        backup_path = self.with_stem(backup_stem)
-378        self.copy(backup_path, True)
-379        return backup_path
+475        backup_path = self.with_stem(backup_stem)
+476        self.copy(backup_path, True)
+477        return backup_path
+478
+479    def execute(self, command: str = "", args: str = "") -> int:
+480        """Make a call to `os.system` using the path pointed to by this
+Pathier object.
+481
+482        #### :params:
+483
+484        `command`: Program/command to precede the path with.
+485
+486        `args`: Any arguments that should come after the path.
+487
+488        :returns: The integer output of `os.system`.
+489
+490        e.g.
+491        >>> path = Pathier("mydirectory") / "myscript.py"
+492        then
+493        >>> path.execute("py", "--iterations 10")
+494        equivalent to
+495        >>> os.system(f"py {path} --iterations 10")"""
+496        return os.system(f"{command} {self} {args}")
 Subclasses the standard library pathlib.Path class.
 Pathier()
 dob: datetime.datetime | None
 Returns the creation date of this file or directory as a dateime.datetime
 object.
 age: float | None
 Returns the age in seconds of this file or directory.
 mod_date: datetime.datetime | None
 Returns the modification date of this file or directory as a datetime.datetime
 object.
 mod_delta: float | None
 Returns how long ago in seconds this file or directory was modified.
-⁰
-def size(self, format: bool = False) -> int | str | None: View Source
-65    def size(self, format: bool = False) -> int | str | None:
-66        """Returns the size in bytes of this file or directory.
-67        Returns None if this path doesn't exist.
-68
-69        :param format: If True, return value as a formatted string."""
-70        if not self.exists():
-71            return None
-72        if self.is_file():
-73            size = self.stat().st_size
-74        if self.is_dir():
-75            size = sum(file.stat().st_size for file in self.rglob("*.*"))
-76        if format:
-77            return self.format_size(size)
-78        return size
-Returns the size in bytes of this file or directory. Returns None if this path
-doesn't exist.
-* Parameters *
-    * format: If True, return value as a formatted string.
+last_read_time: datetime.datetime | None
+Returns the last time this object made a call to self.read_text(),
+self.read_bytes(), or self.open(mode="r"|"rb"). Returns None if the file hasn't
+been read from.
+Note: This property is only relative to the lifetime of this Pathier instance,
+not the file itself. i.e. This property will reset if you create a new Pathier
+object pointing to the same file.
+modified_since_last_read: bool
+Returns True if this file hasn't been read from or has been modified since the
+last time this object made a call to self.read_text(), self.read_bytes(), or
+self.open(mode="r"|"rb").
+Note: This property is only relative to the lifetime of this Pathier instance,
+not the file itself. i.e. This property will reset if you create a new Pathier
+object pointing to the same file.
+*** Caveat: ***
+May not be accurate if the file was modified within a couple of seconds of
+checking this property. (For instance, on my machine self.mod_date is
+consistently 1-1.5s in the future from when self.write_text() was called
+according to time.time().)
+size: int
+Returns the size in bytes of this file or directory.
+If this path doesn't exist, 0 will be returned.
 ⁰
 @staticmethod
-def format_size(size: int) -> str: View Source
-80    @staticmethod
-81    def format_size(size: int) -> str:
-82        """Format 'size' with common file size abbreviations
-83        and rounded to two decimal places.
-84        >>> 1234 -> "1.23 kb" """
-85        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
-86            if unit != "bytes":
-87                size *= 0.001
-88            if size < 1000 or unit == "pb":
-89                return f"{round(size, 2)} {unit}"
-Format 'size' with common file size abbreviations and rounded to two decimal
+def format_bytes(size: int) -> str: View Source
+102    @staticmethod
+103    def format_bytes(size: int) -> str:
+104        """Format `size` with common file size abbreviations and rounded to
+two decimal places.
+105        >>> 1234 -> "1.23 kb" """
+106        for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
+107            if unit != "bytes":
+108                size *= 0.001
+109            if size < 1000 or unit == "pb":
+110                return f"{round(size, 2)} {unit}"
+Format size with common file size abbreviations and rounded to two decimal
 places.
 >>> 1234 -> "1.23 kb"
 ⁰
 def is_larger(self, path: Self) -> bool: View Source
-91    def is_larger(self, path: Self) -> bool:
-92        """Returns whether this file or folder is larger than
-93        the one pointed to by 'path'."""
-94        return self.size() > path.size()
-Returns whether this file or folder is larger than the one pointed to by
-'path'.
+112    def is_larger(self, path: Self) -> bool:
+113        """Returns whether this file or folder is larger than the one
+pointed to by `path`."""
+114        return self.size > path.size
+Returns whether this file or folder is larger than the one pointed to by path.
 ⁰
 def is_older(self, path: Self) -> bool: View Source
-96    def is_older(self, path: Self) -> bool:
-97        """Returns whether this file or folder is older than
-98        the one pointed to by 'path'."""
-99        return self.dob < path.dob
-Returns whether this file or folder is older than the one pointed to by 'path'.
+116    def is_older(self, path: Self) -> bool:
+117        """Returns whether this file or folder is older than the one pointed
+to by `path`."""
+118        return self.dob < path.dob
+Returns whether this file or folder is older than the one pointed to by path.
 ⁰
 def modified_more_recently(self, path: Self) -> bool: View Source
-101    def modified_more_recently(self, path: Self) -> bool:
-102        """Returns whether this file or folder was modified
-103        more recently than the one pointed to by 'path'."""
-104        return self.mod_date > path.mod_date
+120    def modified_more_recently(self, path: Self) -> bool:
+121        """Returns whether this file or folder was modified more recently
+than the one pointed to by `path`."""
+122        return self.mod_date > path.mod_date
 Returns whether this file or folder was modified more recently than the one
-pointed to by 'path'.
+pointed to by path.
 ⁰
 def mkcwd(self): View Source
-107    def mkcwd(self):
-108        """Make this path your current working directory."""
-109        os.chdir(self)
+125    def mkcwd(self):
+126        """Make this path your current working directory."""
+127        os.chdir(self)
 Make this path your current working directory.
 in_PATH: bool
 Return True if this path is in sys.path.
 ⁰
 def add_to_PATH(self, index: int = 0): View Source
-117    def add_to_PATH(self, index: int = 0):
-118        """Insert this path into sys.path
-119        if it isn't already there.
-120
-121        :param index: The index of sys.path
-122        to insert this path at."""
-123        path = str(self)
-124        if not self.in_PATH:
-125            sys.path.insert(index, path)
+134    def add_to_PATH(self, index: int = 0):
+135        """Insert this path into `sys.path` if it isn't already there.
+136
+137        #### :params:
+138
+139        `index`: The index of `sys.path` to insert this path at."""
+140        path = str(self)
+141        if not self.in_PATH:
+142            sys.path.insert(index, path)
 Insert this path into sys.path if it isn't already there.
-* Parameters *
-    * index: The index of sys.path to insert this path at.
+*** :params: ***
+index: The index of sys.path to insert this path at.
 ⁰
 def append_to_PATH(self): View Source
-127    def append_to_PATH(self):
-128        """Append this path to sys.path
-129        if it isn't already there."""
-130        path = str(self)
-131        if not self.in_PATH:
-132            sys.path.append(path)
+144    def append_to_PATH(self):
+145        """Append this path to `sys.path` if it isn't already there."""
+146        path = str(self)
+147        if not self.in_PATH:
+148            sys.path.append(path)
 Append this path to sys.path if it isn't already there.
 ⁰
 def remove_from_PATH(self): View Source
-134    def remove_from_PATH(self):
-135        """Remove this path from sys.path
-136        if it's in sys.path."""
-137        if self.in_PATH:
-138            sys.path.remove(str(self))
+150    def remove_from_PATH(self):
+151        """Remove this path from `sys.path` if it's in `sys.path`."""
+152        if self.in_PATH:
+153            sys.path.remove(str(self))
 Remove this path from sys.path if it's in sys.path.
 ⁰
 def moveup(self, name: str) -> Self: View Source
-140    def moveup(self, name: str) -> Self:
-141        """Return a new Pathier object that is a parent of this instance.
-142        'name' is case-sensitive and raises an exception if it isn't in
-self.parts.
-143        >>> p = Pathier("C:\some\directory\in\your\system")
-144        >>> print(p.moveup("directory"))
-145        >>> "C:\some\directory"
-146        >>> print(p.moveup("yeet"))
-147        >>> "Exception: yeet is not a parent of C:
+155    def moveup(self, name: str) -> Self:
+156        """Return a new `Pathier` object that is a parent of this instance.
+157
+158        `name` is case-sensitive and raises an exception if it isn't in
+`self.parts`.
+159        >>> p = Pathier("C:\some\directory\in\your\system")
+160        >>> print(p.moveup("directory"))
+161        >>> "C:\some\directory"
+162        >>> print(p.moveup("yeet"))
+163        >>> "Exception: yeet is not a parent of C:
 \some\directory\in\your\system" """
-148        if name not in self.parts:
-149            raise Exception(f"{name} is not a parent of {self}")
-150        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
-Return a new Pathier object that is a parent of this instance. 'name' is case-
-sensitive and raises an exception if it isn't in self.parts.
+164        if name not in self.parts:
+165            raise Exception(f"{name} is not a parent of {self}")
+166        return Pathier(*(self.parts[: self.parts.index(name) + 1]))
+Return a new Pathier object that is a parent of this instance.
+name is case-sensitive and raises an exception if it isn't in self.parts.
 >>> p = Pathier("C:\some\directory\in\your\system")
 >>> print(p.moveup("directory"))
 >>> "C:\some\directory"
 >>> print(p.moveup("yeet"))
 >>> "Exception: yeet is not a parent of C:\some\directory\in\your\system"
 ⁰
 def move_under(self, name: str) -> Self: View Source
-163    def move_under(self, name: str) -> Self:
-164        """Return a new Pathier object such that the stem
-165        is one level below the folder 'name'.
-166        'name' is case-sensitive and raises an exception if it isn't in
-self.parts.
-167        >>> p = Pathier("a/b/c/d/e/f/g")
-168        >>> print(p.move_under("c"))
-169        >>> 'a/b/c/d'"""
-170        if name not in self.parts:
-171            raise Exception(f"{name} is not a parent of {self}")
-172        return self - (len(self.parts) - self.parts.index(name) - 2)
-Return a new Pathier object such that the stem is one level below the folder
-'name'. 'name' is case-sensitive and raises an exception if it isn't in
-self.parts.
+179    def move_under(self, name: str) -> Self:
+180        """Return a new `Pathier` object such that the stem is one level
+below the given folder `name`.
+181
+182        `name` is case-sensitive and raises an exception if it isn't in
+`self.parts`.
+183        >>> p = Pathier("a/b/c/d/e/f/g")
+184        >>> print(p.move_under("c"))
+185        >>> 'a/b/c/d'"""
+186        if name not in self.parts:
+187            raise Exception(f"{name} is not a parent of {self}")
+188        return self - (len(self.parts) - self.parts.index(name) - 2)
+Return a new Pathier object such that the stem is one level below the given
+folder name.
+name is case-sensitive and raises an exception if it isn't in self.parts.
 >>> p = Pathier("a/b/c/d/e/f/g")
 >>> print(p.move_under("c"))
 >>> 'a/b/c/d'
 ⁰
 def separate(self, name: str, keep_name: bool = False) -> Self: View Source
-174    def separate(self, name: str, keep_name: bool = False) -> Self:
-175        """Return a new Pathier object that is the
-176        relative child path after 'name'.
-177        'name' is case-sensitive and raises an exception if it isn't in
-self.parts.
-178
-179        :param keep_name: If True, the returned path will start with 'name'.
-180        >>> p = Pathier("a/b/c/d/e/f/g")
-181        >>> print(p.separate("c"))
-182        >>> 'd/e/f/g'
-183        >>> print(p.separate("c", True))
-184        >>> 'c/d/e/f/g'"""
-185        if name not in self.parts:
-186            raise Exception(f"{name} is not a parent of {self}")
-187        if keep_name:
-188            return Pathier(*self.parts[self.parts.index(name) :])
-189        return Pathier(*self.parts[self.parts.index(name) + 1 :])
-Return a new Pathier object that is the relative child path after 'name'.
-'name' is case-sensitive and raises an exception if it isn't in self.parts.
-* Parameters *
-    * keep_name: If True, the returned path will start with 'name'. >>> p =
-      Pathier("a/b/c/d/e/f/g") >>> print(p.separate("c")) >>> 'd/e/f/g' >>>
-      print(p.separate("c", True)) >>> 'c/d/e/f/g'
+190    def separate(self, name: str, keep_name: bool = False) -> Self:
+191        """Return a new `Pathier` object that is the relative child path
+after `name`.
+192
+193        `name` is case-sensitive and raises an exception if it isn't in
+`self.parts`.
+194
+195        #### :params:
+196
+197        `keep_name`: If `True`, the returned path will start with `name`.
+198        >>> p = Pathier("a/b/c/d/e/f/g")
+199        >>> print(p.separate("c"))
+200        >>> 'd/e/f/g'
+201        >>> print(p.separate("c", True))
+202        >>> 'c/d/e/f/g'"""
+203        if name not in self.parts:
+204            raise Exception(f"{name} is not a parent of {self}")
+205        if keep_name:
+206            return Pathier(*self.parts[self.parts.index(name) :])
+207        return Pathier(*self.parts[self.parts.index(name) + 1 :])
+Return a new Pathier object that is the relative child path after name.
+name is case-sensitive and raises an exception if it isn't in self.parts.
+*** :params: ***
+keep_name: If True, the returned path will start with name.
+>>> p = Pathier("a/b/c/d/e/f/g")
+>>> print(p.separate("c"))
+>>> 'd/e/f/g'
+>>> print(p.separate("c", True))
+>>> 'c/d/e/f/g'
 ⁰
 def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool = True):
 View Source
-192    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
+210    def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool =
 True):
-193        """Create this directory.
-194        Same as Path().mkdir() except
-195        'parents' and 'exist_ok' default
-196        to True instead of False."""
-197        super().mkdir(mode, parents, exist_ok)
-Create this directory. Same as Path().mkdir() except 'parents' and 'exist_ok'
-default to True instead of False.
+211        """Create this directory.
+212
+213        Same as `Path().mkdir()` except `parents` and `exist_ok` default to
+`True` instead of `False`."""
+214        super().mkdir(mode, parents, exist_ok)
+Create this directory.
+Same as Path().mkdir() except parents and exist_ok default to True instead of
+False.
 ⁰
 def touch(self): View Source
-199    def touch(self):
-200        """Create file and parents if necessary."""
-201        self.parent.mkdir()
-202        super().touch()
-Create file and parents if necessary.
+216    def touch(self):
+217        """Create file (and parents if necessary)."""
+218        self.parent.mkdir()
+219        super().touch()
+Create file (and parents if necessary).
+⁰
+def open(
+self,
+mode='r',
+buffering=-1,
+encoding=None,
+errors=None,
+newline=None): View Source
+221    def open(self, mode="r", buffering=-1, encoding=None, errors=None,
+newline=None):
+222        """
+223        Open the file pointed by this path and return a file object, as
+224        the built-in open() function does.
+225        """
+226        stream = super().open(mode, buffering, encoding, errors, newline)
+227        if "r" in mode:
+228            self._last_read_time = time.time()
+229        return stream
+Open the file pointed by this path and return a file object, as the built-in
+open() function does.
 ⁰
 def write_text(
 self,
 data: Any,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None,
 newline: typing.Any | None = None,
 parents: bool = True): View Source
-204    def write_text(
-205        self,
-206        data: Any,
-207        encoding: Any | None = None,
-208        errors: Any | None = None,
-209        newline: Any | None = None,
-210        parents: bool = True,
-211    ):
-212        """Write data to file. If a TypeError is raised, the function
-213        will attempt to case data to a str and try the write again.
-214        If a FileNotFoundError is raised and parents = True,
-215        self.parent will be created."""
-216        write = functools.partial(
-217            super().write_text,
-218            encoding=encoding,
-219            errors=errors,
-220            newline=newline,
-221        )
-222        try:
-223            write(data)
-224        except TypeError:
-225            data = str(data)
-226            write(data)
-227        except FileNotFoundError:
-228            if parents:
-229                self.parent.mkdir(parents=True)
-230                write(data)
-231            else:
-232                raise
-233        except Exception as e:
-234            raise
-Write data to file. If a TypeError is raised, the function will attempt to case
-data to a str and try the write again. If a FileNotFoundError is raised and
-parents = True, self.parent will be created.
+231    def write_text(
+232        self,
+233        data: Any,
+234        encoding: Any | None = None,
+235        errors: Any | None = None,
+236        newline: Any | None = None,
+237        parents: bool = True,
+238    ):
+239        """Write data to file.
+240
+241        If a `TypeError` is raised, the function  will attempt to cast
+`data` to a `str` and try the write again.
+242
+243        If a `FileNotFoundError` is raised and `parents = True`,
+`self.parent` will be created."""
+244        write = functools.partial(
+245            super().write_text,
+246            encoding=encoding,
+247            errors=errors,
+248            newline=newline,
+249        )
+250        try:
+251            write(data)
+252        except TypeError:
+253            data = str(data)
+254            write(data)
+255        except FileNotFoundError:
+256            if parents:
+257                self.parent.mkdir(parents=True)
+258                write(data)
+259            else:
+260                raise
+261        except Exception as e:
+262            raise
+Write data to file.
+If a TypeError is raised, the function will attempt to cast data to a str and
+try the write again.
+If a FileNotFoundError is raised and parents = True, self.parent will be
+created.
 ⁰
 def write_bytes(self, data: bytes, parents: bool = True): View Source
-236    def write_bytes(self, data: bytes, parents: bool = True):
-237        """Write bytes to file.
-238
-239        :param parents: If True and the write operation fails
-240        with a FileNotFoundError, make the parent directory
-241        and retry the write."""
-242        try:
-243            super().write_bytes(data)
-244        except FileNotFoundError:
-245            if parents:
-246                self.parent.mkdir(parents=True)
-247                super().write_bytes(data)
-248            else:
-249                raise
-250        except Exception as e:
-251            raise
+264    def write_bytes(self, data: bytes, parents: bool = True):
+265        """Write bytes to file.
+266
+267        #### :params:
+268
+269        `parents`: If `True` and the write operation fails with a
+`FileNotFoundError`,
+270        make the parent directory and retry the write."""
+271        try:
+272            super().write_bytes(data)
+273        except FileNotFoundError:
+274            if parents:
+275                self.parent.mkdir(parents=True)
+276                super().write_bytes(data)
+277            else:
+278                raise
+279        except Exception as e:
+280            raise
 Write bytes to file.
-* Parameters *
-    * parents: If True and the write operation fails with a FileNotFoundError,
-      make the parent directory and retry the write.
+*** :params: ***
+parents: If True and the write operation fails with a FileNotFoundError, make
+the parent directory and retry the write.
+⁰
+def append(
+self,
+data: str,
+new_line: bool = True,
+encoding: typing.Any | None = None): View Source
+282    def append(self, data: str, new_line: bool = True, encoding: Any | None
+= None):
+283        """Append `data` to the file pointed to by this `Pathier` object.
+284
+285        #### :params:
+286
+287        `new_line`: If `True`, add `\\n` to `data`.
+288
+289        `encoding`: The file encoding to use."""
+290        if new_line:
+291            data += "\n"
+292        with self.open("a", encoding=encoding) as file:
+293            file.write(data)
+Append data to the file pointed to by this Pathier object.
+*** :params: ***
+new_line: If True, add \n to data.
+encoding: The file encoding to use.
+⁰
+def replace(
+self,
+substitutions: list[tuple[str, str]],
+count: int = -1,
+encoding: typing.Any | None = None): View Source
+295    def replace(
+296        self,
+297        substitutions: list[tuple[str, str]],
+298        count: int = -1,
+299        encoding: Any | None = None,
+300    ):
+301        """For each pair in `substitutions`, replace the first string with
+the second string.
+302
+303        #### :params:
+304
+305        `count`: Only replace this many occurences of each pair.
+306        By default (`-1`), all occurences are replaced.
+307
+308        `encoding`: The file encoding to use.
+309
+310        e.g.
+311        >>> path = Pathier("somefile.txt")
+312        >>>
+313        >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
+314        equivalent to
+315        >>> path.write_text(path.read_text().replace("hello",
+"yeet").replace("goodbye", "yeehaw"))"""
+316        text = self.read_text(encoding)
+317        for sub in substitutions:
+318            text = text.replace(sub[0], sub[1], count)
+319        self.write_text(text, encoding=encoding)
+For each pair in substitutions, replace the first string with the second
+string.
+*** :params: ***
+count: Only replace this many occurences of each pair. By default (-1), all
+occurences are replaced.
+encoding: The file encoding to use.
+e.g.
+>>> path = Pathier("somefile.txt")
+>>>
+>>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
+equivalent to
+>>> path.write_text(path.read_text().replace("hello", "yeet").replace
+("goodbye", "yeehaw"))
+⁰
+def join(
+self,
+data: list[str],
+encoding: typing.Any | None = None,
+sep: str = '\n'): View Source
+321    def join(self, data: list[str], encoding: Any | None = None, sep: str =
+"\n"):
+322        """Write a list of strings, joined by `sep`, to the file pointed at
+by this instance.
+323
+324        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
+encoding=encoding)`
+325
+326        #### :params:
+327
+328        `encoding`: The file encoding to use.
+329
+330        `sep`: The separator to use when joining `data`."""
+331        self.write_text(sep.join(data), encoding=encoding)
+Write a list of strings, joined by sep, to the file pointed at by this
+instance.
+Equivalent to Pathier("somefile.txt").write_text(sep.join(data),
+encoding=encoding)
+*** :params: ***
+encoding: The file encoding to use.
+sep: The separator to use when joining data.
+⁰
+def split(
+self,
+encoding: typing.Any | None = None,
+keepends: bool = False) -> list[str]: View Source
+333    def split(self, encoding: Any | None = None, keepends: bool = False) -
+> list[str]:
+334        """Returns the content of the pointed at file as a list of strings,
+splitting at new line characters.
+335
+336        Equivalent to `Pathier("somefile.txt").read_text
+(encoding=encoding).splitlines()`
+337
+338        #### :params:
+339
+340        `encoding`: The file encoding to use.
+341
+342        `keepend`: If `True`, line breaks will be included in returned
+strings."""
+343        return self.read_text(encoding=encoding).splitlines(keepends)
+Returns the content of the pointed at file as a list of strings, splitting at
+new line characters.
+Equivalent to Pathier("somefile.txt").read_text(encoding=encoding).splitlines()
+*** :params: ***
+encoding: The file encoding to use.
+keepend: If True, line breaks will be included in returned strings.
 ⁰
 def json_loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-253    def json_loads(self, encoding: Any | None = None, errors: Any | None =
+345    def json_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-254        """Load json file."""
-255        return json.loads(self.read_text(encoding, errors))
+346        """Load json file."""
+347        return json.loads(self.read_text(encoding, errors))
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
-257    def json_dumps(
-258        self,
-259        data: Any,
-260        encoding: Any | None = None,
-261        errors: Any | None = None,
-262        newline: Any | None = None,
-263        sort_keys: bool = False,
-264        indent: Any | None = None,
-265        default: Any | None = None,
-266        parents: bool = True,
-267    ) -> Any:
-268        """Dump data to json file."""
-269        self.write_text(
-270            json.dumps(data, indent=indent, default=default,
+349    def json_dumps(
+350        self,
+351        data: Any,
+352        encoding: Any | None = None,
+353        errors: Any | None = None,
+354        newline: Any | None = None,
+355        sort_keys: bool = False,
+356        indent: Any | None = None,
+357        default: Any | None = None,
+358        parents: bool = True,
+359    ) -> Any:
+360        """Dump `data` to json file."""
+361        self.write_text(
+362            json.dumps(data, indent=indent, default=default,
 sort_keys=sort_keys),
-271            encoding,
-272            errors,
-273            newline,
-274            parents,
-275        )
+363            encoding,
+364            errors,
+365            newline,
+366            parents,
+367        )
 Dump data to json file.
 ⁰
 def toml_loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-277    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
+369    def toml_loads(self, encoding: Any | None = None, errors: Any | None =
 None) -> Any:
-278        """Load toml file."""
-279        return tomlkit.loads(self.read_text(encoding, errors))
+370        """Load toml file."""
+371        return tomlkit.loads(self.read_text(encoding, errors)).unwrap()
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
-281    def toml_dumps(
-282        self,
-283        data: Any,
-284        encoding: Any | None = None,
-285        errors: Any | None = None,
-286        newline: Any | None = None,
-287        sort_keys: bool = False,
-288        parents: bool = True,
-289    ):
-290        """Dump data to toml file."""
-291        self.write_text(
-292            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
+373    def toml_dumps(
+374        self,
+375        data: Any,
+376        encoding: Any | None = None,
+377        errors: Any | None = None,
+378        newline: Any | None = None,
+379        sort_keys: bool = False,
+380        parents: bool = True,
+381    ):
+382        """Dump `data` to toml file."""
+383        self.write_text(
+384            tomlkit.dumps(data, sort_keys), encoding, errors, newline,
 parents
-293        )
+385        )
 Dump data to toml file.
 ⁰
 def loads(
 self,
 encoding: typing.Any | None = None,
 errors: typing.Any | None = None) -> Any: View Source
-295    def loads(self, encoding: Any | None = None, errors: Any | None = None)
+387    def loads(self, encoding: Any | None = None, errors: Any | None = None)
 -> Any:
-296        """Load a json or toml file based off this instance's suffix."""
-297        match self.suffix:
-298            case ".json":
-299                return self.json_loads(encoding, errors)
-300            case ".toml":
-301                return self.toml_loads(encoding, errors)
+388        """Load a json or toml file based off this instance's suffix."""
+389        match self.suffix:
+390            case ".json":
+391                return self.json_loads(encoding, errors)
+392            case ".toml":
+393                return self.toml_loads(encoding, errors)
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
-303    def dumps(
-304        self,
-305        data: Any,
-306        encoding: Any | None = None,
-307        errors: Any | None = None,
-308        newline: Any | None = None,
-309        sort_keys: bool = False,
-310        indent: Any | None = None,
-311        default: Any | None = None,
-312        parents: bool = True,
-313    ):
-314        """Dump data to a json or toml file based off this instance's
+395    def dumps(
+396        self,
+397        data: Any,
+398        encoding: Any | None = None,
+399        errors: Any | None = None,
+400        newline: Any | None = None,
+401        sort_keys: bool = False,
+402        indent: Any | None = None,
+403        default: Any | None = None,
+404        parents: bool = True,
+405    ):
+406        """Dump `data` to a json or toml file based off this instance's
 suffix."""
-315        match self.suffix:
-316            case ".json":
-317                self.json_dumps(
-318                    data, encoding, errors, newline, sort_keys, indent,
+407        match self.suffix:
+408            case ".json":
+409                self.json_dumps(
+410                    data, encoding, errors, newline, sort_keys, indent,
 default, parents
-319                )
-320            case ".toml":
-321                self.toml_dumps(data, encoding, errors, newline, sort_keys,
+411                )
+412            case ".toml":
+413                self.toml_dumps(data, encoding, errors, newline, sort_keys,
 parents)
 Dump data to a json or toml file based off this instance's suffix.
 ⁰
 def delete(self, missing_ok: bool = True): View Source
-323    def delete(self, missing_ok: bool = True):
-324        """Delete the file or folder pointed to by this instance.
-325        Uses self.unlink() if a file and uses shutil.rmtree() if a
+415    def delete(self, missing_ok: bool = True):
+416        """Delete the file or folder pointed to by this instance.
+417
+418        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a
 directory."""
-326        if self.is_file():
-327            self.unlink(missing_ok)
-328        elif self.is_dir():
-329            shutil.rmtree(self)
-Delete the file or folder pointed to by this instance. Uses self.unlink() if a
-file and uses shutil.rmtree() if a directory.
+419        if self.is_file():
+420            self.unlink(missing_ok)
+421        elif self.is_dir():
+422            shutil.rmtree(self)
+Delete the file or folder pointed to by this instance.
+Uses self.unlink() if a file and uses shutil.rmtree() if a directory.
 ⁰
 def copy(
 self,
 new_path: Union[Self, pathlib.Path, str],
 overwrite: bool = False) -> Self: View Source
-331    def copy(
-332        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
-333    ) -> Self:
-334        """Copy the path pointed to by this instance
-335        to the instance pointed to by new_path using shutil.copyfile
-336        or shutil.copytree. Returns the new path.
-337
-338        :param new_path: The copy destination.
-339
-340        :param overwrite: If True, files already existing in new_path
-341        will be overwritten. If False, only files that don't exist in
-new_path
-342        will be copied."""
-343        new_path = Pathier(new_path)
-344        if self.is_dir():
-345            if overwrite or not new_path.exists():
-346                shutil.copytree(self, new_path, dirs_exist_ok=True)
-347            else:
-348                files = self.rglob("*.*")
-349                for file in files:
-350                    dst = new_path.with_name(file.name)
-351                    if not dst.exists():
-352                        shutil.copyfile(file, dst)
-353        elif self.is_file():
-354            if overwrite or not new_path.exists():
-355                shutil.copyfile(self, new_path)
-356        return new_path
+424    def copy(
+425        self, new_path: Self | pathlib.Path | str, overwrite: bool = False
+426    ) -> Self:
+427        """Copy the path pointed to by this instance
+428        to the instance pointed to by `new_path` using `shutil.copyfile`
+429        or `shutil.copytree`.
+430
+431        Returns the new path.
+432
+433        #### :params:
+434
+435        `new_path`: The copy destination.
+436
+437        `overwrite`: If `True`, files already existing in `new_path` will be
+overwritten.
+438        If `False`, only files that don't exist in `new_path` will be
+copied."""
+439        new_path = Pathier(new_path)
+440        if self.is_dir():
+441            if overwrite or not new_path.exists():
+442                shutil.copytree(self, new_path, dirs_exist_ok=True)
+443            else:
+444                files = self.rglob("*.*")
+445                for file in files:
+446                    dst = new_path.with_name(file.name)
+447                    if not dst.exists():
+448                        shutil.copyfile(file, dst)
+449        elif self.is_file():
+450            if overwrite or not new_path.exists():
+451                shutil.copyfile(self, new_path)
+452        return new_path
 Copy the path pointed to by this instance to the instance pointed to by
-new_path using shutil.copyfile or shutil.copytree. Returns the new path.
-* Parameters *
-    * new_path: The copy destination.
-    * overwrite: If True, files already existing in new_path will be
-      overwritten. If False, only files that don't exist in new_path will be
-      copied.
+new_path using shutil.copyfile or shutil.copytree.
+Returns the new path.
+*** :params: ***
+new_path: The copy destination.
+overwrite: If True, files already existing in new_path will be overwritten. If
+False, only files that don't exist in new_path will be copied.
 ⁰
 def backup(self, timestamp: bool = False) -> Optional[Self]: View Source
-358    def backup(self, timestamp: bool = False) -> Self | None:
-359        """Create a copy of this file or directory with `_backup` appended
+454    def backup(self, timestamp: bool = False) -> Self | None:
+455        """Create a copy of this file or directory with `_backup` appended
 to the path stem.
-360        If the path to be backed up doesn't exist, `None` is returned.
-361        Otherwise a `Pathier` object for the backup is returned.
-362
-363        :param `timestamp`: Add a timestamp to the backup name to prevent
+456        If the path to be backed up doesn't exist, `None` is returned.
+457        Otherwise a `Pathier` object for the backup is returned.
+458
+459        #### :params:
+460
+461        `timestamp`: Add a timestamp to the backup name to prevent
 overriding previous backups.
-364
-365        >>> path = Pathier("some_file.txt")
-366        >>> path.backup()
-367        >>> list(path.iterdir())
-368        >>> ['some_file.txt', 'some_file_backup.txt']
-369        >>> path.backup(True)
-370        >>> list(path.iterdir())
-371        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
+462
+463        >>> path = Pathier("some_file.txt")
+464        >>> path.backup()
+465        >>> list(path.iterdir())
+466        >>> ['some_file.txt', 'some_file_backup.txt']
+467        >>> path.backup(True)
+468        >>> list(path.iterdir())
+469        >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-
 28-2023-06_25_52_PM.txt']"""
-372        if not self.exists():
-373            return None
-374        backup_stem = f"{self.stem}_backup"
-375        if timestamp:
-376            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
+470        if not self.exists():
+471            return None
+472        backup_stem = f"{self.stem}_backup"
+473        if timestamp:
+474            backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime
 ('%m-%d-%Y-%I_%M_%S_%p')}"
-377        backup_path = self.with_stem(backup_stem)
-378        self.copy(backup_path, True)
-379        return backup_path
+475        backup_path = self.with_stem(backup_stem)
+476        self.copy(backup_path, True)
+477        return backup_path
 Create a copy of this file or directory with _backup appended to the path stem.
 If the path to be backed up doesn't exist, None is returned. Otherwise a
 Pathier object for the backup is returned.
-* Parameters *
-    * timestamp: Add a timestamp to the backup name to prevent overriding
-      previous backups.
+*** :params: ***
+timestamp: Add a timestamp to the backup name to prevent overriding previous
+backups.
 >>> path = Pathier("some_file.txt")
 >>> path.backup()
 >>> list(path.iterdir())
 >>> ['some_file.txt', 'some_file_backup.txt']
 >>> path.backup(True)
 >>> list(path.iterdir())
 >>> ['some_file.txt', 'some_file_backup.txt', 'some_file_backup_04-28-2023-
 06_25_52_PM.txt']
+⁰
+def execute(self, command: str = '', args: str = '') -> int: View Source
+479    def execute(self, command: str = "", args: str = "") -> int:
+480        """Make a call to `os.system` using the path pointed to by this
+Pathier object.
+481
+482        #### :params:
+483
+484        `command`: Program/command to precede the path with.
+485
+486        `args`: Any arguments that should come after the path.
+487
+488        :returns: The integer output of `os.system`.
+489
+490        e.g.
+491        >>> path = Pathier("mydirectory") / "myscript.py"
+492        then
+493        >>> path.execute("py", "--iterations 10")
+494        equivalent to
+495        >>> os.system(f"py {path} --iterations 10")"""
+496        return os.system(f"{command} {self} {args}")
+Make a call to os.system using the path pointed to by this Pathier object.
+*** :params: ***
+command: Program/command to precede the path with.
+args: Any arguments that should come after the path.
+:returns: The integer output of os.system.
+e.g.
+>>> path = Pathier("mydirectory") / "myscript.py"
+then
+>>> path.execute("py", "--iterations 10")
+equivalent to
+>>> os.system(f"py {path} --iterations 10")
 ** Inherited Members **
 
+Pathy = pathier.Pathier | pathlib.Path
+
+Pathish = pathier.Pathier | pathlib.Path | str
+
```

### Comparing `pathier-0.9.0/src/pathier/pathier.py` & `pathier-1.0.0/src/pathier/pathier.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,16 +24,15 @@
                 "cannot instantiate %r on your system" % (cls.__name__,)
             )
         return self
 
     # ===============================================stats===============================================
     @property
     def dob(self) -> datetime.datetime | None:
-        """Returns the creation date of this file
-        or directory as a dateime.datetime object."""
+        """Returns the creation date of this file or directory as a `dateime.datetime` object."""
         if self.exists():
             return datetime.datetime.fromtimestamp(self.stat().st_ctime)
         else:
             return None
 
     @property
     def age(self) -> float | None:
@@ -41,181 +40,210 @@
         if self.exists():
             return (datetime.datetime.now() - self.dob).total_seconds()
         else:
             return None
 
     @property
     def mod_date(self) -> datetime.datetime | None:
-        """Returns the modification date of this file
-        or directory as a datetime.datetime object."""
+        """Returns the modification date of this file or directory as a `datetime.datetime` object."""
         if self.exists():
             return datetime.datetime.fromtimestamp(self.stat().st_mtime)
         else:
             return None
 
     @property
     def mod_delta(self) -> float | None:
-        """Returns how long ago in seconds this file
-        or directory was modified."""
+        """Returns how long ago in seconds this file or directory was modified."""
         if self.exists():
             return (datetime.datetime.now() - self.mod_date).total_seconds()
         else:
             return None
 
-    def size(self, format: bool = False) -> int | str | None:
+    @property
+    def last_read_time(self) -> datetime.datetime | None:
+        """Returns the last time this object made a call to `self.read_text()`, `self.read_bytes()`, or `self.open(mode="r"|"rb")`.
+        Returns `None` if the file hasn't been read from.
+
+        Note: This property is only relative to the lifetime of this `Pathier` instance, not the file itself.
+        i.e. This property will reset if you create a new `Pathier` object pointing to the same file."""
+        if self._last_read_time:
+            return datetime.datetime.fromtimestamp(self._last_read_time)
+        else:
+            return self._last_read_time
+
+    @property
+    def modified_since_last_read(self) -> bool:
+        """Returns `True` if this file hasn't been read from or has been modified since the last time this object
+        made a call to `self.read_text()`, `self.read_bytes()`, or `self.open(mode="r"|"rb")`.
+
+        Note: This property is only relative to the lifetime of this `Pathier` instance, not the file itself.
+        i.e. This property will reset if you create a new `Pathier` object pointing to the same file.
+
+        #### Caveat:
+        May not be accurate if the file was modified within a couple of seconds of checking this property.
+        (For instance, on my machine `self.mod_date` is consistently 1-1.5s in the future from when `self.write_text()` was called according to `time.time()`.)
+        """
+
+        return self.last_read_time is None or self.mod_date > self.last_read_time
+
+    @property
+    def size(self) -> int:
         """Returns the size in bytes of this file or directory.
-        Returns None if this path doesn't exist.
 
-        :param format: If True, return value as a formatted string."""
+        If this path doesn't exist, `0` will be returned."""
         if not self.exists():
-            return None
-        if self.is_file():
-            size = self.stat().st_size
-        if self.is_dir():
-            size = sum(file.stat().st_size for file in self.rglob("*.*"))
-        if format:
-            return self.format_size(size)
-        return size
+            return 0
+        elif self.is_file():
+            return self.stat().st_size
+        elif self.is_dir():
+            return sum(file.stat().st_size for file in self.rglob("*.*"))
+        return 0
 
     @staticmethod
-    def format_size(size: int) -> str:
-        """Format 'size' with common file size abbreviations
-        and rounded to two decimal places.
+    def format_bytes(size: int) -> str:
+        """Format `size` with common file size abbreviations and rounded to two decimal places.
         >>> 1234 -> "1.23 kb" """
         for unit in ["bytes", "kb", "mb", "gb", "tb", "pb"]:
             if unit != "bytes":
                 size *= 0.001
             if size < 1000 or unit == "pb":
                 return f"{round(size, 2)} {unit}"
 
     def is_larger(self, path: Self) -> bool:
-        """Returns whether this file or folder is larger than
-        the one pointed to by 'path'."""
-        return self.size() > path.size()
+        """Returns whether this file or folder is larger than the one pointed to by `path`."""
+        return self.size > path.size
 
     def is_older(self, path: Self) -> bool:
-        """Returns whether this file or folder is older than
-        the one pointed to by 'path'."""
+        """Returns whether this file or folder is older than the one pointed to by `path`."""
         return self.dob < path.dob
 
     def modified_more_recently(self, path: Self) -> bool:
-        """Returns whether this file or folder was modified
-        more recently than the one pointed to by 'path'."""
+        """Returns whether this file or folder was modified more recently than the one pointed to by `path`."""
         return self.mod_date > path.mod_date
 
     # ===============================================navigation===============================================
     def mkcwd(self):
         """Make this path your current working directory."""
         os.chdir(self)
 
     @property
     def in_PATH(self) -> bool:
-        """Return True if this
-        path is in sys.path."""
+        """Return `True` if this path is in `sys.path`."""
         return str(self) in sys.path
 
     def add_to_PATH(self, index: int = 0):
-        """Insert this path into sys.path
-        if it isn't already there.
+        """Insert this path into `sys.path` if it isn't already there.
+
+        #### :params:
 
-        :param index: The index of sys.path
-        to insert this path at."""
+        `index`: The index of `sys.path` to insert this path at."""
         path = str(self)
         if not self.in_PATH:
             sys.path.insert(index, path)
 
     def append_to_PATH(self):
-        """Append this path to sys.path
-        if it isn't already there."""
+        """Append this path to `sys.path` if it isn't already there."""
         path = str(self)
         if not self.in_PATH:
             sys.path.append(path)
 
     def remove_from_PATH(self):
-        """Remove this path from sys.path
-        if it's in sys.path."""
+        """Remove this path from `sys.path` if it's in `sys.path`."""
         if self.in_PATH:
             sys.path.remove(str(self))
 
     def moveup(self, name: str) -> Self:
-        """Return a new Pathier object that is a parent of this instance.
-        'name' is case-sensitive and raises an exception if it isn't in self.parts.
+        """Return a new `Pathier` object that is a parent of this instance.
+
+        `name` is case-sensitive and raises an exception if it isn't in `self.parts`.
         >>> p = Pathier("C:\some\directory\in\your\system")
         >>> print(p.moveup("directory"))
         >>> "C:\some\directory"
         >>> print(p.moveup("yeet"))
         >>> "Exception: yeet is not a parent of C:\some\directory\in\your\system" """
         if name not in self.parts:
             raise Exception(f"{name} is not a parent of {self}")
         return Pathier(*(self.parts[: self.parts.index(name) + 1]))
 
     def __sub__(self, levels: int) -> Self:
-        """Return a new Pathier object moved up 'levels' number of parents from the current path.
+        """Return a new `Pathier` object moved up `levels` number of parents from the current path.
         >>> p = Pathier("C:\some\directory\in\your\system")
         >>> new_p = p - 3
         >>> print(new_p)
         >>> "C:\some\directory" """
         path = self
         for _ in range(levels):
             path = path.parent
         return path
 
     def move_under(self, name: str) -> Self:
-        """Return a new Pathier object such that the stem
-        is one level below the folder 'name'.
-        'name' is case-sensitive and raises an exception if it isn't in self.parts.
+        """Return a new `Pathier` object such that the stem is one level below the given folder `name`.
+
+        `name` is case-sensitive and raises an exception if it isn't in `self.parts`.
         >>> p = Pathier("a/b/c/d/e/f/g")
         >>> print(p.move_under("c"))
         >>> 'a/b/c/d'"""
         if name not in self.parts:
             raise Exception(f"{name} is not a parent of {self}")
         return self - (len(self.parts) - self.parts.index(name) - 2)
 
     def separate(self, name: str, keep_name: bool = False) -> Self:
-        """Return a new Pathier object that is the
-        relative child path after 'name'.
-        'name' is case-sensitive and raises an exception if it isn't in self.parts.
+        """Return a new `Pathier` object that is the relative child path after `name`.
+
+        `name` is case-sensitive and raises an exception if it isn't in `self.parts`.
 
-        :param keep_name: If True, the returned path will start with 'name'.
+        #### :params:
+
+        `keep_name`: If `True`, the returned path will start with `name`.
         >>> p = Pathier("a/b/c/d/e/f/g")
         >>> print(p.separate("c"))
         >>> 'd/e/f/g'
         >>> print(p.separate("c", True))
         >>> 'c/d/e/f/g'"""
         if name not in self.parts:
             raise Exception(f"{name} is not a parent of {self}")
         if keep_name:
             return Pathier(*self.parts[self.parts.index(name) :])
         return Pathier(*self.parts[self.parts.index(name) + 1 :])
 
     # ============================================write and read============================================
     def mkdir(self, mode: int = 511, parents: bool = True, exist_ok: bool = True):
         """Create this directory.
-        Same as Path().mkdir() except
-        'parents' and 'exist_ok' default
-        to True instead of False."""
+
+        Same as `Path().mkdir()` except `parents` and `exist_ok` default to `True` instead of `False`."""
         super().mkdir(mode, parents, exist_ok)
 
     def touch(self):
-        """Create file and parents if necessary."""
+        """Create file (and parents if necessary)."""
         self.parent.mkdir()
         super().touch()
 
+    def open(self, mode="r", buffering=-1, encoding=None, errors=None, newline=None):
+        """
+        Open the file pointed by this path and return a file object, as
+        the built-in open() function does.
+        """
+        stream = super().open(mode, buffering, encoding, errors, newline)
+        if "r" in mode:
+            self._last_read_time = time.time()
+        return stream
+
     def write_text(
         self,
         data: Any,
         encoding: Any | None = None,
         errors: Any | None = None,
         newline: Any | None = None,
         parents: bool = True,
     ):
-        """Write data to file. If a TypeError is raised, the function
-        will attempt to case data to a str and try the write again.
-        If a FileNotFoundError is raised and parents = True,
-        self.parent will be created."""
+        """Write data to file.
+
+        If a `TypeError` is raised, the function  will attempt to cast `data` to a `str` and try the write again.
+
+        If a `FileNotFoundError` is raised and `parents = True`, `self.parent` will be created."""
         write = functools.partial(
             super().write_text,
             encoding=encoding,
             errors=errors,
             newline=newline,
         )
         try:
@@ -231,28 +259,92 @@
                 raise
         except Exception as e:
             raise
 
     def write_bytes(self, data: bytes, parents: bool = True):
         """Write bytes to file.
 
-        :param parents: If True and the write operation fails
-        with a FileNotFoundError, make the parent directory
-        and retry the write."""
+        #### :params:
+
+        `parents`: If `True` and the write operation fails with a `FileNotFoundError`,
+        make the parent directory and retry the write."""
         try:
             super().write_bytes(data)
         except FileNotFoundError:
             if parents:
                 self.parent.mkdir(parents=True)
                 super().write_bytes(data)
             else:
                 raise
         except Exception as e:
             raise
 
+    def append(self, data: str, new_line: bool = True, encoding: Any | None = None):
+        """Append `data` to the file pointed to by this `Pathier` object.
+
+        #### :params:
+
+        `new_line`: If `True`, add `\\n` to `data`.
+
+        `encoding`: The file encoding to use."""
+        if new_line:
+            data += "\n"
+        with self.open("a", encoding=encoding) as file:
+            file.write(data)
+
+    def replace(
+        self,
+        substitutions: list[tuple[str, str]],
+        count: int = -1,
+        encoding: Any | None = None,
+    ):
+        """For each pair in `substitutions`, replace the first string with the second string.
+
+        #### :params:
+
+        `count`: Only replace this many occurences of each pair.
+        By default (`-1`), all occurences are replaced.
+
+        `encoding`: The file encoding to use.
+
+        e.g.
+        >>> path = Pathier("somefile.txt")
+        >>>
+        >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
+        equivalent to
+        >>> path.write_text(path.read_text().replace("hello", "yeet").replace("goodbye", "yeehaw"))"""
+        text = self.read_text(encoding)
+        for sub in substitutions:
+            text = text.replace(sub[0], sub[1], count)
+        self.write_text(text, encoding=encoding)
+
+    def join(self, data: list[str], encoding: Any | None = None, sep: str = "\n"):
+        """Write a list of strings, joined by `sep`, to the file pointed at by this instance.
+
+        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data), encoding=encoding)`
+
+        #### :params:
+
+        `encoding`: The file encoding to use.
+
+        `sep`: The separator to use when joining `data`."""
+        self.write_text(sep.join(data), encoding=encoding)
+
+    def split(self, encoding: Any | None = None, keepends: bool = False) -> list[str]:
+        """Returns the content of the pointed at file as a list of strings, splitting at new line characters.
+
+        Equivalent to `Pathier("somefile.txt").read_text(encoding=encoding).splitlines()`
+
+        #### :params:
+
+        `encoding`: The file encoding to use.
+
+        `keepend`: If `True`, line breaks will be included in returned strings."""
+        return self.read_text(encoding=encoding).splitlines(keepends)
+
     def json_loads(self, encoding: Any | None = None, errors: Any | None = None) -> Any:
         """Load json file."""
         return json.loads(self.read_text(encoding, errors))
 
     def json_dumps(
         self,
         data: Any,
@@ -260,37 +352,37 @@
         errors: Any | None = None,
         newline: Any | None = None,
         sort_keys: bool = False,
         indent: Any | None = None,
         default: Any | None = None,
         parents: bool = True,
     ) -> Any:
-        """Dump data to json file."""
+        """Dump `data` to json file."""
         self.write_text(
             json.dumps(data, indent=indent, default=default, sort_keys=sort_keys),
             encoding,
             errors,
             newline,
             parents,
         )
 
     def toml_loads(self, encoding: Any | None = None, errors: Any | None = None) -> Any:
         """Load toml file."""
-        return tomlkit.loads(self.read_text(encoding, errors))
+        return tomlkit.loads(self.read_text(encoding, errors)).unwrap()
 
     def toml_dumps(
         self,
         data: Any,
         encoding: Any | None = None,
         errors: Any | None = None,
         newline: Any | None = None,
         sort_keys: bool = False,
         parents: bool = True,
     ):
-        """Dump data to toml file."""
+        """Dump `data` to toml file."""
         self.write_text(
             tomlkit.dumps(data, sort_keys), encoding, errors, newline, parents
         )
 
     def loads(self, encoding: Any | None = None, errors: Any | None = None) -> Any:
         """Load a json or toml file based off this instance's suffix."""
         match self.suffix:
@@ -306,43 +398,47 @@
         errors: Any | None = None,
         newline: Any | None = None,
         sort_keys: bool = False,
         indent: Any | None = None,
         default: Any | None = None,
         parents: bool = True,
     ):
-        """Dump data to a json or toml file based off this instance's suffix."""
+        """Dump `data` to a json or toml file based off this instance's suffix."""
         match self.suffix:
             case ".json":
                 self.json_dumps(
                     data, encoding, errors, newline, sort_keys, indent, default, parents
                 )
             case ".toml":
                 self.toml_dumps(data, encoding, errors, newline, sort_keys, parents)
 
     def delete(self, missing_ok: bool = True):
         """Delete the file or folder pointed to by this instance.
-        Uses self.unlink() if a file and uses shutil.rmtree() if a directory."""
+
+        Uses `self.unlink()` if a file and uses `shutil.rmtree()` if a directory."""
         if self.is_file():
             self.unlink(missing_ok)
         elif self.is_dir():
             shutil.rmtree(self)
 
     def copy(
         self, new_path: Self | pathlib.Path | str, overwrite: bool = False
     ) -> Self:
         """Copy the path pointed to by this instance
-        to the instance pointed to by new_path using shutil.copyfile
-        or shutil.copytree. Returns the new path.
+        to the instance pointed to by `new_path` using `shutil.copyfile`
+        or `shutil.copytree`.
+
+        Returns the new path.
 
-        :param new_path: The copy destination.
+        #### :params:
 
-        :param overwrite: If True, files already existing in new_path
-        will be overwritten. If False, only files that don't exist in new_path
-        will be copied."""
+        `new_path`: The copy destination.
+
+        `overwrite`: If `True`, files already existing in `new_path` will be overwritten.
+        If `False`, only files that don't exist in `new_path` will be copied."""
         new_path = Pathier(new_path)
         if self.is_dir():
             if overwrite or not new_path.exists():
                 shutil.copytree(self, new_path, dirs_exist_ok=True)
             else:
                 files = self.rglob("*.*")
                 for file in files:
@@ -355,15 +451,17 @@
         return new_path
 
     def backup(self, timestamp: bool = False) -> Self | None:
         """Create a copy of this file or directory with `_backup` appended to the path stem.
         If the path to be backed up doesn't exist, `None` is returned.
         Otherwise a `Pathier` object for the backup is returned.
 
-        :param `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.
+        #### :params:
+
+        `timestamp`: Add a timestamp to the backup name to prevent overriding previous backups.
 
         >>> path = Pathier("some_file.txt")
         >>> path.backup()
         >>> list(path.iterdir())
         >>> ['some_file.txt', 'some_file_backup.txt']
         >>> path.backup(True)
         >>> list(path.iterdir())
@@ -373,14 +471,39 @@
         backup_stem = f"{self.stem}_backup"
         if timestamp:
             backup_stem = f"{backup_stem}_{datetime.datetime.now().strftime('%m-%d-%Y-%I_%M_%S_%p')}"
         backup_path = self.with_stem(backup_stem)
         self.copy(backup_path, True)
         return backup_path
 
+    def execute(self, command: str = "", args: str = "") -> int:
+        """Make a call to `os.system` using the path pointed to by this Pathier object.
+
+        #### :params:
+
+        `command`: Program/command to precede the path with.
+
+        `args`: Any arguments that should come after the path.
+
+        :returns: The integer output of `os.system`.
+
+        e.g.
+        >>> path = Pathier("mydirectory") / "myscript.py"
+        then
+        >>> path.execute("py", "--iterations 10")
+        equivalent to
+        >>> os.system(f"py {path} --iterations 10")"""
+        return os.system(f"{command} {self} {args}")
+
+
+Pathy = Pathier | pathlib.Path
+Pathish = Pathier | pathlib.Path | str
+
 
 class PosixPath(Pathier, pathlib.PurePosixPath):
     __slots__ = ()
+    _last_read_time = None
 
 
 class WindowsPath(Pathier, pathlib.PureWindowsPath):
     __slots__ = ()
+    _last_read_time = None
```

### Comparing `pathier-0.9.0/LICENSE.txt` & `pathier-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathier-0.9.0/pyproject.toml` & `pathier-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -5,65 +5,62 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 7061 7468 6965 7222 0d0a 6465 7363   "pathier"..desc
 00000070: 7269 7074 696f 6e20 3d20 2245 7874 656e  ription = "Exten
 00000080: 6473 2074 6865 2073 7461 6e64 6172 6420  ds the standard 
 00000090: 6c69 6272 6172 7920 7061 7468 6c69 622e  library pathlib.
 000000a0: 5061 7468 2063 6c61 7373 2e22 0d0a 7665  Path class."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e39 2e30 220d  rsion = "0.9.0".
+000000b0: 7273 696f 6e20 3d20 2231 2e30 2e30 220d  rsion = "1.0.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 746f  endencies = ["to
-000000f0: 6d6c 6b69 7422 2c20 2270 7974 6573 7422  mlkit", "pytest"
-00000100: 2c20 2274 7970 696e 675f 6578 7465 6e73  , "typing_extens
-00000110: 696f 6e73 225d 0d0a 7265 6164 6d65 203d  ions"]..readme =
-00000120: 2022 5245 4144 4d45 2e6d 6422 0d0a 6b65   "README.md"..ke
-00000130: 7977 6f72 6473 203d 205b 2270 6174 686c  ywords = ["pathl
-00000140: 6962 222c 2022 7061 7468 222c 2022 6a73  ib", "path", "js
-00000150: 6f6e 222c 2022 746f 6d6c 222c 2022 7368  on", "toml", "sh
-00000160: 7574 696c 222c 2022 6578 7465 6e64 6572  util", "extender
-00000170: 222c 2022 6578 7465 6e73 696f 6e22 5d0d  ", "extension"].
-00000180: 0a63 6c61 7373 6966 6965 7273 203d 205b  .classifiers = [
-00000190: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
-000001a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001b0: 7974 686f 6e20 3a3a 2033 222c 0d0a 2020  ython :: 3",..  
-000001c0: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
-000001d0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000001e0: 5420 4c69 6365 6e73 6522 2c0d 0a20 2020  T License",..   
-000001f0: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
-00000200: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000210: 6465 6e74 222c 0d0a 2020 2020 5d0d 0a0d  dent",..    ]...
-00000220: 0a5b 5b70 726f 6a65 6374 2e61 7574 686f  .[[project.autho
-00000230: 7273 5d5d 0d0a 6e61 6d65 203d 2022 4d61  rs]]..name = "Ma
-00000240: 7474 204d 616e 6573 220d 0a65 6d61 696c  tt Manes"..email
-00000250: 203d 2022 6d61 7474 6d61 6e65 7340 706d   = "mattmanes@pm
-00000260: 2e6d 6522 0d0a 0d0a 5b70 726f 6a65 6374  .me"....[project
-00000270: 2e75 726c 735d 0d0a 2248 6f6d 6570 6167  .urls].."Homepag
-00000280: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
-00000290: 7468 7562 2e63 6f6d 2f6d 6174 742d 6d61  thub.com/matt-ma
-000002a0: 6e65 732f 7061 7468 6965 7222 0d0a 2244  nes/pathier".."D
-000002b0: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
-000002c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000002d0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f70  com/matt-manes/p
-000002e0: 6174 6869 6572 2f74 7265 652f 6d61 696e  athier/tree/main
-000002f0: 2f64 6f63 7322 0d0a 2253 6f75 7263 6520  /docs".."Source 
-00000300: 636f 6465 2220 3d20 2268 7474 7073 3a2f  code" = "https:/
-00000310: 2f67 6974 6875 622e 636f 6d2f 6d61 7474  /github.com/matt
-00000320: 2d6d 616e 6573 2f70 6174 6869 6572 2f74  -manes/pathier/t
-00000330: 7265 652f 6d61 696e 2f73 7263 2f70 6174  ree/main/src/pat
-00000340: 6869 6572 220d 0a0d 0a5b 746f 6f6c 2e70  hier"....[tool.p
-00000350: 7974 6573 742e 696e 695f 6f70 7469 6f6e  ytest.ini_option
-00000360: 735d 0d0a 6164 646f 7074 7320 3d20 5b0d  s]..addopts = [.
-00000370: 0a20 2020 2022 2d2d 696d 706f 7274 2d6d  .    "--import-m
-00000380: 6f64 653d 696d 706f 7274 6c69 6222 2c0d  ode=importlib",.
-00000390: 0a20 2020 205d 0d0a 7079 7468 6f6e 7061  .    ]..pythonpa
-000003a0: 7468 203d 2022 7372 6322 0d0a 0d0a 5b74  th = "src"....[t
-000003b0: 6f6f 6c2e 6861 7463 682e 6275 696c 642e  ool.hatch.build.
-000003c0: 7461 7267 6574 732e 7364 6973 745d 0d0a  targets.sdist]..
-000003d0: 6578 636c 7564 6520 3d20 5b0d 0a20 2020  exclude = [..   
-000003e0: 2022 2e63 6f76 6572 6167 6522 2c0d 0a20   ".coverage",.. 
-000003f0: 2020 2022 2e70 7974 6573 745f 6361 6368     ".pytest_cach
-00000400: 6522 2c0d 0a20 2020 2022 2e76 7363 6f64  e",..    ".vscod
-00000410: 6522 2c0d 0a20 2020 2022 7465 7374 7322  e",..    "tests"
-00000420: 2c0d 0a20 2020 2022 2e67 6974 6967 6e6f  ,..    ".gitigno
-00000430: 7265 220d 0a20 2020 205d 0d0a 5b70 726f  re"..    ]..[pro
-00000440: 6a65 6374 2e73 6372 6970 7473 5d         ject.scripts]
+000000f0: 6d6c 6b69 743e 3d30 2e31 312e 3822 2c20  mlkit>=0.11.8", 
+00000100: 2270 7974 6573 7422 2c20 2274 7970 696e  "pytest", "typin
+00000110: 675f 6578 7465 6e73 696f 6e73 225d 0d0a  g_extensions"]..
+00000120: 7265 6164 6d65 203d 2022 5245 4144 4d45  readme = "README
+00000130: 2e6d 6422 0d0a 6b65 7977 6f72 6473 203d  .md"..keywords =
+00000140: 205b 2270 6174 686c 6962 222c 2022 7061   ["pathlib", "pa
+00000150: 7468 222c 2022 6a73 6f6e 222c 2022 746f  th", "json", "to
+00000160: 6d6c 222c 2022 7368 7574 696c 222c 2022  ml", "shutil", "
+00000170: 6578 7465 6e64 6572 222c 2022 6578 7465  extender", "exte
+00000180: 6e73 696f 6e22 5d0d 0a63 6c61 7373 6966  nsion"]..classif
+00000190: 6965 7273 203d 205b 2250 726f 6772 616d  iers = ["Program
+000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001b0: 2050 7974 686f 6e20 3a3a 2033 222c 2022   Python :: 3", "
+000001c0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001d0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001e0: 6963 656e 7365 222c 2022 4f70 6572 6174  icense", "Operat
+000001f0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000200: 2049 6e64 6570 656e 6465 6e74 225d 0d0a   Independent"]..
+00000210: 0d0a 5b5b 7072 6f6a 6563 742e 6175 7468  ..[[project.auth
+00000220: 6f72 735d 5d0d 0a6e 616d 6520 3d20 224d  ors]]..name = "M
+00000230: 6174 7420 4d61 6e65 7322 0d0a 656d 6169  att Manes"..emai
+00000240: 6c20 3d20 226d 6174 746d 616e 6573 4070  l = "mattmanes@p
+00000250: 6d2e 6d65 220d 0a0d 0a5b 7072 6f6a 6563  m.me"....[projec
+00000260: 742e 7572 6c73 5d0d 0a48 6f6d 6570 6167  t.urls]..Homepag
+00000270: 6520 3d20 2268 7474 7073 3a2f 2f67 6974  e = "https://git
+00000280: 6875 622e 636f 6d2f 6d61 7474 2d6d 616e  hub.com/matt-man
+00000290: 6573 2f70 6174 6869 6572 220d 0a44 6f63  es/pathier"..Doc
+000002a0: 756d 656e 7461 7469 6f6e 203d 2022 6874  umentation = "ht
+000002b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000002c0: 2f6d 6174 742d 6d61 6e65 732f 7061 7468  /matt-manes/path
+000002d0: 6965 722f 7472 6565 2f6d 6169 6e2f 646f  ier/tree/main/do
+000002e0: 6373 220d 0a22 536f 7572 6365 2063 6f64  cs".."Source cod
+000002f0: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
+00000300: 7468 7562 2e63 6f6d 2f6d 6174 742d 6d61  thub.com/matt-ma
+00000310: 6e65 732f 7061 7468 6965 722f 7472 6565  nes/pathier/tree
+00000320: 2f6d 6169 6e2f 7372 632f 7061 7468 6965  /main/src/pathie
+00000330: 7222 0d0a 0d0a 5b70 726f 6a65 6374 2e73  r"....[project.s
+00000340: 6372 6970 7473 5d0d 0a0d 0a5b 746f 6f6c  cripts]....[tool
+00000350: 5d0d 0a5b 746f 6f6c 2e70 7974 6573 742e  ]..[tool.pytest.
+00000360: 696e 695f 6f70 7469 6f6e 735d 0d0a 6164  ini_options]..ad
+00000370: 646f 7074 7320 3d20 5b22 2d2d 696d 706f  dopts = ["--impo
+00000380: 7274 2d6d 6f64 653d 696d 706f 7274 6c69  rt-mode=importli
+00000390: 6222 5d0d 0a70 7974 686f 6e70 6174 6820  b"]..pythonpath 
+000003a0: 3d20 2273 7263 220d 0a0d 0a5b 746f 6f6c  = "src"....[tool
+000003b0: 2e68 6174 6368 2e62 7569 6c64 2e74 6172  .hatch.build.tar
+000003c0: 6765 7473 2e73 6469 7374 5d0d 0a65 7863  gets.sdist]..exc
+000003d0: 6c75 6465 203d 205b 222e 636f 7665 7261  lude = [".covera
+000003e0: 6765 222c 2022 2e70 7974 6573 745f 6361  ge", ".pytest_ca
+000003f0: 6368 6522 2c20 222e 7673 636f 6465 222c  che", ".vscode",
+00000400: 2022 7465 7374 7322 2c20 222e 6769 7469   "tests", ".giti
+00000410: 676e 6f72 6522 5d0d 0a                   gnore"]..
```

### Comparing `pathier-0.9.0/PKG-INFO` & `pathier-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pathier
-Version: 0.9.0
+Version: 1.0.0
 Summary: Extends the standard library pathlib.Path class.
 Project-URL: Homepage, https://github.com/matt-manes/pathier
 Project-URL: Documentation, https://github.com/matt-manes/pathier/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/pathier/tree/main/src/pathier
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: extender,extension,json,path,pathlib,shutil,toml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pytest
-Requires-Dist: tomlkit
+Requires-Dist: tomlkit>=0.11.8
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # pathier
 
 Extends the standard library pathlib.Path class.
 
@@ -57,15 +57,15 @@
 >>> path.separate("file", True)
 WindowsPath('file/on/the/system')
 >>> path.mkcwd()
 >>> Pathier.cwd()
 WindowsPath('C:/some/directory/to/some/file/on/the/system')
 </pre>
 
-#### PATH
+#### Environment PATH Variable
 
 Pathier objects can be added and removed from sys.path:<br>
 (The path will only be added if it isn't already in sys.path)
 <pre>
 >>> from pathier import Pathier
 >>> path = Pathier.cwd()
 >>> path.in_PATH
@@ -97,32 +97,49 @@
 `Pathier().write_text()` and `Pathier().write_bytes()` will create parent directories by default if they won't exist.<br>
 
 `Pathier().write_text()` will also try to cast the data to be written to a string if a TypeError is thrown.<br>
 
 `Pathier().delete()` will delete a file or directory, event if that directory isn't empty.<br>
 
 `Pathier().copy()` will copy a file or a directory tree to a new destination and return a Pathier object for the new path<br>
-By default, files in the destination will not be overwritten.
+By default, files in the destination will not be overwritten.<br>
 
+`Pathier().backup()` will create a copy of the path with `_backup` appended to the stem.
+If the optional parameter, `timestamp`, is `True`, a datetime string will be added after `_backup` to prevent overwriting previous backup files.<br>
+
+`Pathier().replace()` takes a list of string pairs and will read the file the instance points to, replace the first of each pair with the second of each pair, and then write it back to the file.<br>
+Essentially just condenses reading the file, using str.replace(), and then writing the new content into one function call.<br>
+
+`Pathier().execute()` wraps calling `os.system()` on the path pointed to be the `Pathier` instance.<br>
+Optional strings that should come before and after the path string can be specified with the `command` and `args` params, respectively.<br>
+`Pathier("file.py").execute("py", "--iterations 10")` is equivalent to `os.system("py file.py --iterations 10")`<br>
+
+`Pathier().append()` will append the given string to the file pointed at by the instance.<br>
+
+`Pathier().join(data)` is equivalent to calling `Pathier().write_text("\n".join(data))`.<br>
+The joining string can be specified with the `sep` parameter.<br>
+
+`Pathier().split()` is equivalent to calling `Pathier().read_text().splitlines()`.<br>
+Optionally, line endings can be kept with `Pathier().split(keepends=True)`.<br>
 #### Stats and Comparisons
 <pre>
 >>> from pathier import Pathier
 >>> p = Pathier.cwd() / "pathier.py"
 >>> i = p.parent / "__init__.py"
 >>> p.dob
 datetime.datetime(2023, 3, 31, 18, 43, 12, 360000)
 >>> p.age
 8846.024934
 >>> p.mod_date
 datetime.datetime(2023, 3, 31, 21, 7, 30)
 >>> p.mod_delta
 207.488857
->>> p.size()
+>>> p.size
 10744
->>> p.size(True)
+>>> p.format_bytes(p.size)
 '10.74 kb'
 >>> p.is_larger(i)
 True
 >>> p.is_older(i)
 False
 >>> p.modified_more_recently(i)
 True
```

